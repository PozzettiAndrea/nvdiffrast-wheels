# nvdiffrast Prebuilt Wheels

Prebuilt [nvdiffrast](https://github.com/NVlabs/nvdiffrast) wheels with compiled CUDA extensions for Windows.

These wheels include pre-compiled `.pyd` extensions so you don't need CUDA toolkit or Visual Studio to use nvdiffrast.

## Available Wheels

| CUDA Version | PyTorch Version | Python | Platform |
|--------------|-----------------|--------|----------|
| 12.4 | 2.4.1 | 3.10 | Windows x64 |

## Installation

```bash
pip install nvdiffrast --find-links https://pozzettiandrea.github.io/nvdiffrast-wheels/cu124/
```

Or specify version explicitly:
```bash
pip install nvdiffrast==0.3.5+pt2.4.1cu124 --find-links https://pozzettiandrea.github.io/nvdiffrast-wheels/cu124/
```

## Why?

nvdiffrast normally requires JIT compilation at runtime, which needs:
- CUDA Toolkit with nvcc
- Visual Studio with C++ build tools
- Matching versions of everything

These prebuilt wheels skip all that - just install and use.

## Build Info

Built with:
- CUDA 12.4
- PyTorch 2.4.1+cu124
- Visual Studio 2025 Preview (MSVC 19.43)
- Python 3.10.11
- CUDA architectures: 6.1, 7.0, 7.5, 8.0, 8.6, 8.9, 9.0

## License

nvdiffrast is licensed by NVIDIA. See [NVlabs/nvdiffrast](https://github.com/NVlabs/nvdiffrast) for license details.

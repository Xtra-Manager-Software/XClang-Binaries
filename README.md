# XClang-Binaries

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
[![LLVM](https://img.shields.io/badge/Based%20on-LLVM%20Project-orange.svg)](https://llvm.org/)

Pre-compiled Clang Compiler binaries for Android and other platforms.

## Description

XClang is a public repository providing pre-compiled binaries of the Clang compiler built on top of the LLVM Project. This repository contains ready-to-use binaries for various development purposes, particularly for Android development.

**Note**: This is a binaries-only repository. The build process and source modifications are maintained in a separate private repository.

## Features

- Latest Clang compiler with custom optimizations
- Complete header files for C/C++ development
- Support for multiple target architectures
- Performance-optimized binaries
- Compatible with Android NDK

## Package Contents

```
XClang-22.tar.gz          # Compiler binary archive
├── bin/                  # Executable binaries
├── include/              # Header files
│   └── clang/           # Clang-specific headers
│       ├── AST/         # Abstract Syntax Tree
│       ├── Analysis/    # Code analysis tools
│       ├── Basic/       # Basic utilities
│       ├── CodeGen/     # Code generation
│       └── ...          # And more
└── lib/                 # Libraries (if any)
```

## Installation

### Download

Download the latest release from the [Releases page](https://github.com/Xtra-Manager-Software/XClang-Binaries/releases).

### Add to PATH (Optional)

```bash
export PATH=$PATH:/path/to/xclang/bin
```

Or add to `~/.bashrc` or `~/.zshrc` for permanent setup:

```bash
echo 'export PATH=$PATH:/path/to/xclang/bin' >> ~/.bashrc
source ~/.bashrc
```

## Usage

### Compile C File

```bash
clang -o output program.c
```

### Compile C++ File

```bash
clang++ -o output program.cpp
```

### With Optimization

```bash
clang -O2 -o output program.c
```

### Cross-compile for Android

```bash
clang --target=aarch64-linux-android -o output program.c
```

## System Requirements

- Linux (x86_64 or ARM64)
- Minimum 2GB RAM
- 500MB free disk space

## License

This project is licensed under the Apache License 2.0. See the [LICENSE](LICENSE) file for complete details.

See [NOTICE](NOTICE) file for complete LLVM licensing information.

## Credits and Attribution

This project is built upon and uses components from:

### LLVM Project

XClang is built on top of the **[LLVM Project](https://llvm.org/)**, a collection of modular and reusable compiler and toolchain technologies.

- **Website**: https://llvm.org/
- **Repository**: https://github.com/llvm/llvm-project
- **License**: Apache License 2.0 with LLVM Exceptions
- **Copyright**: University of Illinois at Urbana-Champaign and LLVM contributors

### Clang

**[Clang](https://clang.llvm.org/)** is a C language family frontend for LLVM supporting C, C++, Objective-C, and Objective-C++.

- **Website**: https://clang.llvm.org/
- **Documentation**: https://clang.llvm.org/docs/

### Acknowledgments

Special thanks to:
- The LLVM Team and all contributors who have developed this outstanding compiler infrastructure
- University of Illinois at Urbana-Champaign for the initial LLVM development
- The open source community that continues to contribute to the LLVM ecosystem

## Documentation

- [LLVM Documentation](https://llvm.org/docs/)
- [Clang Documentation](https://clang.llvm.org/docs/)
- [LLVM Language Reference](https://llvm.org/docs/LangRef.html)

## Contributing

This is a binaries-only public repository. If you encounter issues with the binaries or have suggestions:

1. Open an issue in this repository describing the problem
2. For build-related contributions, please contact the maintainers

Note: The build process is maintained separately and is not part of this public repository.

## Contact & Support

For questions, bug reports, or support:
- Open an issue in this repository
- Visit [LLVM Community](https://llvm.org/docs/#community) for LLVM support

## Disclaimer

This project is a binary distribution built from the LLVM Project. We do not claim ownership of the LLVM/Clang source code. All credit for the core compiler functionality goes to the LLVM team and its contributors.

## Version Information

- Based on XClang LLVM custom build
- Optimized for Android development
- Complete header files for C/C++ development

---

**Created by**: Xtra Manager Software Community  
**Based on**: LLVM Project (https://llvm.org/)  
**License**: Apache License 2.0  
**Year**: 2026

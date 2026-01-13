# FPDev Bootstrap Compilers

Bootstrap compilers for building FPC from source.

## Overview

This repository provides minimal FPC compilers needed to bootstrap (compile) newer FPC versions from source code.

## Available Versions

| Version | Linux x86_64 | Windows x86_64 | macOS x86_64 | macOS ARM64 |
|---------|--------------|----------------|--------------|-------------|
| 3.3.1   | Yes          | -              | -            | -           |
| 3.2.2   | -            | -              | -            | -           |
| 3.2.0   | -            | -              | -            | -           |

## Package Contents

Each bootstrap package contains only the minimal compiler executable:

```
bootstrap-{version}-{platform}/
└── bin/
    └── ppcx64       # or ppcx64.exe on Windows
```

## Usage

fpdev automatically downloads and uses bootstrap compilers when building FPC from source:

```bash
# Build FPC from source (bootstrap is downloaded automatically)
fpdev fpc install main --from-source
```

## Mirrors

- **GitHub**: https://github.com/dtamade/fpdev-bootstrap
- **Gitee**: https://gitee.com/dtamade/fpdev-bootstrap (China)

## License

MIT

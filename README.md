# Scoop-xPack

[![Tests](https://github.com/kanami09/Scoop-xPack/actions/workflows/ci.yml/badge.svg)](https://github.com/kanami09/Scoop-xPack/actions/workflows/ci.yml)

[中文](README.zh-CN.md)

An unofficial [Scoop](https://scoop.sh) bucket for [xPack Dev Tools](https://xpack-dev-tools.github.io) on Windows.

[xPack Dev Tools](https://xpack-dev-tools.github.io) provides pre-built binary distributions of various development tools (GCC toolchains, LLVM clang, OpenOCD, etc.). This bucket packages them as Scoop manifests for easy installation and management on Windows.

## Available Packages

| Manifest                      | Description                      | Notes                                    |
|-------------------------------|----------------------------------|------------------------------------------|
| `xpack-arm-none-eabi-gcc`     | Arm Embedded GCC toolchain       |                                          |
| `xpack-arm-none-eabi-gcc-x86` | Arm Embedded GCC toolchain (x86) | Last version with Windows 32-bit support |
| `xpack-aarch64-none-elf-gcc`  | AArch64 Embedded GCC toolchain   |                                          |
| `xpack-riscv-none-elf-gcc`    | RISC-V Embedded GCC toolchain    |                                          |
| `xpack-clang`                 | LLVM clang toolchain             |                                          |
| `xpack-clang-x86`             | LLVM clang toolchain (x86)       | Last version with Windows 32-bit support |
| `xpack-gcc`                   | GNU GCC compiler                 |                                          |
| `xpack-gcc-x86`               | GNU GCC compiler (x86)           | Last version with Windows 32-bit support |
| `xpack-cmake`                 | CMake build tool                 |                                          |
| `xpack-cmake-x86`             | CMake build tool (x86)           | Last version with Windows 32-bit support |
| `xpack-ninja`                 | Ninja build tool                 |                                          |
| `xpack-ninja-x86`             | Ninja build tool (x86)           | Last version with Windows 32-bit support |
| `xpack-openocd`               | OpenOCD on-chip debugger         |                                          |
| `xpack-openocd-x86`           | OpenOCD on-chip debugger (x86)   | Last version with Windows 32-bit support |

## Usage

### Prerequisites

This project is a **Scoop** bucket. You need to install Scoop first.<br>
For most users, run the following two PowerShell commands:

```pwsh
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression
```

If the installation fails, refer to the [Scoop official installation guide](https://github.com/ScoopInstaller/Install#readme).

### Add this bucket

```txt
scoop bucket add xpack https://github.com/kanami09/Scoop-xPack
```

### Remove this bucket

```txt
scoop bucket rm xpack
```

### Install a package

```txt
scoop install xpack/<app-name>
```

### Update a package

```txt
scoop update xpack/<app-name>
```

### Uninstall a package

```txt
scoop uninstall <app-name>
```

## Notes

- All packages are sourced from official [GitHub Releases](https://github.com/xpack-dev-tools).
- This is an unofficial, community-maintained Scoop bucket and is not affiliated with the xPack project.

## Related Links

- [xPack Dev Tools](https://xpack-dev-tools.github.io/)
- [Scoop](https://scoop.sh)
- [Scoop App Manifests Wiki](https://github.com/ScoopInstaller/Scoop/wiki/App-Manifests)

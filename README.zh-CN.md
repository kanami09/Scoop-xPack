# Scoop-xPack

[![Tests](https://github.com/kanami09/Scoop-xPack/actions/workflows/ci.yml/badge.svg)](https://github.com/kanami09/Scoop-xPack/actions/workflows/ci.yml)

[English](README.md)

本仓库为 [xPack Dev Tools](https://xpack-dev-tools.github.io) 提供的 [Scoop](https://scoop.sh) 第三方 bucket。

[xPack Dev Tools](https://xpack-dev-tools.github.io) 提供了一系列预编译的开发工具（如：GCC 工具链、LLVM、OpenOCD 等）的二进制发行版。

## 可用软件包

| 名称                          | 说明                        | 备注                                      |
|------------------------------ | --------------------------- | ----------------------------------------- |
| `xpack-arm-none-eabi-gcc`     | Arm 嵌入式 GCC 工具链       |                                           |
| `xpack-arm-none-eabi-gcc-x86` | Arm 嵌入式 GCC 工具链 (x86) | 此版本是最后一个支持 Windows-32bit 的版本 |
| `xpack-aarch64-none-elf-gcc`  | AArch64 嵌入式 GCC 工具链   |                                           |
| `xpack-riscv-none-elf-gcc`    | RISC-V 嵌入式 GCC 工具链    |                                           |
| `xpack-clang`                 | LLVM clang 工具链           |                                           |
| `xpack-clang-x86`             | LLVM clang 工具链 (x86)     | 此版本是最后一个支持 Windows-32bit 的版本 |
| `xpack-gcc`                   | GNU GCC 编译器              |                                           |
| `xpack-gcc-x86`               | GNU GCC 编译器 (x86)        | 此版本是最后一个支持 Windows-32bit 的版本 |

## 使用方法

### 先决条件

本项目是包管理器 **Scoop** 的 bucket，使用之前需要先安装 Scoop。<br>
对于一般用户，执行以下两行 PowerShell 脚本即可完成安装：

```pwsh
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression
```

若安装失败，请参阅 [Scoop 官方安装文档](https://github.com/ScoopInstaller/Install#readme)。

### 添加此 bucket

```txt
scoop bucket add xpack https://github.com/kanami09/Scoop-xPack
```

### 移除此 bucket

```txt
scoop bucket rm xpack
```

### 安装软件包

```txt
scoop install xpack/<app-name>
```

### 更新软件包

```txt
scoop update xpack/<app-name>
```

### 卸载软件包

```txt
scoop uninstall <app-name>
```

## 注意事项

- 所有软件包均来源于官方的 [GitHub Releases](https://github.com/xpack-dev-tools)。
- 本 bucket 为非官方的社区维护项目，与 xPack 项目无隶属关系。

## 相关链接

- [xPack Dev Tools](https://xpack-dev-tools.github.io/)
- [Scoop](https://scoop.sh)
- [Scoop App Manifests 文档](https://github.com/ScoopInstaller/Scoop/wiki/App-Manifests)

<div align="center">
  <h1>
    <img src="src/pack.png" width="256" alt="Icon"/><br/>
    Jappa Bedrock 🕳️<br/>
    <img src="https://img.shields.io/badge/Versions-1.6.1_--_26.1.2-purple?style=for-the-badge" alt="Versions 1.6.1 - 26.1.2">
    <img src="https://img.shields.io/badge/Edition-Java-orange?style=for-the-badge" alt="Java Edition"><br/>
    <a href="https://modrinth.com/resourcepack/jappa-bedrock">
      <img src="https://img.shields.io/badge/Available_on-Modrinth-00AF5C?style=for-the-badge&logo=modrinth" alt="Available on Modrinth"></img>
    </a>
  </h1>
</div>

**A Minecraft Java Edition resource pack** that reimagines the Bedrock texture from scratch. Instead of updating or modifying the original texture, this pack presents Bedrock exactly as Jappa would have designed it on a blank canvas, fully embracing the clean, modern aesthetic of contemporary Minecraft.

## 🔍 Overview

![Screenshot](assets/screenshot.png)

## 🔗 Dependencies

This repository uses [Nix](https://nixos.org) to provide a consistent development environment via `nix-shell` with all the necessary tools.

> [!WARNING]
> Nix is natively supported only on Unix-like operating systems (Linux and macOS). Windows users can use it via WSL2 (Windows Subsystem for Linux).

### ✍️ Manual Installation (Alternative)
If you prefer not to use Nix, or if you are on a system that doesn't support it, you can install all the required tools manually. You will need:

* [GNU Make](https://ftp.gnu.org/gnu/make/) – For automating the packaging process.
* [minizip-ng](https://github.com/zlib-ng/minizip-ng) – For packaging of zip archives.
* [yq](https://github.com/mikefarah/yq) – For parsing TOML.

## 🛠️ Packaging

> [!TIP]
> 📁 [`src/`](src/) – Contains the source files of the pack.
>
> 📦 [`packs/`](packs/) – Contains final, ready-to-use packs.

1. **Enter the Nix environment:**
   Open your terminal in the root directory of the repository and run:
   ```bash
   nix-shell
   ```
   *This will automatically download and install all necessary tools.*

2. **Build the pack:**
   Inside the Nix shell, run the following command to package:
   ```bash
   make
   ```

## 💝 Acknowledgements

* This repository is generated from the [mc-pack-env](https://github.com/segabass65/mc-pack-env) template.

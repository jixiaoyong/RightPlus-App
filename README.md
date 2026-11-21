# Right+ (RightPlus App)

<p align="center">
  <img src="assets/logo.svg" width="96" height="96" alt="Right+ Logo">
</p>

<p align="center">
  <b>Lightweight, native, and efficient Finder context menu enhancement for macOS.</b>
</p>

<p align="center">
  <a href="README_zh.md">简体中文</a> | <b>English</b>
</p>

<p align="center">
  <a href="https://github.com/jixiaoyong/RightPlus-App/releases/latest"><img src="https://img.shields.io/github/v/release/jixiaoyong/RightPlus-App?color=blue&label=Latest%20Release" alt="Latest Release"></a>
  <img src="https://img.shields.io/badge/Platform-macOS%2014.0%2B-lightgrey" alt="macOS 14.0+">
  <img src="https://img.shields.io/badge/Arch-Apple%20Silicon%20%7C%20Intel-success" alt="Architecture">
  <img src="https://img.shields.io/badge/License-MIT-orange" alt="License">
</p>

---

## Overview

**Right+** is a minimalist and high-performance macOS Finder context menu extension built natively with Swift and Apple's `FIFinderSync` framework. It requires no heavy background services and maintains a negligible memory footprint.

### Key Highlights

- **Quick File Creation**: Create common file types instantly in any folder, including Markdown (`.md`), Word (`.docx`), Excel (`.xlsx`), PowerPoint (`.pptx`), Plain Text (`.txt`), Shell Script (`.sh`), and Python (`.py`). Automatically handles filename collision with incremented numbering.
- **Application Shortcuts**: Pin your high-frequency tools (VS Code, Sublime Text, Typora, Xcode, etc.) to the context menu, complete with real-time app search and category filtering.
- **Copy Path / Filename with Multi-Screen HUD**: Copy POSIX paths or filenames with one click. Displays a floating ultra-thin material HUD capsule at the bottom of the active monitor with smart path truncation and subtle audio feedback.
- **Direct Terminal Access**: Open the current directory directly in Terminal or iTerm2.
- **Native Dual-Architecture Optimization**: Standalone packages optimized for Apple Silicon (M-series) and Intel architectures. In-memory caching and asynchronous icon pre-warming eliminate context menu latency.
- **100% Offline & Private**: Zero network telemetry. All settings and caches remain strictly on your local machine.

---

## Download & Installation

### 1. Download

Visit [GitHub Releases](https://github.com/jixiaoyong/RightPlus-App/releases/latest) to download the package corresponding to your Mac:
- **Apple Silicon (M1/M2/M3/M4)**: Download `RightPlus-0.1.0-arm64.zip`
- **Intel Processors**: Download `RightPlus-0.1.0-x86_64.zip`

### 2. Installation Steps

1. Extract the downloaded `.zip` file to obtain `RightPlus.app`.
2. Move `RightPlus.app` into your `/Applications` folder.
3. **Bypass Gatekeeper (First Launch Only)**:
   Because this release is ad-hoc signed, if macOS displays a warning ("cannot verify developer" or "app is damaged"), run the following command once in **Terminal**:
   ```bash
   xattr -cr /Applications/RightPlus.app
   ```
4. **Enable Finder Extension**:
   - Launch `RightPlus.app`.
   - Open macOS **System Settings -> Privacy & Security -> Extensions -> Added extensions (or Finder Extensions)**.
   - Check the toggle for **Right+**.
   - If the menu items do not appear immediately, refresh Finder cache by running `killall Finder` in Terminal.

---

## Official Website

- Live Site: [https://jixiaoyong.github.io/RightPlus-App/](https://jixiaoyong.github.io/RightPlus-App/)

---

## Feedback & Issues

If you encounter any issues or have feature requests, please submit an issue on [GitHub Issues](https://github.com/jixiaoyong/RightPlus-App/issues).

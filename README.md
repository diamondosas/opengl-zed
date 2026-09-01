# Zed - OpenGL Fork

[![Zed](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/zed-industries/zed/main/assets/badge/v0.json)](https://zed.dev)
[![CI](https://github.com/zed-industries/zed/actions/workflows/run_tests.yml/badge.svg)](https://github.com/zed-industries/zed/actions/workflows/run_tests.yml)

## What is this?

This is a custom fork of [Zed](https://zed.dev), a modern code editor, that replaces the default Vulkan rendering backend with **OpenGL** for Linux and macOS.

> **⚠️ This fork is designed for older GPUs that don't support Vulkan.** If you need Zed on hardware with limited graphics support, this is for you.

---

## Why OpenGL?

### The Problem
The official Zed editor uses **Vulkan** for rendering, which requires modern GPUs. This leaves users with older hardware out in the cold:
- Older integrated graphics (Intel HD 4000, etc.)
- Legacy gaming GPUs
- Virtualized environments with limited graphics support

### The Solution
This fork uses **OpenGL** instead, which has much broader hardware support while maintaining excellent performance and visual quality.

---

## Who Should Use This?

✅ You have **older or integrated graphics** that don't support Vulkan  
✅ You're running Zed on a **virtual machine** with limited GPU support  
✅ You want to use Zed but were told your hardware is "too old"  

❌ Your hardware already supports Vulkan (use official Zed instead)

---

## Getting Started

### Installation

For now, you'll need to build from source:

```bash
git clone https://github.com/diamondosas/opengl-zed.git
cd opengl-zed
cargo build --release
```

The compiled binary will be in `target/release/zed`.

### Supported Platforms

- **Linux** (with OpenGL support)
- **macOS** (with OpenGL support)

---

## How This Fork Works

Instead of using Vulkan (which requires newer driver support), this fork leverages OpenGL for rendering. OpenGL has been around for decades and works on virtually any GPU made in the last 15+ years.

### Performance

You can expect performance comparable to the official Zed on compatible hardware. OpenGL is a mature API with excellent driver support across platforms.

---

## Features

All Zed features are included:
- Fast, responsive code editing
- Multi-line editing and collaborative features
- Language server protocol (LSP) support
- Built-in terminal
- Keyboard-centric workflow
- Theme support

---

## Compatibility

This fork aims to track the upstream [Zed repository](https://github.com/zed-industries/zed) as closely as possible. Updates and improvements from official Zed releases are regularly merged in.

---

## Contributing

Found a bug specific to the OpenGL backend? Have improvements? Contributions are welcome!

Please note: This is a community fork. For issues specific to Zed itself, check the [official repository](https://github.com/zed-industries/zed).

---

## License

This fork maintains the same license as the official Zed project.

---

## Resources

- 🔗 [Official Zed Documentation](https://zed.dev/docs)
- 🐙 [Official Zed Repository](https://github.com/zed-industries/zed)
- 💬 [Zed Community Discord](https://discord.gg/qSDq23cM86)

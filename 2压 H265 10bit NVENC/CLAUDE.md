# H.265 10-bit NVIDIA NVENC GPU Encoding

## Overview

This folder contains H.265/HEVC encoding presets using NVIDIA GPU acceleration (NVENC) with 10-bit color depth. Provides fast GPU-accelerated encoding with modern codec and superior color handling.

## Use Cases

- Fast H.265 encoding on NVIDIA GPU hardware
- Content requiring superior color depth support
- Modern device streaming and distribution
- High-quality archival with hardware acceleration

## Encoding Characteristics

- **Codec**: H.265/HEVC (hevc_nvenc)
- **Bit Depth**: 10-bit
- **Quality Level**: CQ 23 (NVENC quality metric)
- **Preset Speed**: hq (high quality)
- **Profile**: main10
- **Audio Codec**: copy (stream passthrough)
- **Container Format**: MP4 with faststart

## Special Features

- **GPU Acceleration**: NVIDIA NVENC for hardware-accelerated encoding
- **10-bit Color Depth**: Superior color information preservation
- **Main10 Profile**: Professional-grade H.265 support
- **High Quality Focus**: hq preset for optimal quality

## Recommended For

- NVIDIA GPU systems with NVENC capability
- Modern devices that support H.265
- Professional streaming platforms
- High-quality distribution with color depth needs

## Notes

- Requires NVIDIA GPU with HEVC NVENC support (GTX 950 or newer, RTX series)
- Significantly faster than CPU-based x265
- CQ 23 with 10-bit profile provides excellent quality
- Audio passed through to preserve original quality

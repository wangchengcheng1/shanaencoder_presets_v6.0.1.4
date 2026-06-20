# H.265 10-Bit Intel QSV Encoding Presets

## Overview

This folder contains H.265/HEVC video encoding presets using Intel Quick Sync Video (QSV) GPU acceleration with 10-bit encoding depth. These presets provide hardware-accelerated H.265 encoding on Intel systems.

## Use Cases

- Intel GPU-accelerated H.265 encoding
- Systems with Intel integrated graphics
- Fast H.265 encoding on Intel platforms
- Modern codec efficiency with Intel hardware
- Power-efficient encoding (integrated GPU)

## Encoding Characteristics

- **Codec**: H.265/HEVC
- **Bit Depth**: 10-bit
- **Acceleration**: Intel Quick Sync Video (QSV)
- **Speed**: Very fast hardware-accelerated encoding
- **Compatibility**: Modern H.265-capable devices
- **Audio Codec**: AAC (libfdk_aac)

## Hardware Requirements

- Intel processor with QSV support:
  - 6th Gen Core and newer (Skylake+)
  - Intel Arc A-series discrete GPUs
  - Some mobile/laptop processors

## Benefits

- **Speed**: Fast hardware-accelerated H.265 encoding
- **Efficiency**: Offloads to GPU (Intel UHD/Iris graphics)
- **Power**: Lower power consumption than CPU encoding
- **Compression**: 50% better than H.264
- **Quality**: 10-bit for superior color representation

## Performance Profile

- Encoding speed: Very fast (hardware accelerated)
- Quality level: High (good H.265 compression)
- File size: ~50% smaller than H.264 equivalent
- Power usage: Low (GPU acceleration efficient)

## Intel GPU Support

- Integrated Intel HD/UHD Graphics
- Intel Iris Pro Graphics
- Intel Arc discrete GPUs (newer)
- Laptop integrated graphics

## When to Use

- Intel-based systems (laptops, desktops, servers)
- Power-efficient encoding workflows
- Systems without NVIDIA GPU
- Modern device compatibility requirements
- Real-time or batch encoding on Intel hardware

## Compatibility Notes

- Works on Intel 6th Gen and newer
- Some older mobile processors may have limited support
- Laptop battery efficiency benefit (uses integrated GPU)
- Suitable for both consumer and professional Intel platforms

## Performance Notes

- Multi-threaded support for efficiency
- Excellent for laptop battery life
- Suitable for 24/7 server encoding
- Good balance of speed and quality

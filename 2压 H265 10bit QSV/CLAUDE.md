# H.265 10-bit Intel Quick Sync Video (QSV) Encoding

## Overview

This folder contains H.265/HEVC encoding presets using Intel Quick Sync Video (QSV) GPU acceleration. Provides fast encoding on Intel systems with integrated or discrete Intel GPUs.

## Use Cases

- H.265 encoding on Intel GPU-equipped systems
- Quick video encoding with Intel QSV hardware
- Content distribution on Intel-based platforms
- Fast encoding without NVIDIA GPU requirements

## Encoding Characteristics

- **Codec**: H.265/HEVC (hevc_qsv)
- **Bit Depth**: 10-bit
- **Quality Level**: Variable bitrate mode (1064k target, 2240k max)
- **Preset Speed**: veryfast
- **Audio Codec**: copy (stream passthrough)
- **Container Format**: MP4 with faststart

## Special Features

- **Intel QSV Acceleration**: Hardware acceleration on Intel GPUs
- **Bitrate Limiting**: Smart bitrate constraints for file size control
- **10-bit Profile**: Main profile H.265 support
- **Fast Processing**: Hardware-accelerated encoding speed

## Recommended For

- Intel systems with QSV capability (6th gen Core and newer)
- Cost-effective GPU acceleration on Intel platforms
- H.265 encoding without NVIDIA dependencies
- Modern Intel-based systems needing video encoding

## Notes

- Requires Intel system with Quick Sync Video support
- Much faster than CPU-based encoding
- Bitrate constraints (1064k target, 2240k max) ensure predictable file sizes
- Good alternative for Intel systems without NVIDIA GPU

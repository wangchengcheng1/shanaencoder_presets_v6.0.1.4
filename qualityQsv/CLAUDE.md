# Intel Quick Sync Video (QSV) Quality Presets

## Overview

This folder contains H.265/HEVC quality presets using Intel Quick Sync Video (QSV) GPU acceleration. Provides efficient GPU-accelerated encoding on Intel systems with reasonable processing speeds.

## Use Cases

- Quality encoding on Intel GPU systems
- Fast encoding with Intel QSV acceleration
- H.265 encoding without NVIDIA GPU dependencies
- Modern Intel platform optimization

## Encoding Characteristics

- **Codec**: H.265/HEVC (hevc_qsv)
- **Bit Depth**: 10-bit
- **Quality Level**: 23 (Intel QSV quality metric)
- **Preset Speed**: veryfast
- **Profile**: main
- **Audio Codec**: libfdk_aac at 192k
- **Container Format**: MP4

## Special Features

- **Intel QSV Acceleration**: GPU-accelerated on Intel platforms
- **10-bit Support**: Main profile H.265 with color depth
- **Fast Processing**: veryfast preset for quick encoding
- **AAC Audio**: Quality audio codec at 192k

## Recommended For

- Intel systems with Quick Sync Video support
- Cost-effective GPU acceleration on Intel platforms
- H.265 encoding without NVIDIA dependencies
- Modern Intel-based video workflows

## Notes

- Requires Intel system with QSV support (6th gen Core and newer)
- Significantly faster than CPU-based encoding
- Quality level 23 provides good balance
- Good alternative for Intel systems without NVIDIA GPU

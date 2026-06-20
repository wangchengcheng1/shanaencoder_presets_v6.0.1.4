# H.264 8-bit x264 CPU Encoding

## Overview

This folder contains H.264 encoding presets using x264 software encoder. Designed for H.264 compatibility with CPU-based processing, suitable for systems without GPU acceleration or when H.264 is required.

## Use Cases

- H.264 encoding on CPU-based systems
- Content requiring H.264 codec for compatibility
- Archival with older codec standards
- Streaming to devices that require H.264 support

## Encoding Characteristics

- **Codec**: H.264/AVC (libx264)
- **Bit Depth**: 8-bit
- **Quality Level**: CRF 19.0
- **Preset Speed**: veryfast
- **Audio Codec**: copy (stream passthrough)
- **Container Format**: MP4 with faststart

## Special Features

- **SSIM Tuning**: Optimized for perceptual quality using SSIM metrics
- **Enhanced Filtering**: Unsharp and deblock filters for visual improvement
- **CPU-Based**: Works on any system with CPU (no GPU required)
- **Compatibility**: H.264 codec for universal device support

## Recommended For

- Systems without GPU acceleration
- Content requiring H.264 codec
- Compatibility with older devices and platforms
- CPU-only encoding workflows

## Notes

- CRF 19.0 provides good quality with veryfast preset
- Slower than NVENC but works on any system
- H.264 codec ensures compatibility with older devices
- SSIM-tuned parameters optimize for perceived quality

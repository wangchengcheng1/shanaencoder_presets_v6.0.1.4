# H.264 8-bit NVIDIA NVENC GPU Encoding

## Overview

This folder contains H.264 encoding presets using NVIDIA GPU acceleration (NVENC). Provides fast encoding leveraging GPU hardware while maintaining compatibility with older devices that require H.264.

## Use Cases

- Fast video encoding on NVIDIA GPU hardware
- Content requiring H.264 codec for compatibility
- Real-time or near-real-time encoding workflows
- Archival with hardware acceleration capabilities

## Encoding Characteristics

- **Codec**: H.264/AVC (h264_nvenc)
- **Bit Depth**: 8-bit
- **Quality Level**: CQ 23 (NVENC quality metric)
- **Preset Speed**: hq (high quality)
- **Audio Codec**: copy (stream passthrough)
- **Container Format**: MP4 with faststart

## Special Features

- **GPU Acceleration**: NVIDIA NVENC for fast hardware encoding
- **Video Enhancement**: Unsharp and deblock filters for improved visual quality
- **Compatibility**: H.264 codec for universal device support
- **Quality Focus**: High-quality NVENC preset

## Recommended For

- NVIDIA GPU systems with NVENC capability
- Content requiring H.264 compatibility
- Fast encoding workflows on compatible hardware
- Streaming to devices that require H.264

## Notes

- Requires NVIDIA GPU with NVENC support (GTX 950 or newer, RTX series)
- Much faster than CPU-based encoding
- CQ 23 provides good quality with hardware acceleration
- Audio is passed through unchanged to minimize processing

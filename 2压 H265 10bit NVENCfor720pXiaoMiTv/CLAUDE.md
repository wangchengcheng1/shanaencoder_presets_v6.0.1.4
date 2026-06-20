# H.265 10-bit NVIDIA NVENC 720p Xiaomi TV Optimization

## Overview

This folder contains H.265/HEVC presets specifically optimized for Xiaomi Smart TV playback at 720p resolution. Uses NVIDIA NVENC GPU acceleration with resolution scaling and audio optimization for Xiaomi TV compatibility.

## Use Cases

- Encoding content specifically for Xiaomi Smart TVs
- 720p streaming to Xiaomi TV devices
- Optimized playback on Xiaomi TV hardware
- Budget-conscious encoding with TV compatibility

## Encoding Characteristics

- **Codec**: H.265/HEVC (hevc_nvenc)
- **Bit Depth**: 10-bit
- **Quality Level**: CQ 23
- **Preset Speed**: hq (high quality)
- **Resolution**: 720p (1280x720) with scale/pad filters
- **Audio Codec**: libmp3lame at 128k (2 channels)
- **Container Format**: MP4 with faststart

## Special Features

- **Xiaomi Optimization**: Tuned scaling and padding for TV playback
- **720p Resolution**: Optimized for HD TV display
- **Scale Filters**: Bicubic scaling with auto-padding for aspect ratio preservation
- **MP3 Audio**: Reduced audio bitrate (128k) for TV compatibility
- **GPU Acceleration**: NVIDIA NVENC processing

## Recommended For

- Streaming to Xiaomi Smart TVs
- 720p content distribution for TV playback
- Optimized Xiaomi TV device compatibility
- Budget-conscious encoding with quality

## Notes

- 720p resolution optimized for standard HD TV displays
- Audio downsampled to 128k MP3 for compatibility and file size
- Scale/pad filters ensure proper aspect ratio on various TV models
- GPU acceleration provides fast processing

# NVIDIA GPU Quality Transcoding to 720p

## Overview

This folder contains NVIDIA GPU-accelerated H.265 presets that scale video to 720p resolution. Provides fast 720p transcoding using NVENC with focus on quality and efficiency.

## Use Cases

- Fast 720p transcoding on NVIDIA systems
- Downscaling high-resolution content to 720p
- Mobile and streaming optimization to 720p
- Quick GPU-accelerated 720p encoding

## Encoding Characteristics

- **Codec**: H.265/HEVC (hevc_nvenc)
- **Bit Depth**: 10-bit
- **Quality Level**: CQ 23
- **Preset Speed**: hq (high quality)
- **Resolution**: 720p (1280x720) with scaling filters
- **Profile**: main10
- **Audio Codec**: libfdk_aac at 192k
- **Container Format**: MP4

## Special Features

- **GPU Acceleration**: NVIDIA NVENC for fast processing
- **720p Scaling**: Optimized downscaling to HD format
- **Scaling Filters**: Quality-focused resolution conversion
- **High Quality Preset**: hq with main10 profile
- **AAC Audio**: Quality audio codec at 192k

## Recommended For

- NVIDIA GPU systems requiring 720p output
- Mobile and streaming distribution at 720p
- Fast 720p transcoding workflows
- Bandwidth-optimized streaming

## Notes

- Requires NVIDIA GPU with HEVC NVENC support
- Significantly faster than CPU-based 720p transcoding
- CQ 23 provides good quality at 720p resolution
- Good balance between quality and file size

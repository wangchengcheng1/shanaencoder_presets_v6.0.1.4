# NVIDIA GPU Quality Transcoding to 1080p

## Overview

This folder contains NVIDIA GPU-accelerated H.265 presets that scale video to 1080p resolution. Provides fast 1080p transcoding using NVENC hardware acceleration with quality focus.

## Use Cases

- Fast 1080p transcoding on NVIDIA systems
- Standardizing mixed resolutions to 1080p
- GPU-accelerated resolution normalization
- Quick quality 1080p encoding

## Encoding Characteristics

- **Codec**: H.265/HEVC (hevc_nvenc)
- **Bit Depth**: 10-bit
- **Quality Level**: CQ 23
- **Preset Speed**: hq (high quality)
- **Resolution**: 1080p (1920x1080) with bicubic scaling/padding
- **Profile**: main10
- **Audio Codec**: libfdk_aac at 192k
- **Container Format**: MP4

## Special Features

- **GPU Acceleration**: NVIDIA NVENC for fast encoding
- **1080p Scaling**: Bicubic scaling to 1080p resolution
- **Auto Padding**: Maintains aspect ratio during scaling
- **High Quality**: hq preset with main10 profile
- **AAC Audio**: Quality audio encoding at 192k

## Recommended For

- NVIDIA GPU systems requiring 1080p output
- Fast 1080p transcoding workflows
- Standardizing video to 1080p resolution
- Streaming to 1080p targets

## Notes

- Requires NVIDIA GPU with HEVC NVENC support
- Much faster than CPU-based 1080p transcoding
- CQ 23 with hq preset provides excellent quality
- Bicubic scaling ensures good visual quality

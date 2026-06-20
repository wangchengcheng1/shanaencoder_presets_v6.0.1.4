# NVIDIA GPU Quality Transcoding to 1080p with Audio Passthrough

## Overview

This folder contains NVIDIA GPU-accelerated H.265 presets that scale video to 1080p while preserving original audio. Combines GPU speed with 1080p standardization and audio preservation.

## Use Cases

- Fast 1080p transcoding on NVIDIA systems with audio preservation
- Standardizing mixed resolutions to 1080p with original audio
- Professional workflows requiring audio integrity
- GPU-accelerated 1080p normalization

## Encoding Characteristics

- **Codec**: H.265/HEVC (hevc_nvenc)
- **Bit Depth**: 10-bit
- **Quality Level**: CQ 23
- **Preset Speed**: hq (high quality)
- **Resolution**: 1080p (1920x1080) with scaling/padding
- **Profile**: main10
- **Audio Codec**: copy (stream passthrough)
- **Container Format**: MP4

## Special Features

- **GPU Acceleration**: NVIDIA NVENC for fast processing
- **1080p Scaling**: Bicubic scaling to consistent resolution
- **Audio Preservation**: Original audio passed through unchanged
- **Auto Padding**: Maintains aspect ratio during scaling
- **High Quality**: hq preset with main10 profile

## Recommended For

- NVIDIA GPU systems requiring 1080p output
- Professional workflows with audio preservation needs
- Fast 1080p transcoding with quality focus
- Streaming to 1080p targets with original audio

## Notes

- Requires NVIDIA GPU with HEVC NVENC support
- Significantly faster than CPU-based 1080p transcoding
- Scaling/padding filters maintain aspect ratio
- Audio passthrough ensures original quality preservation

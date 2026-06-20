# CPU-Based Quality Transcoding to 1080p

## Overview

This folder contains CPU-based H.265 encoding presets that scale video to 1080p resolution while maintaining quality. Designed for upscaling or downscaling content to a consistent 1080p target.

## Use Cases

- Standardizing video to 1080p resolution
- Upscaling lower resolution content
- Downscaling higher resolution content to 1080p
- Creating consistent 1080p output from mixed source resolutions

## Encoding Characteristics

- **Codec**: H.265/HEVC (libx265)
- **Bit Depth**: 10-bit
- **Quality Level**: CRF 21.0
- **Preset Speed**: veryfast
- **Resolution**: 1080p (1920x1080) with bicubic scaling
- **Audio Codec**: libfdk_aac at 192k
- **Container Format**: MP4

## Special Features

- **Bicubic Scaling**: High-quality scaling algorithm
- **Auto Padding**: Maintains aspect ratio with padding as needed
- **Quality Focus**: CRF 21.0 for good quality
- **CPU-Based Processing**: Works on any system

## Recommended For

- Standardizing video resolution to 1080p
- Content requiring 1080p output format
- Scaling mixed-resolution sources to consistent output
- Workflows where 1080p is the target format

## Notes

- Bicubic scaling provides good quality for scaling operations
- Auto padding maintains original aspect ratio
- CRF 21.0 provides good quality at 1080p
- Audio is re-encoded to AAC at 192k

# CPU-Based Quality Transcoding to 720p

## Overview

This folder contains CPU-based H.265 encoding presets that scale video to 720p resolution. Designed for downscaling high-resolution content or standardizing sources to 720p HD format.

## Use Cases

- Standardizing video to 720p HD resolution
- Downscaling 1080p or higher resolution content
- Creating 720p distribution copies
- Mobile and streaming optimization to 720p

## Encoding Characteristics

- **Codec**: H.265/HEVC (libx265)
- **Bit Depth**: 10-bit
- **Quality Level**: CRF 21.0
- **Preset Speed**: veryfast
- **Resolution**: 720p (1280x720) with bicubic scaling
- **Audio Codec**: libfdk_aac at 192k
- **Container Format**: MP4

## Special Features

- **Bicubic Scaling**: High-quality downscaling algorithm
- **Auto Padding**: Maintains aspect ratio with padding
- **CPU-Based Processing**: Universal system compatibility
- **AAC Audio**: Quality audio encoding at 192k

## Recommended For

- Creating 720p copies from higher resolutions
- Mobile device optimization
- Streaming scenarios where 720p is standard
- Bandwidth-conscious distribution

## Notes

- Bicubic scaling provides good quality for downscaling
- Auto padding preserves original aspect ratio
- 720p is good compromise between quality and file size
- CRF 21.0 suitable for 720p quality expectations

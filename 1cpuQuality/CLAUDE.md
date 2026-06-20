# Standard CPU Quality Presets

## Overview

This folder contains standard quality CPU-based H.265 encoding presets. Provides a good balance of quality and performance suitable for general-purpose video encoding tasks.

## Use Cases

- Standard video encoding workflows
- General-purpose quality conversions
- Content distribution with good quality standards
- Default preset for most encoding scenarios

## Encoding Characteristics

- **Codec**: H.265/HEVC (libx265)
- **Bit Depth**: 10-bit
- **Quality Level**: CRF 20.0
- **Preset Speed**: veryfast
- **Audio Codec**: libfdk_aac at 192k
- **Container Format**: MP4 with faststart optimization

## Special Features

- **Veryfast Preset**: Quick encoding without compromising quality significantly
- **10-bit Support**: Preserves color depth for better visual fidelity
- **AAC Audio**: High-quality audio codec at 192k bitrate
- **Streaming Optimized**: faststart for efficient streaming playback

## Recommended For

- General video encoding tasks
- Batch processing with moderate time constraints
- Standard quality archival
- Content distribution platforms

## Notes

- Veryfast preset provides reasonable encoding speed while maintaining CRF 20.0 quality
- Represents a balanced middle ground for most use cases
- Good quality-to-performance ratio for diverse content types

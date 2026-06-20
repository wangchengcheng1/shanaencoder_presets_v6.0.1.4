# High Bitrate H.265 10-bit x265 Encoding

## Overview

This folder contains high-bitrate H.265/HEVC encoding presets using constant quantizer (CQP) mode. Designed for scenarios where maximum quality is essential and bitrate constraints are not primary concerns.

## Use Cases

- Professional video production with quality priority
- High-bitrate archival for maximum quality
- Studio environments where file size is not constrained
- Premium distribution requiring best possible quality

## Encoding Characteristics

- **Codec**: H.265/HEVC (libx265)
- **Bit Depth**: 10-bit
- **Quality Mode**: CQP 15 (constant quantizer - very high quality)
- **Preset Speed**: medium
- **Bitrate Limits**: 1064k target, 2240k max, 4480k buffer
- **Audio Codec**: copy (stream passthrough)
- **Container Format**: MP4 with faststart

## Special Features

- **Constant Quantizer (CQP)**: Maintains consistent quality regardless of scene complexity
- **High Bitrate**: Generous bitrate budget for best quality
- **Medium Preset**: Good balance of quality and processing time
- **Unsharp Filter**: Enhanced detail preservation
- **10-bit Profile**: Maximum color depth support

## Recommended For

- Professional video production
- High-quality archival
- Studio environments with no size constraints
- Premium quality distribution channels

## Notes

- CQP 15 maintains consistent quality across all frames
- Medium preset provides reasonable encoding speed
- High bitrate limits ensure no quality compromise
- Best used when file size is not a limiting factor

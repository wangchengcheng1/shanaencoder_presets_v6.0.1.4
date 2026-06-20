# Lower Quality H.265 10-bit x265 Encoding

## Overview

This folder contains lower-quality H.265/HEVC encoding presets with variable bitrate mode and aggressive constraints. Optimized for scenarios where file size reduction is prioritized while maintaining acceptable quality.

## Use Cases

- File size reduction while maintaining basic quality
- Archival with space constraints
- Distribution scenarios where smaller files are beneficial
- Content where highest quality is not essential

## Encoding Characteristics

- **Codec**: H.265/HEVC (libx265)
- **Bit Depth**: 10-bit
- **Quality Mode**: Variable bitrate (1064k target, 2240k max)
- **Preset Speed**: veryfast
- **Audio Codec**: copy (stream passthrough)
- **Container Format**: MP4 with faststart

## Special Features

- **Bitrate Constraints**: Targets smaller files with controlled quality
- **Variable Bitrate**: Adapts to content complexity within limits
- **Fast Processing**: veryfast preset for quick encoding
- **10-bit Support**: Maintains color depth despite lower quality
- **Unsharp Filter**: Compensates for quality reduction

## Recommended For

- File size reduction scenarios
- Archival with storage limitations
- Distribution where smaller files matter
- Content where lower quality is acceptable

## Notes

- Bitrate limits (1064k target, 2240k max) reduce file sizes significantly
- Still maintains 10-bit color depth for better quality than 8-bit alternatives
- Veryfast preset ensures quick processing
- Good compromise between size and quality

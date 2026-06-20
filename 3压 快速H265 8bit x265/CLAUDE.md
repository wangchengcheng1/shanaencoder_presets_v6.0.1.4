# Fast Lower Quality H.265 8-bit x265 Encoding

## Overview

This folder contains fast, lower-quality H.265/HEVC encoding presets with 8-bit color depth and aggressive bitrate constraints. Optimized for maximum file size reduction with quick encoding speed.

## Use Cases

- Aggressive file size reduction
- Quick encoding with minimum quality requirements
- Archival with tight storage constraints
- Distribution where very small files are needed

## Encoding Characteristics

- **Codec**: H.265/HEVC (libx265)
- **Bit Depth**: 8-bit
- **Quality Mode**: Variable bitrate (500k target, 1000k max, 2000k buffer)
- **Preset Speed**: veryfast
- **Audio Codec**: copy (stream passthrough)
- **Container Format**: MP4 with faststart

## Special Features

- **Aggressive Bitrate Constraints**: Very low bitrate targets for minimal files
- **8-bit Encoding**: Reduces color depth for further size reduction
- **Fast Processing**: veryfast preset for rapid encoding
- **PSNR Tuning**: Optimized for PSNR metrics despite lower quality
- **Deblock Filter**: Minimizes blocking artifacts

## Recommended For

- Maximum file size reduction needed
- Quick encoding with minimal quality
- Tight storage or bandwidth constraints
- Content where low quality is acceptable

## Notes

- Extremely aggressive bitrate constraints (500k target, 1000k max)
- 8-bit encoding reduces file size vs 10-bit variants
- Produces smallest possible files with acceptable playability
- Best for scenarios where size matters more than quality

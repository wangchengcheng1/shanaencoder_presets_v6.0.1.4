# CPU-Based Quality Transcoding to 720p with Audio Passthrough

## Overview

This folder contains CPU-based H.265 encoding presets that scale video to 720p while preserving the original audio stream. Optimized for 720p distribution without audio re-encoding.

## Use Cases

- Creating 720p copies with audio preservation
- Downscaling to 720p while maintaining original audio
- Professional workflows requiring audio integrity
- Mobile distribution with audio fidelity needs

## Encoding Characteristics

- **Codec**: H.265/HEVC (libx265)
- **Bit Depth**: 10-bit
- **Quality Level**: CRF 21.0
- **Preset Speed**: veryfast
- **Resolution**: 720p (1280x720) with bicubic scaling
- **Audio Codec**: copy (stream passthrough)
- **Container Format**: MP4

## Special Features

- **720p Scaling**: Optimized downscaling to HD format
- **Audio Preservation**: Original audio stream preserved unchanged
- **Bicubic Scaling**: Quality-focused scaling algorithm
- **Auto Padding**: Maintains aspect ratio during scaling

## Recommended For

- 720p distribution with original audio
- Mobile streaming with audio preservation
- Professional content requiring audio integrity
- Bandwidth-conscious workflows with audio focus

## Notes

- Bicubic scaling ensures good visual quality at 720p
- Audio passthrough reduces overall processing time
- Maintains original audio fidelity while optimizing video
- Good balance between quality and file size

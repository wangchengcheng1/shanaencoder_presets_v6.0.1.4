# CPU-Based Quality Transcoding to 1080p with Audio Passthrough

## Overview

This folder contains CPU-based H.265 encoding presets that scale video to 1080p while preserving the original audio stream. Ideal for workflows requiring 1080p video normalization without audio re-encoding.

## Use Cases

- Standardizing video to 1080p with audio preservation
- Scaling content while maintaining original audio quality
- Professional workflows requiring audio integrity
- Mixed resolution sources needing 1080p normalization

## Encoding Characteristics

- **Codec**: H.265/HEVC (libx265)
- **Bit Depth**: 10-bit
- **Quality Level**: CRF 21.0
- **Preset Speed**: veryfast
- **Resolution**: 1080p (1920x1080) with bicubic scaling
- **Audio Codec**: copy (stream passthrough)
- **Container Format**: MP4

## Special Features

- **Bicubic Scaling**: High-quality resolution scaling
- **Auto Padding**: Aspect ratio preservation with padding
- **Audio Preservation**: Original audio stream passed through unchanged
- **CPU-Based**: Universal system compatibility

## Recommended For

- 1080p standardization with audio preservation
- Professional workflows requiring original audio
- Content where audio quality must not be compromised
- Consistent 1080p output with audio integrity

## Notes

- Bicubic scaling maintains good quality during resolution changes
- Auto padding preserves original aspect ratio
- Audio is not re-encoded, preserving original quality
- Faster overall processing due to audio passthrough

# Medium CPU Quality Presets with Audio Passthrough

## Overview

This folder contains medium-speed CPU-based H.265 encoding presets with GPT 5.3 Codex optimization that preserve the original audio stream without re-encoding. Ideal for workflows where maintaining original audio quality is critical.

## Use Cases

- Content where audio must remain unchanged or uncompressed
- Archival with original audio preservation
- Workflows where audio re-encoding is not desired
- Professional video production requiring audio integrity

## Encoding Characteristics

- **Codec**: H.265/HEVC (libx265)
- **Bit Depth**: 10-bit
- **Quality Level**: CRF 20.0 (high quality)
- **Preset Speed**: medium
- **Audio Codec**: copy (stream passthrough - no re-encoding)
- **Container Format**: MP4 with faststart optimization

## Special Features

- **Audio Passthrough**: Original audio stream copied without transcoding
- **Lossless Audio Preservation**: No audio quality degradation
- **Video Quality Focus**: All encoding effort directed to video
- **GPT 5.3 Codex Optimization**: Intelligent video parameter tuning

## Recommended For

- Professional audio content that must not be modified
- Content with high-quality audio tracks
- Workflows where audio format preservation is mandatory
- Archival scenarios requiring bit-for-bit audio fidelity

## Notes

- Audio is passed through unchanged, preserving original codec and quality
- Reduces file size and processing time compared to re-encoding audio
- Ensures perfect audio fidelity while optimizing video encoding

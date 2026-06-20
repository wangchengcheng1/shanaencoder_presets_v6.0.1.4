# Fast CPU Quality with Audio Passthrough

## Overview

This folder contains fast CPU-based H.265 encoding presets that preserve the original audio stream. Optimized for quick encoding while maintaining original audio quality without re-encoding.

## Use Cases

- Fast encoding with audio preservation
- Content where quick processing is needed but audio quality must not be compromised
- Standard batch processing with audio integrity requirements
- Quick archival without audio transcoding

## Encoding Characteristics

- **Codec**: H.265/HEVC (libx265)
- **Bit Depth**: 10-bit
- **Quality Level**: CRF 20.0
- **Preset Speed**: fast
- **Audio Codec**: copy (stream passthrough)
- **Container Format**: MP4 with faststart optimization

## Special Features

- **Fast Encoding**: Prioritizes quick processing
- **Audio Preservation**: Original audio stream copied unchanged
- **Reduced Processing Time**: Less work required due to audio passthrough
- **Quality Maintained**: 10-bit video with CRF 20.0

## Recommended For

- Quick video conversions with audio integrity
- Batch processing where speed and audio quality matter equally
- Content distribution with specific audio requirements
- Fast re-encoding when audio must not be modified

## Notes

- Faster than medium preset while maintaining audio fidelity
- Reduced overall file size and processing time due to audio passthrough
- Good balance between speed and quality when audio preservation is needed

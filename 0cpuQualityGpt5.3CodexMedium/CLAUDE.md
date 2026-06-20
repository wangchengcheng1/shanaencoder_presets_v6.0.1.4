# Medium CPU Quality Presets with GPT 5.3 Codex

## Overview

This folder contains medium-speed CPU-based H.265 encoding presets with GPT 5.3 Codex optimization. Provides balanced quality and encoding speed, suitable for scenarios where both quality and reasonable processing time are important.

## Use Cases

- Standard video encoding with quality requirements
- Content where encoding speed matters but quality is not sacrificed
- Streaming and distribution scenarios
- Long-form content processing with time considerations

## Encoding Characteristics

- **Codec**: H.265/HEVC (libx265)
- **Bit Depth**: 10-bit
- **Quality Level**: CRF 20.0 (high quality)
- **Preset Speed**: medium
- **Audio Codec**: libfdk_aac at 192k
- **Container Format**: MP4 with faststart optimization

## Special Features

- **Balanced Encoding**: Optimal compromise between speed and quality
- **GPT 5.3 Codex Optimization**: Intelligent parameter tuning for encoder efficiency
- **10-bit Color Depth**: Preserves color information effectively
- **Optimized Container**: faststart for streaming compatibility

## Recommended For

- Professional video production workflows
- Content distribution platforms
- Standard quality archival with reasonable processing time
- Streaming media files where quality matters

## Notes

- CRF 20.0 with medium preset offers better quality than fast presets with moderate speed increase
- Medium preset uses more efficient encoding algorithms than fast, improving bitrate efficiency
- Suitable as a default preset for most use cases

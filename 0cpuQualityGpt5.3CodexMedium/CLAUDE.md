# Medium Quality CPU x265 Encoding Presets (GPT 5.3 Codex)

## Overview

This folder contains medium-quality CPU-based x265 encoding presets optimized using GPT 5.3 Codex. These presets balance encoding speed with video quality for general-purpose video transcoding.

## Use Cases

- General-purpose video transcoding
- Balanced quality and encoding speed requirement
- Archive and storage encoding
- Standard definition and HD video encoding
- Video distribution to multiple platforms

## Encoding Characteristics

- **Codec**: H.265/HEVC (libx265)
- **Bit Depth**: 10-bit for better color gradation
- **Mode**: CPU-based software encoding
- **Quality Level**: Medium (CRF ~20-24 range)
- **Preset**: Medium speed/quality balance
- **Audio Codec**: AAC (libfdk_aac) at 192kbps

## Preset Organization

Presets are numbered to indicate quality variations:
- Lower numbers: Faster encoding, slightly lower quality
- Higher numbers: Better quality, slower encoding
- Variants include special configurations (BigVoice for content with heavy dialogue)

## Special Variants

- **BigVoice Variant**: Optimized audio handling for dialogue-heavy content
- **Standard Variant**: General-purpose balanced encoding

## Performance Profile

- Encoding speed: Moderate (faster than high quality, slower than fast presets)
- Quality level: Good visual quality suitable for most applications
- CPU efficiency: Well-balanced for multi-threaded processing
- File size: Reduced compared to original while maintaining quality

## Recommended For

- Long-form content (TV shows, movies, lectures)
- Archival storage with good quality preservation
- Multi-platform distribution requiring broad compatibility
- General transcoding workflows with balanced requirements

# High-Quality H.265 10-bit x265 CPU Encoding

## Overview

This folder contains high-quality H.265/HEVC encoding presets using x265 software encoder with very low CRF values. Designed for scenarios where maximum video quality is required despite longer encoding times.

## Use Cases

- Archival with maximum video quality preservation
- Professional video production requiring best quality
- Long-form content where quality is paramount
- High-quality distribution when file size allows

## Encoding Characteristics

- **Codec**: H.265/HEVC (libx265)
- **Bit Depth**: 10-bit
- **Quality Level**: CRF 10.0 (very high quality)
- **Preset Speed**: veryfast
- **Audio Codec**: copy (stream passthrough)
- **Container Format**: MP4 with faststart

## Special Features

- **Very Low CRF**: CRF 10.0 prioritizes quality over file size
- **SSIM Tuning**: Optimized for structural similarity metrics
- **Enhanced Filtering**: Unsharp and deblock filters for visual improvement
- **10-bit Color Depth**: Maximum color information preservation

## Recommended For

- Archival with quality preservation
- Professional production requiring best output
- Scenarios where file size is not a constraint
- Long-term storage with maximum fidelity

## Notes

- CRF 10.0 significantly larger files than standard presets but vastly superior quality
- Veryfast preset balances quality and reasonable encoding speed
- Best-in-class quality for x265 encoding
- SSIM-tuned for perceptual quality metrics

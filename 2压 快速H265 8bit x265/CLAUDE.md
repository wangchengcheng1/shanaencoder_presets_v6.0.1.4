# Fast H.265 8-bit x265 CPU Encoding

## Overview

This folder contains fast H.265/HEVC encoding presets using x265 with 8-bit color depth. Optimized for quick encoding while maintaining decent quality and reduced file sizes compared to 10-bit variants.

## Use Cases

- Quick video encoding with reasonable quality
- Content distribution where speed matters
- Batch processing with moderate quality requirements
- Storage scenarios where file size and speed balance is needed

## Encoding Characteristics

- **Codec**: H.265/HEVC (libx265)
- **Bit Depth**: 8-bit
- **Quality Level**: CRF 19.0
- **Preset Speed**: veryfast
- **Audio Codec**: copy (stream passthrough)
- **Container Format**: MP4 with faststart

## Special Features

- **8-bit Encoding**: Reduces file size compared to 10-bit
- **PSNR Tuning**: Optimized for PSNR quality metrics
- **Fast Processing**: veryfast preset for quick encoding
- **Deblock Filter**: Reduces blocking artifacts

## Recommended For

- Quick video encoding workflows
- Content distribution with speed priority
- Storage with balanced quality-to-size ratio
- Batch processing with moderate quality needs

## Notes

- 8-bit encoding reduces file size vs 10-bit variants
- CRF 19.0 with veryfast preset provides good speed/quality balance
- Smaller files than 10-bit presets while maintaining good quality
- Good for streaming and distribution scenarios

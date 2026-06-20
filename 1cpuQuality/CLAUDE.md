# Standard Quality CPU-Based Encoding Presets

## Overview

This folder contains standard quality CPU-based encoding presets providing balanced quality and encoding performance for general video transcoding tasks.

## Use Cases

- Standard video transcoding
- Quality preservation with reasonable file size reduction
- CPU-only encoding environments (no GPU acceleration)
- Multi-platform video distribution
- Archive storage with acceptable quality

## Encoding Characteristics

- **Codec**: H.265/HEVC (libx265)
- **Bit Depth**: 10-bit
- **Mode**: CPU-based software encoding (no GPU)
- **Quality Level**: Balanced quality/compression ratio
- **Audio Codec**: AAC (libfdk_aac)

## Performance Profile

- Encoding speed: Standard (moderate CPU usage)
- Quality level: Good visual fidelity for most applications
- File size reduction: Effective compression maintaining quality
- Compatibility: Broad device support via H.265

## Presets Organization

Presets are numbered to indicate quality variations from fast to highest quality within the standard tier.

## Suitable For

- General-purpose video transcoding
- Video archival with quality requirements
- Multi-platform distribution workflows
- Content where GPU acceleration is unavailable
- Long-form content (movies, TV shows, lectures)

## Optimization

These presets are optimized for modern multi-core CPUs to achieve good encoding throughput without requiring specialized GPU hardware.

# Fast H.265 8-Bit x265 CPU Encoding Presets

## Overview

This folder contains fast H.265/HEVC encoding presets using x265 CPU encoder with 8-bit encoding depth. These presets prioritize encoding speed while maintaining reasonable quality through x265 optimization.

## Use Cases

- Fast H.265 encoding on CPU systems
- Quick transcoding with good compression
- Real-time video processing workflows
- Batch encoding with time constraints
- Systems prioritizing speed over maximum quality

## Encoding Characteristics

- **Codec**: H.265/HEVC
- **Bit Depth**: 8-bit
- **Encoder**: x265 (CPU-based)
- **Speed**: Optimized for fast encoding
- **Quality Level**: Good balance of speed and quality
- **Audio Codec**: AAC (libfdk_aac)

## Features

- **Speed Optimization**: Preset set to "fast" or "faster" modes
- **Compression**: H.265 efficiency (40-50% smaller than H.264)
- **Quality**: Good visual quality at faster encoding speeds
- **Flexibility**: Still has full x265 capability

## Performance Profile

- Encoding speed: Fast (much faster than quality-focused x265)
- Quality level: Good (suitable for most applications)
- File size: Effective H.265 compression
- CPU usage: High utilization for speed

## Trade-offs vs Quality x265

- **Advantage**: Significantly faster encoding
- **Advantage**: Good compression efficiency
- **Limitation**: 8-bit instead of 10-bit (slightly less color precision)
- **Limitation**: Lower quality than "medium/slow" x265 presets

## When to Use

- Fast transcoding requirements
- Encoding speed more important than maximum quality
- Intermediate encoding (re-encoding later)
- Quick preview encoding
- Batch processing with time constraints

## Performance Scaling

- Scales well with multi-core CPUs
- Good for parallel batch encoding
- Suitable for real-time workflows
- Efficient multi-threaded performance

## Use Case Examples

- Quick video format conversion
- Preview encoding before final quality pass
- Real-time streaming encoding
- Intermediate transcoding steps
- Fast backup encoding

## Comparison

- Faster than 10-bit quality x265
- Slower than NVENC or QSV
- Better quality than hardware accelerators
- 8-bit vs 10-bit trade-off for speed

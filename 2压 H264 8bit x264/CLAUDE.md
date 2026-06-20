# H.264 8-Bit x264 CPU Encoding Presets

## Overview

This folder contains H.264 video encoding presets using the x264 CPU-based software encoder with 8-bit depth. These presets provide excellent compression and quality through mature software encoding.

## Use Cases

- High-quality H.264 encoding on CPU systems
- Systems without GPU acceleration
- Archival encoding requiring good quality
- Professional video encoding with strict quality requirements
- Broad compatibility encoding

## Encoding Characteristics

- **Codec**: H.264 (AVC)
- **Bit Depth**: 8-bit
- **Encoder**: x264 (CPU-based software)
- **Quality Level**: High (superior to NVENC equivalent)
- **Compatibility**: Universal H.264 device support
- **Audio Codec**: AAC (libfdk_aac)

## Benefits

- **Quality**: Better quality than GPU NVENC at same bitrate
- **Compatibility**: H.264 supported by essentially all devices
- **Maturity**: x264 is mature, stable, battle-tested encoder
- **Flexibility**: Full control over encoding parameters
- **Efficiency**: Good compression-to-quality ratio

## Performance Profile

- Encoding speed: Moderate (CPU-bound, slower than NVENC)
- Quality level: High (excellent visual quality)
- File size: Good compression with quality preservation
- CPU usage: Full utilization (multi-threaded)

## Quality Optimization

x264 presets provide excellent quality optimization through:
- Psycho-visual tuning
- Advanced motion estimation
- Scene detection
- Adaptive quantization

## When to Use

- Maximum quality H.264 encoding
- CPU-only systems (no GPU)
- Archival with compatibility requirements
- Professional workflows prioritizing quality over speed
- Encoding where broad device compatibility is critical

## Performance Notes

- Multi-threaded for modern multi-core CPUs
- Scales well with additional CPU cores
- Memory usage: Moderate
- Suitable for real-time and batch encoding

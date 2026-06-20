# Intel Quick Sync Video (QSV) Quality Presets

## Overview

This folder contains quality-focused encoding presets using Intel Quick Sync Video (QSV) GPU acceleration. These presets balance quality optimization with fast hardware-accelerated encoding.

## Use Cases

- Intel GPU-accelerated quality encoding
- Fast H.265 encoding on Intel systems
- Professional Intel-based workflows
- Real-time streaming with Intel hardware
- High-throughput encoding on Intel

## Encoding Characteristics

- **Codec**: H.265/HEVC
- **Bit Depth**: 10-bit (professional color)
- **Acceleration**: Intel Quick Sync Video
- **Speed**: Very fast hardware acceleration
- **Quality Level**: Optimized quality parameters
- **Audio Codec**: AAC (libfdk_aac)

## Hardware Requirements

- Intel processor with QSV support:
  - 6th Gen Core and newer
  - Intel Arc discrete GPUs
  - Mobile/laptop processors with iGPU
  - Professional Intel cards

## Benefits

- **Speed**: Fast hardware-accelerated encoding
- **Efficiency**: Offloads to GPU, minimal CPU
- **Quality**: Optimized quality parameters
- **Power**: Lower power consumption
- **Compression**: H.265 efficiency (50% vs H.264)

## Performance Profile

- Encoding speed: Very fast (GPU accelerated)
- Quality level: High (professional tuning)
- File size: Efficient H.265 compression
- Power usage: Low (integrated GPU)
- CPU usage: Minimal

## Intel GPU Technology

- **Integrated Graphics**: Intel HD/UHD/Iris
- **Discrete GPUs**: Intel Arc series
- **Mobile Support**: Laptop iGPU support
- **Professional**: Intel Xe graphics

## When to Use

- Intel-based systems (workstations/laptops)
- Quality-important with speed needs
- Power-efficient encoding (laptops)
- Real-time streaming on Intel
- Batch processing on Intel servers

## Use Case Examples

- Laptop real-time encoding
- Intel-based media servers
- Professional Intel workstations
- Battery-efficient mobile encoding
- Server-side fast encoding

## Quality Optimization

- Professional QSV parameter tuning
- Adaptive bitrate allocation
- Quality-focused preset selection
- Scene-aware optimization

## Comparison with Other Encoders

| Aspect | vs NVENC | vs x265 | vs x264 |
|--------|----------|---------|---------|
| Speed | Similar | Much faster | Much faster |
| Quality | Good | Better | Better |
| Power | Very low | High | High |
| Intel Support | No | Yes | Yes |

## Professional Applications

- Content creation on Intel platforms
- Professional streaming
- Real-time broadcasting
- Server-side transcoding
- Laptop-based mobile encoding

## Performance Notes

- Excellent for multi-stream encoding
- Suitable for 24/7 server operation
- Laptop battery life friendly
- Professional-grade quality

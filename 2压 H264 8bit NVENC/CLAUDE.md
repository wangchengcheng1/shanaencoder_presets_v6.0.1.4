# H.264 8-Bit NVIDIA NVENC Encoding Presets

## Overview

This folder contains H.264 video encoding presets using NVIDIA NVENC GPU acceleration with 8-bit encoding depth. These presets leverage GPU hardware for fast encoding with good compression.

## Use Cases

- Real-time video encoding with NVIDIA GPU
- Fast H.264 compression for broad device compatibility
- GPU-accelerated batch video processing
- Systems with dedicated NVIDIA GPU hardware
- Quick encoding prioritizing speed over maximum quality

## Encoding Characteristics

- **Codec**: H.264 (AVC)
- **Bit Depth**: 8-bit
- **Acceleration**: NVIDIA NVENC GPU hardware encoding
- **Speed**: Very fast GPU-accelerated encoding
- **Compatibility**: Excellent device compatibility (H.264 is widely supported)
- **Audio Codec**: AAC (libfdk_aac)

## Hardware Requirements

- NVIDIA GPU with NVENC capability:
  - GeForce GTX/RTX series
  - Tesla/Quadro professional cards
  - Modern mobile GPUs

## Benefits

- **Speed**: Fast GPU-accelerated encoding (10-50x faster than CPU)
- **Efficiency**: Offloads encoding to GPU, freeing CPU for other tasks
- **Compatibility**: H.264 widely supported on all devices
- **Quality**: Good balance of compression and quality

## Performance Profile

- Encoding speed: Very fast (GPU accelerated)
- Quality level: Good for general use
- File size: Moderate compression (H.264 standard)
- CPU usage: Minimal (GPU handles encoding)

## Limitations

- Requires NVIDIA GPU with NVENC support
- Quality generally slightly lower than x264 software encoding
- 8-bit depth limits color precision compared to 10-bit

## Ideal Scenarios

- Real-time encoding workflows
- Batch processing with NVIDIA hardware
- Server-side encoding with GPU resources
- When GPU availability is priority over maximum quality

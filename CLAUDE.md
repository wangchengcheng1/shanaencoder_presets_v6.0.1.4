# ShanaEncoder Presets Repository

## Overview

This repository contains XML preset configurations for **ShanaEncoder**, a video encoding tool. Each folder groups related encoding presets by quality level, codec, and use case.

## Repository Structure

### Core Preset Categories

#### CPU-based Quality Presets
- **`0cpuQualityGpt5.3CodexFast`** - Fast CPU-based x265 encoding with GPT 5.3 Codex optimization
- **`0cpuQualityGpt5.3CodexFastScene`** - Scene-focused fast CPU x265 encoding variant
- **`0cpuQualityGpt5.3CodexMedium`** - Medium quality CPU x265 encoding with GPT 5.3 Codex
- **`1cpuQuality`** - Standard quality CPU-based encoding presets
- **`1cpuQualityGpt5.3Codex`** - CPU quality presets with GPT 5.3 Codex optimization

#### Lossless/Passthrough Presets
- **`0压 视频复制流`** - Video stream copy (no re-encoding)
- **`0压 音频复制流`** - Audio stream copy (no re-encoding)

#### H.264 Compression Presets
- **`2压 H264 8bit NVENC`** - H.264 8-bit compression using NVIDIA NVENC GPU acceleration
- **`2压 H264 8bit x264`** - H.264 8-bit compression using x264 CPU encoder

#### H.265/HEVC Compression Presets
- **`2压 H265 10bit NVENC`** - H.265 10-bit compression using NVIDIA NVENC
- **`2压 H265 10bit NVENCfor720pXiaoMiTv`** - H.265 10-bit NVENC optimized for 720p playback on Xiaomi TVs
- **`2压 H265 10bit QSV`** - H.265 10-bit compression using Intel Quick Sync Video
- **`2压 H265 10bit x265`** - H.265 10-bit compression using x265 CPU encoder
- **`2压 快速H265 8bit x265`** - Fast H.265 8-bit compression using x265
- **`2压 高码H265 10bit x265`** - High bitrate H.265 10-bit compression using x265

#### Advanced H.265 Presets
- **`3压 H265 10bit x265`** - Advanced H.265 10-bit x265 presets
- **`3压 快速H265 8bit x265`** - Advanced fast H.265 8-bit x265 presets

#### Audio Presets
- **`2压 音频预设`** - Audio-only compression presets

#### Quality Transformation Presets
- **`qualityCpuTransTo1080p`** - CPU-based transcoding to 1080p resolution
- **`qualityCpuTransTo1080pSameAudio`** - CPU transcoding to 1080p with audio stream copy
- **`qualityCpuTransTo720p`** - CPU-based transcoding to 720p resolution
- **`qualityCpuTransTo720pSameAudio`** - CPU transcoding to 720p with audio stream copy
- **`qualityTransTo1080p`** - Standard transcoding to 1080p resolution
- **`qualityTransTo720p`** - Standard transcoding to 720p resolution

#### GPU-accelerated Presets
- **`nvQuality`** - NVIDIA GPU-accelerated quality presets

#### Special Purpose Presets
- **`qualitySameAudio`** - Quality presets with audio stream copy
- **`qualitySameAudioTransTo1080p`** - Quality + audio copy + 1080p transcoding
- **`qualityQsv`** - Intel Quick Sync Video (QSV) quality presets

#### Legacy/Reference Presets
- **`舟 5.X原预设`** - Original presets from ShanaEncoder 5.X version
- **`舟 6.0原预设`** - Original presets from ShanaEncoder 6.0 version
- **`舟 滤镜参考`** - Filter reference and documentation presets

#### Skills/Tools
- **`skills`** - Utility scripts and tools for the preset system

## File Format

Each preset is stored as an XML file with the following structure:

```xml
<?xml version="1.0" encoding="utf-8"?>
<Settings>
  <extensiontextBox>Output file extension</extensiontextBox>
  <filterparamBoxV>Video filters (FFmpeg format)</filterparamBoxV>
  <filterparamBoxA>Audio filters (FFmpeg format)</filterparamBoxA>
  <encparamBox>Encoding parameters (FFmpeg format)</encparamBox>
  <Logo>Logo overlay configuration</Logo>
</Settings>
```

## Key Encoding Encoders

- **x264** - H.264 software encoder (CPU-based)
- **x265** - H.265/HEVC software encoder (CPU-based)
- **NVENC** - NVIDIA GPU-accelerated encoder
- **QSV** - Intel Quick Sync Video (GPU-accelerated on Intel)
- **libfdk_aac** - AAC audio codec

## Quality Levels

Presets are organized by quality and compression ratio:
- **0压** (0 compression) - Lossless, copy streams without re-encoding
- **1压** (1 compression) - High quality, preserves details
- **2压** (2 compression) - Standard quality, good balance
- **3压** (3 compression) - Lower quality, higher compression

## Naming Conventions

- Files ending in `Same_Audio` preserve original audio (copy stream instead of re-encoding)
- Files ending in `TransTo720p/1080p` resample to specific resolutions
- NVENC variants use NVIDIA GPU acceleration
- QSV variants use Intel GPU acceleration
- x265/x264 variants use CPU-based software encoding

## Usage

Load these presets in ShanaEncoder to apply predefined encoding configurations for batch video processing with consistent quality and performance characteristics.

## Recent Updates

- Scene-focused presets for optimized x265 encoding
- Xiaomi TV compatibility optimization for 720p playback
- GPT 5.3 Codex optimization variants
- Quality/performance tuning across multiple encoder backends

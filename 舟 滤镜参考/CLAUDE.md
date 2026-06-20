# HDR and Filter Reference Presets

## Overview

This folder contains reference presets for HDR/Dolby Vision and advanced filter configurations. Includes presets with color space and mastering metadata support for professional HDR video workflows.

## Use Cases

- HDR and Dolby Vision content encoding
- Professional video production with color grading
- Reference implementations for advanced filters
- HDR streaming distribution

## Encoding Characteristics

- **Codec**: H.265/HEVC (libx265)
- **Bit Depth**: 10-bit
- **Quality Level**: CRF 21.0
- **Preset Speed**: veryfast
- **Profile**: main (supports HDR)
- **Level**: 5.1 (supports higher resolutions)
- **Audio Codec**: copy (stream passthrough)
- **Container Format**: MP4 with faststart

## Special Features

- **HDR Support**: BT.2020 color space with SMPTE 2084 (PQ) transfer function
- **Mastering Metadata**: Master display info and MaxCLL/MaxFALL data
- **Advanced Filters**: 
  - Unsharp filter (0.02) for detail enhancement
  - Subtitle support
  - Deblock filter for artifact reduction
- **Dolby Vision Compatible**: Color space configuration suitable for DV
- **Professional Grade**: Level 5.1 profile support

## Recommended For

- HDR content encoding and delivery
- Dolby Vision material preparation
- Professional video production
- HDR streaming platforms

## Notes

- Requires HDR-capable source and target devices
- BT.2020 color space (wide gamut) ensures proper color representation
- SMPTE 2084 (PQ) transfer function for HDR brightness levels
- Profile and level settings ensure HDR compatibility
- Master display metadata helps with tone mapping

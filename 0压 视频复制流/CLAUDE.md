# Video Stream Copy Presets

## Overview

This folder contains presets for video stream copy operations. These presets do NOT re-encode the video stream but copy it directly from source to output, preserving original quality and format.

## Use Cases

- Re-container video without re-encoding (e.g., AVI to MP4)
- Fast format conversion
- Preserve original video quality
- Remove or replace audio without touching video
- Quick file format changes

## Encoding Characteristics

- **Video Codec**: Stream copy (no re-encoding)
- **Quality**: Lossless (100% quality preservation)
- **Speed**: Extremely fast (no encoding computational cost)
- **File Size**: Minimal changes (only container overhead)

## Benefits

- **Speed**: Near-instant operation compared to re-encoding
- **Quality**: Perfect lossless video preservation
- **CPU Usage**: Minimal (data copy operation only)
- **Compatibility**: Depends on container and codec compatibility

## Important Considerations

- Output container must support source video codec
- Some devices may not support certain codec/container combinations
- Video filter operations are NOT possible with stream copy
- Works only with compatible codec/container pairs

## Common Use Cases

- MP4/MOV container conversion
- Removing incompatible audio tracks
- Adding new audio track to video
- Quick backup with format conversion
- Container changes without quality loss

## Performance

- Encoding time: Near-instantaneous (seconds for large files)
- CPU usage: Negligible
- Output quality: Identical to input (lossless)
- File size: Essentially unchanged

# Quality Presets with Audio Stream Copy

## Overview

This folder contains quality encoding presets where the video stream is re-encoded but the audio stream is copied without re-encoding (stream copy mode). This preserves original audio quality while optimizing video compression.

## Use Cases

- Preserve original audio quality while re-encoding video
- Reduce encoding time by skipping audio transcoding
- Maintain high-fidelity audio tracks (lossless audio)
- Batch processing with consistent audio requirements

## Encoding Characteristics

- **Video Codec**: H.265/HEVC (libx265)
- **Bit Depth**: 10-bit video encoding
- **Audio Mode**: Stream copy (no re-encoding)
- **Quality Level**: CPU-optimized quality presets
- **Container**: MP4 format

## Benefits

- **Faster Encoding**: Audio stream copy is significantly faster than transcoding
- **Audio Quality**: Original audio quality preserved perfectly
- **File Size**: Optimized video with no audio transcoding overhead
- **Compatibility**: Maintains original audio codec compatibility

## Considerations

- All audio tracks must be compatible with MP4 container
- Audio codec must be supported by target devices
- Cannot modify audio properties (sample rate, channels, etc.)

## When to Use

Use these presets when your original audio is already in the desired format and you want to focus on video quality optimization without re-encoding audio.

## Quality Levels

Available presets provide different quality/speed trade-offs while keeping audio unchanged.

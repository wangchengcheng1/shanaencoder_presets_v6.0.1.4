# Audio Stream Copy Presets

## Overview

This folder contains presets for audio stream copy operations. These presets preserve the original audio stream without re-encoding while allowing video processing.

## Use Cases

- Preserve original audio quality while changing video
- Extract audio with video re-encoding
- Avoid audio transcoding overhead
- Maintain high-fidelity audio tracks
- Fast audio/video processing

## Encoding Characteristics

- **Audio Codec**: Stream copy (no re-encoding)
- **Quality**: Lossless audio preservation
- **Speed**: Fastest audio processing (copy only)
- **Compatibility**: Depends on container support

## Benefits

- **Quality**: Perfect audio preservation
- **Speed**: Avoids audio transcoding computational cost
- **Fidelity**: Original audio format and quality maintained
- **Simplicity**: No audio codec selection needed

## Important Considerations

- Output container must support source audio codec
- Cannot modify audio properties (sample rate, channels, etc.)
- Audio filter operations are NOT possible
- Video can be re-encoded independently

## Common Scenarios

- Video re-encoding with original audio preservation
- Format conversion keeping original audio
- Audio codec compatibility changes via container conversion
- Multi-audio track management
- Batch processing with consistent audio requirements

## Performance

- Audio processing time: Negligible (copy operation only)
- CPU usage: Minimal
- Audio quality: 100% preservation (lossless)
- File size: No audio compression applied

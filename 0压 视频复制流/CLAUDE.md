# Video Stream Copy (Lossless - No Re-encoding)

## Overview

This folder contains lossless video passthrough presets that copy video streams without any re-encoding. Only container format conversion is performed, preserving original video quality and characteristics.

## Use Cases

- Container format conversion without quality loss
- Re-muxing video files to different container formats
- Changing file formats while preserving video integrity
- Quick file format conversion without processing overhead

## Encoding Characteristics

- **Codec**: copy (no re-encoding)
- **Quality Level**: Lossless - identical to source
- **Processing**: Container conversion only
- **Audio Codec**: copy (stream passthrough)
- **Container Format**: FLV

## Special Features

- **Zero Transcoding**: No video re-encoding whatsoever
- **Lossless Quality**: Original video completely preserved
- **Minimal Processing**: Container format change only
- **Maximum Speed**: Fastest possible conversion

## Recommended For

- Container format conversion (MP4 to FLV, etc.)
- Quick file re-muxing without quality degradation
- Archival where source quality must be preserved
- Format compatibility without re-encoding overhead

## Notes

- Produces exact copy of video data, only changes container
- Significantly faster than any re-encoding operation
- No quality loss - identical to source video
- Best option when only format change is needed

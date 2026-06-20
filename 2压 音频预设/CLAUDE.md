# Audio Encoding Presets

## Overview

This folder contains audio-only encoding presets for audio compression and format conversion. These presets focus on audio transcoding with various quality and codec options.

## Use Cases

- Audio extraction and re-encoding
- Audio format conversion
- Audio quality optimization
- Dialogue and speech optimization
- Multi-track audio processing

## Preset Types

Various audio presets for different purposes:
- **Standard audio**: General-purpose audio encoding
- **High quality audio**: Lossless or near-lossless audio
- **Dialogue/Speech**: Optimized for voice content
- **Music**: Optimized for music content
- **Streaming**: Optimized for low-bitrate streaming

## Audio Codecs Supported

- **AAC (libfdk_aac)**: High-quality AAC encoding
- **MP3**: Standard MP3 format
- **FLAC**: Lossless compression
- **Opus**: Modern low-bitrate codec
- **PCM**: Uncompressed audio

## Encoding Characteristics

- **Focus**: Audio-only transcoding
- **Quality Levels**: Various bitrates and codecs
- **Container**: MP4, MKV, or audio-only formats
- **Metadata**: Preserve or optimize audio metadata

## Common Audio Presets

- **192 kbps AAC**: Transparent quality (general purpose)
- **128 kbps AAC**: Good quality, smaller files (streaming)
- **320 kbps MP3**: High-quality MP3
- **Lossless FLAC**: Archive-quality audio
- **Opus Low**: Low-bitrate streaming

## Performance

- Encoding speed: Very fast (audio-only)
- CPU usage: Minimal compared to video
- File size: Depends on bitrate and codec
- Quality: Excellent with appropriate bitrate

## When to Use

- Extracting audio from video files
- Audio format conversion
- Optimizing audio track quality
- Batch audio processing
- Audio/video separation workflows

## Audio Quality Guidelines

- **Transparent**: 192+ kbps AAC, 320 kbps MP3
- **High Quality**: 128+ kbps AAC, 192+ kbps MP3
- **Streaming**: 96-128 kbps (speech/dialogue)
- **Lossless**: FLAC, WAV, uncompressed

## Professional Notes

- Preserve original audio for archival
- Use appropriate bitrate for content type
- Consider playback device audio codec support
- Plan for multiple audio track encoding

# Scene x265 Cheat Sheet / 场景压制速查

## Goal Matrix / 目标矩阵

- Size-first: `-crf 26` with `-qmin 18 -qmax 40`
- Balanced: `-crf 24` with `-qmin 17 -qmax 36`
- Detail-first: `-crf 23` with `-qmin 16 -qmax 34`

## Audio Strategy / 音频策略

- Keep original audio (`-c:a copy`) when source audio is already acceptable.
- Use AAC 192k (`-c:a libfdk_aac -b:a 192k`) when compatibility or normalization is needed.

## Decision Tips / 决策建议

- If output gets larger than source, raise CRF first (for example 24 -> 26).
- If block artifacts appear in dark or motion-heavy scenes, tighten `qmax` (for example 40 -> 36).
- If bitrate spikes too much in easy scenes, raise `qmin` slightly (for example 17 -> 18).

## Test Protocol / 抽样协议

1. Pick 3 clips: dark scene, high motion scene, normal daylight scene.
2. Encode with two candidate presets.
3. Compare subjective quality and file size before batch jobs.

---
name: shanaencoder-x265-lab
description: Build and maintain scene-focused x265 CPU presets in a reversible A/B workflow. Use when tuning `-crf`, `-qmin/-qmax`, audio mode (`copy` vs AAC), and goal-oriented preset branches such as size-first, balanced, and detail-first. 用于 场景化 x265 CPU 预设调参：围绕体积、画质、速度做可回滚的分支化维护与 A/B 对比。
---

# Scene X265 Lab / 场景化 x265 调参技能

## Purpose / 目标

Create stable, reusable scene preset variants without overwriting proven presets.  
不覆盖稳定旧预设，新增可复用的 场景分支方案并支持快速回退。

## Workflow / 工作流

1. Pick one baseline preset (for example `24qualityCpuFast.xml`).
2. Split by intent: `size-first`, `balanced`, `detail-first`, and `same-audio`.
3. Keep one variable theme per branch:
   - quality axis: `-crf`
   - guardrail axis: `-qmin/-qmax`
   - audio axis: `-c:a copy` vs `-c:a libfdk_aac -b:a 192k`
4. Keep filters unchanged unless user explicitly requests changes.
5. Write a short profile note with:
   - source type
   - target resolution
   - quality tier
   - key filters
6. Validate with short clips before batch encoding.

## Practical Defaults / 实战默认值

- Balanced scene (1080p): `-crf 24 -qmin 17 -qmax 36 -preset fast`
- Size-first scene: `-crf 26 -qmin 18 -qmax 40 -preset fast`
- Detail-first scene: `-crf 23 -qmin 16 -qmax 34 -preset fast`
- Same-audio branch: prefer `-c:a copy` when source audio is acceptable

## Guardrail Interpretation / 上下限理解

- `qmin` prevents bitrate spikes caused by over-preserving easy frames.
- `qmax` avoids severe quality collapse in hard scenes.
- Removing guardrails increases CRF freedom and scene adaptivity, but output size is less predictable.

## Safety Rules / 安全规则

- Do not delete or overwrite stable preset files by default.
- Prefer adding a sibling folder for new strategies.
- Keep naming explicit so batch scripts can filter by keywords.

## References / 参考

Read [scene-x265-cheatsheet.md](references/scene-x265-cheatsheet.md) for quick decision guidance.


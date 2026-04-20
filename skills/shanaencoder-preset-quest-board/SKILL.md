---
name: shanaencoder-preset-quest-board
description: Turn preset tuning into mission cards (Size Rush, Quality Keeper, Speed Run, SameAudio Saver) with clear goals and constraints. Use when users want guided, playful iteration paths instead of ad-hoc parameter edits. 用于把调参流程任务化，让预设迭代更有方向和可玩性。
---

# Preset Quest Board / 预设任务板

## Goal / 目标

Convert vague requests into concrete "quests" with win conditions.

## Mission Cards / 任务卡

Use [mission-cards.md](references/mission-cards.md).

- `Size Rush`: minimize output size with acceptable quality.
- `Quality Keeper`: maximize detail retention, allow larger size.
- `Speed Run`: reduce encode time while staying watchable.
- `SameAudio Saver`: keep source audio, optimize video only.

## Quest Flow / 流程

1. Pick one mission card.
2. Clone one baseline preset as quest branch.
3. Apply only card-allowed parameter changes.
4. Run short sample validation.
5. Mark `PASS` / `RETRY` / `ARCHIVE`.

## Naming / 命名

- Prefix quest outputs with `QST_`.
- Example: `QST_SizeRush_24Fast_v1.xml`

## Constraints / 约束

- No direct overwrite of stable presets.
- One mission card per branch.
- Keep change log short and explicit.

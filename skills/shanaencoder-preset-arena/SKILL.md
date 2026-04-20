---
name: shanaencoder-preset-arena
description: Run preset "arena" A/B/C battles on fixed sample clips and select winners by a transparent scorecard. Use when choosing among multiple CRF/qmin/qmax/preset variants for the same source type. 用于固定样本的预设擂台赛：在多个候选方案中快速选出可推广的版本。
---

# Preset Arena / 预设擂台赛

## Goal / 目标

Make preset comparison fun and repeatable, not guesswork.

## Arena Rules / 对战规则

1. One baseline + up to two challengers.
2. Same source clip pack for all contenders:
   - dark scene (30-60s)
   - high motion scene (30-60s)
   - normal daylight scene (30-60s)
3. Keep container/filter chain identical during a match.
4. Compare only one tuning theme per round:
   - CRF round
   - qmin/qmax round
   - audio mode round

## Scoring / 评分

Use [arena-scorecard.md](references/arena-scorecard.md).

- Size score: smaller file gets higher score.
- Quality score: fewer artifacts in dark/motion/skin.
- Speed score: shorter encode time gets higher score.
- Decision:
  - `2 wins` or better -> promote as candidate preset.
  - `1 win` -> keep for next round.
  - `0 win` -> archive as failed branch.

## Promotion Policy / 晋级规则

- Never overwrite stable presets directly.
- Promote by creating new branch files/folder names.
- Record what changed and why it won.

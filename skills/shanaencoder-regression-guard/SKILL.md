---
name: shanaencoder-regression-guard
description: Add guardrails before and after bulk preset edits to catch unintended parameter regressions. Use when touching many XML files or updating policy-wide defaults. 用于大批量改 XML 前后做防回归检查，避免误改导致全仓质量/兼容性倒退。
---

# Regression Guard / 防回归守卫

## Goal / 目标

Catch accidental mass mistakes before they spread.

## Guard Steps / 守卫步骤

1. Pre-change snapshot:
   - file count by folder
   - key line samples (`-c:v`, `-c:a`, `-movflags`, `-tag:v`)
2. Apply intended change to target scope only.
3. Post-change checks:
   - malformed XML check
   - target parameter present
   - unrelated parameter unchanged
4. Spot review by representative files (`23/24/26` quality tiers).

## Red Flags / 高危信号

- Unexpected audio mode change (`copy` <-> AAC).
- Missing `-tag:v hvc1` on HEVC outputs.
- Missing `-movflags faststart` for MP4.
- qmin/qmax inserted into non-target encoders.

## Rollback Policy / 回退策略

- If any red flag appears, stop rollout.
- Restore only the affected branch/folder.
- Re-run scoped patch with narrower filters.

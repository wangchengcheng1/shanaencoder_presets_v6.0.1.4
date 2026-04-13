---
name: shanaencoder-preset-maintainer
description: Maintain and optimize ShanaEncoder XML presets with safe, repeatable folder-level workflows, bilingual naming, and parameter consistency checks. Use when editing `.xml` preset files, cloning preset folders (for A/B variants), bulk-renaming preset files, or applying controlled parameter changes such as `-movflags faststart`, `-preset`, `-crf`, audio mode, and frame-rate mode. 用于维护和优化 ShanaEncoder 的 `.xml` 预设：批量复制目录、重命名文件、统一参数、对比新旧方案，以及做可回滚的安全修改。
---

# ShanaEncoder Preset Maintainer / ShanaEncoder 预设维护

## Purpose / 目标

Keep preset maintenance stable, reversible, and easy to compare.  
让预设维护可回退、可对比、可复用。

## Core Workflow / 核心流程

1. Inspect target folders and XML files before editing.  
先检查目标目录与 XML，再动手改。
2. Prefer creating a parallel variant folder for major tuning changes.  
重大调参优先新建“平行版本目录”，不要直接覆盖原方案。
3. Apply one parameter theme at a time (for example `faststart`, then `preset`).  
一次只改一类参数（例如先加 `faststart`，再改 `preset`）。
4. Verify with spot checks on representative files (for example `24quality...xml`).  
至少抽检代表性文件（如 `24quality...xml`）确认参数生效。
5. Output a concise mapping from old to new names when cloning/renaming.  
涉及复制和重命名时，输出旧名到新名映射表。

## Editing Rules / 修改规则

- Keep source presets unless user explicitly asks to replace them.  
除非用户明确要求覆盖，否则保留原预设。
- Keep naming predictable: `<base>Optimized.xml` for optimized variants.  
优化版默认命名为 `<原名>Optimized.xml`。
- Keep audio/video intent unchanged unless requested (for example `copy` vs re-encode).  
未被要求时，不改变音视频处理意图（如 `copy` 与重编码）。
- Add `-movflags faststart` for MP4 outputs unless a format-specific conflict appears.  
MP4 默认添加 `-movflags faststart`，除非遇到格式冲突。
- For speed-size tradeoff, use `-preset fast` in optimized variants and keep baseline as control.  
速度与体积权衡：优化分支可用 `-preset fast`，并保留基线分支做对照。

## Validation Checklist / 校验清单

1. Confirm XML files are readable and not malformed.  
确认 XML 可正常读取，无结构破损。
2. Confirm expected parameters exist in both old/new folders as intended.  
确认新旧目录参数符合预期（如 only new folder uses `-preset fast`）。
3. Confirm file counts and naming mappings match 1:1 unless explicitly excluded.  
确认文件数量和命名映射为 1:1（除非有明确排除）。
4. Report risks clearly (speed impact, compatibility impact, or quality uncertainty).  
明确提示风险（速度、兼容性、画质不确定性）。

## References / 参考资料

Read [parameter-notes.md](references/parameter-notes.md) when choosing preset flags or explaining tradeoffs.

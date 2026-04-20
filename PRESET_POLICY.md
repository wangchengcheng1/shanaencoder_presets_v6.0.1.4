# PRESET POLICY

## 生效日期

- `2026-04-13`（建立统一策略）
- `2026-04-19`（新增 场景分支预设与技能化维护说明）

## 全局统一策略（适用于全仓 XML）

1. 不强制固定帧率：移除 `-fps_mode cfr`。
2. 不做音量放大：移除 `volume=...`。
3. 不使用 limiter：移除 `alimiter=...`。
4. MP4 统一前置索引：保留/添加 `-movflags faststart`。
5. HEVC 兼容标记：对 HEVC 编码（如 `libx265` / `hevc_*`）添加 `-tag:v hvc1`。
6. 音频复制不加滤镜：`-c:a copy` 的预设不新增音频处理链。

## 主要目录的定位与差异

### `0cpuQuality`

- 角色：基线方案（更快）。
- 视频参数：`-preset veryfast`。
- 质量约束：保留 `-qmin/-qmax`。
- 文件命名：原始命名（如 `24qualityCpu.xml`）。

### `0cpuQualityGpt5.3Codex`

- 角色：优化方案（更省体积倾向）。
- 视频参数：`-preset fast`。
- 质量约束：移除 `-qmin/-qmax`，让 CRF 自适应。
- 文件命名：`*Optimized.xml`（如 `24qualityCpuOptimized.xml`）。

### `0cpuQualityGpt5.3CodexFast`

- 角色：优化方案 + 文件名显式区分。
- 参数：与 `0cpuQualityGpt5.3Codex` 一致（`-preset fast`、无 `qmin/qmax`）。
- 文件命名：`*Fast.xml`（如 `24qualityCpuFast.xml`）。
- 输出后缀：`[se6qualityCpuFastXX].mp4` 规则（如 `[se6qualityCpuFast24].mp4`）。
- 场景分支：允许在本目录新增 `*Scene_*.xml` 作为场景化策略，不覆盖原 `*Fast.xml`。

### `0cpuQualityGpt5.3CodexFast`（场景分支）

- 角色：场景化实验组（A/B 对比用），保留基线文件不动。
- 质量约束：按目标拆分为“自由 CRF / 均衡护栏 / 体积优先 / 细节优先 / 原音保留”。
- 文件命名：`*Scene_*.xml`（如 `24qualityCpuFastScene_BalancedGuard.xml`）。
- 记录要求：每个新增场景预设须注明“适用素材、目标分辨率、质量档位、关键滤镜开关”。

### `0cpuQualitySameAudio`

- 角色：保留原音轨（`-c:a copy`）的优化方案。
- 视频参数：`-preset fast`。
- 质量约束：移除 `-qmin/-qmax`，让 CRF 自适应。
- 播放兼容：保留 `-tag:v hvc1`（HEVC）。
- MP4 体验：保留/添加 `-movflags faststart`。
- 音频策略：不重编码音频，不新增音频放大与 limiter。

## 使用建议

1. 日常大量压制优先用 `0cpuQuality`（更快）。
2. 收藏/长期存储优先用 `0cpuQualityGpt5.3Codex` 或 `0cpuQualityGpt5.3CodexFast`（更偏压缩效率）。
3. 场景类素材优先从 `0cpuQualityGpt5.3CodexFast` 的 `*Scene_*.xml` 小样本 A/B 后再批量。
4. 涉及大范围参数调整时，先复制新目录做 A/B，对比后再推广。

## 变更纪律

1. 修改策略时，先更新本文件，再批量改 XML。
2. 每次大改至少抽测一条动漫、一条真人、一条高运动素材。
3. 若发现兼容问题，优先新增分支预设，不直接覆盖稳定预设。


## 同步与版本约定（Chunfen/Jingzhe 脚本）

- 母版与分段同步：当分段脚本（如 01A/01B/01C/01D）发生内容或结构更新时，必须同步更新对应的母版中英稿（如 `Chunfen/sora_script_en_01_sun_rite.md` 与 `Chunfen/sora_script_cn_01_sun_rite.md`），确保镜头、机位与物理细节一一对应。
- 生成策略：Sora 生成阶段严格按分段执行（如 15s+15s+10s+10s），母版仅作为审阅与剪辑参考。母版时间线开头与结尾保留“黄纸+墨波纹”，中段不使用“收束”。
- 风格与物理一致：统一“复古黄纸+水墨”“右侧清晨光”“风向右→左”“阴影/烟/丝带/水面运动一致”等；禁止在生成阶段出现屏幕文字与音频。
- 关键帧一致：分段的 MJ 关键帧提示与母版风格需一致，用于构图/色温/材质的标尺；如进行无缝拼接，删除中段黄纸转场并以关键帧对齐机位与主体位置。

## Chunfen 专项规则更新（2025-12-29）

- 开头/结尾无水墨晕染：所有分镜脚本开头与末尾不再使用水墨晕染或任何入场/退场特效。片段从首镜头直接起始，末帧直接结束。
- 转场改为直接切镜：分镜之间采用直接镜头切换（hard cut），不再使用墨波纹或其他风格化转场。
- 风格更新为“复古”而非“黄纸”：取消强制“黄纸”背景要求，改为广义复古风格。根据场景选择合适的满屏背景或语义化环境布置（示例：果盘置于对应复古台面/屋内背景，而非悬置在黄纸上）。
- 物理与光风一致：仍保持右侧晨光、风向右→左、阴影与风/烟/丝带/草/水面运动一致等物理逻辑；生成阶段继续“无声无字”。
- 适用范围：以上更新适用于 Chunfen 项目所有分镜与母版；既有脚本逐步迁移到该规范。
# Workflow Rules — 24 Solar Terms Video

Final policy (effective now)
- Sora output: visuals-only (silent), no on-screen text, no embedded narration.
- Post-production: use Jianying (剪映) AI Voiceover for Mandarin narration and Jianying AI Subtitles for Chinese captions.
- Text handling: all titles, solar-term names, custom names, and subtitles are added in post; Sora never renders text.
- Audio handling: all VO/music/SFX are mixed in post; if Sora supplies audio, discard or mute it.

Consistency
- Aspect ratio 16:9; per-custom duration 10–15s.
- Style: vintage yellow rice paper + ink-wash; dawn/dusk lighting; right-side light; wind right→left; shadows consistent.
- Transitions: ink-ripple reveal/retract between rice paper and scene; keep endings on rice paper for stitching.

Implementation notes
- Prompts/scripts may include “text intent” or VO lines for timing, but generation must ignore on-screen text/VO.
- Use provided `voice_profile.md` for VO timbre reference if synthesizing outside Jianying.
- Use `*.srt` files or Jianying auto-caption to generate final subtitles in post.

Fallbacks
- If Jianying AI voice or subtitles require manual timing, align to the SRTs in each folder.
- If Sora length requires splitting, keep rice paper at edges for natural joins.

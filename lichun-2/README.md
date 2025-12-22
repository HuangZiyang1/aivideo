# 立春·鞭春（15秒）

- 最终政策：Sora 仅输出无声、无字的成品画面；中文配音与中文字幕由剪映 AI 在后期生成与叠加。
- 时长：15s；画幅 16:9；风格与参数延续 `Lichun` 版本（复古黄纸版 + 水墨浸染，古风写意，清晨右侧光，风向右→左）。
- 文字与音频：投喂 Sora 时请忽略脚本中的文字与配音指令，仅生成画面；如需旁白与字幕，请参照下方文件在剪映中后期完成。

## 文件说明
- Sora英文脚本（带字幕与配音指令）：见 [lichun-2/sora_script_en.md](lichun-2/sora_script_en.md)
- 中文旁白文本：见 [lichun-2/voiceover_cn.md](lichun-2/voiceover_cn.md)
- 中文字幕 SRT：见 [lichun-2/subtitles_cn.srt](lichun-2/subtitles_cn.srt)
- 统一配音音色规范：见 [lichun-2/voice_profile.md](lichun-2/voice_profile.md)

### 咬春（10秒，字幕+配音）
- Sora英文脚本：见 [lichun-2/yaochun/sora_script_en.md](lichun-2/yaochun/sora_script_en.md)
- 中文旁白文本：见 [lichun-2/yaochun/voiceover_cn.md](lichun-2/yaochun/voiceover_cn.md)
- 中文字幕 SRT：见 [lichun-2/yaochun/subtitles_cn.srt](lichun-2/yaochun/subtitles_cn.srt)

## 使用建议
- 生成画面：仅使用 `sora_script_en.md` 的镜头与物理逻辑说明，忽略文字/配音条目。
- 旁白：在剪映中用 AI 配音（参考 [voice_profile.md](lichun-2/voice_profile.md)）或外部 TTS 生成，再导入时间线。
- 字幕：在剪映中用 AI 字幕自动生成或导入 `subtitles_cn.srt` 校对与美化。
- 全局规则：详见 [WORKFLOW_RULES.md](../WORKFLOW_RULES.md)。
- 镜头与物理逻辑与 `Lichun` 保持一致：
  - 光线：清晨右侧入射；风：右→左；阴影随风与光一致。
  - 转场：统一使用墨波纹从宣纸到场景，再回到宣纸。

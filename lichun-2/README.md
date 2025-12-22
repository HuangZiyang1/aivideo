# 立春·鞭春（15秒，带字幕与配音）

- 目标：测试 Sora 直接生成“片内中文字幕 + 中文配音”的能力。
- 时长：15s；画幅 16:9；风格与参数延续 `Lichun` 版本（复古黄纸版 + 水墨浸染，古风写意，清晨右侧光，风向右→左）。
- 文字与音频：本版本允许 Sora 渲染片内文字与中文配音；若渲染不稳定，改为后期叠加（保留本文件中的 SRT 与旁白文本）。

## 文件说明
- Sora英文脚本（带字幕与配音指令）：见 [lichun-2/sora_script_en.md](lichun-2/sora_script_en.md)
- 中文旁白文本：见 [lichun-2/voiceover_cn.md](lichun-2/voiceover_cn.md)
- 中文字幕 SRT：见 [lichun-2/subtitles_cn.srt](lichun-2/subtitles_cn.srt)

## 使用建议
- 直接投喂 Sora 时，先尝试整段脚本（15s），如出现文字/音频不稳定，可改用后期：
  - 保持画面生成不含文字，后期用 `subtitles_cn.srt` 叠加。
  - 配音不稳定时，使用 `voiceover_cn.md` 文本做 TTS，再合成到时间线上。
- 镜头与物理逻辑与 `Lichun` 保持一致：
  - 光线：清晨右侧入射；风：右→左；阴影随风与光一致。
  - 转场：统一使用墨波纹从宣纸到场景，再回到宣纸。

# 惊蛰（24秒，Sora仅画面）

- 最终政策：Sora 仅输出无声、无字的成品画面；中文配音与中文字幕由剪映 AI 在后期生成与叠加。
- 习俗拆分与时长：
  - 习俗A（农事：春耕与害虫防治）12s
  - 习俗B（民俗：熏艾祛虫与打小人祈安）12s
- 画幅与风格：16:9；复古黄纸版 + 水墨浸染；清晨右侧光；风向右→左；墨波纹转场；物理逻辑一致。
- 使用：
  - 画面生成：按 `sora_script_en.md` 的分镜与物理逻辑投喂 Sora；忽略脚本中的文本与配音条目。
  - 旁白：在剪映用 AI 配音（参考 `../lichun-2/voice_profile.md` 音色参数）或外部 TTS 生成，再导入时间线。
  - 字幕：在剪映用 AI 字幕自动生成或导入本目录的 `subtitles_cn.srt` 校对与美化。
  - 全局规则：详见 [WORKFLOW_RULES.md](../WORKFLOW_RULES.md)。
  - 快速复制：若需要“一次粘贴”的紧凑英文提示，见 [Jingzhe/sora_prompt_compact_en.txt](Jingzhe/sora_prompt_compact_en.txt)。可用24秒整段或拆分为两个12秒块投喂。
  - 单段生成（推荐）：直接使用分拆脚本 [Jingzhe/sora_script_en_A.md](Jingzhe/sora_script_en_A.md) 与 [Jingzhe/sora_script_en_B.md](Jingzhe/sora_script_en_B.md)，每份仅含全局设置与单段分镜，时间轴均从0秒开始，便于贴给 Sora 一次生成一个视频。

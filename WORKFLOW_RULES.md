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

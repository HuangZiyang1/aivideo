# Sora Script (English) — Lichun-2 / Rite of Spring (15s, with Chinese subtitles & VO)

Objective (final policy): Generate visuals-only (silent, no on-screen text) for a single 15-second shot, while keeping the visual style consistent with the Lichun version (vintage rice paper + ink-wash, classical ambience). All narration and captions will be added in post using Jianying AI.

Voice profile (unified across all clips)
- Narrator: mature Mandarin male, baritone, warm and resonant, steady breath; reference tone: documentary narrator in “A Bite of China” (国风雄厚大叔男声，娓娓道来)。
- Tempo & prosody: speaking rate ~0.92× of normal; calm cadence; slight downward inflection at phrase ends; avoid theatrical exaggeration.
- Diction: Standard Putonghua (no regional accent), clear finals and retroflex; light smile tone on blessings.
- Recording style: single close mic, dry (no reverb), center-panned; dynamics gentle compression; VO always on top of ambience.

Global settings
- Aspect ratio: 16:9; Duration: 15 seconds.
- Style: classical Chinese ink-wash over vintage yellow rice paper; semi-realistic textures; dignified festive tone.
- Light & wind: morning light entering from the right; wind flows right-to-left (low to medium); shadows react consistently.
- Transitions: ink-ripple reveal from rice paper to scene, and retract back to rice paper.
- Text rendering: IGNORE for generation (visuals-only). Any text intent below is for post-production reference.
- Voiceover: IGNORE for generation (visuals-only). Use the voice profile above in post when synthesizing VO.
- Audio cues: festive drums, controlled celebratory firecracker ambience (subtle), crowd murmur; prioritize clarity of VO.

Timeline & directions (15s)
0.0–0.5s (Pre-roll)
- Start on vintage rice paper with ink edges; very slight push-in; hold silence.

0.5–2.5s (Title / Opening)
- Subtitles: "立春·鞭春".
- Visuals: ink-ripple reveals a classical street; ceremonial atmosphere; banners minimal.
- Camera: ultra-slow push-in; focal 45mm→55mm.
- VO: speak the title succinctly or keep VO silent per preference (recommended: read softly).

2.6–5.0s (Spring official announcing)
- Subtitles: "春官报春到，福气满门绕".
- Visuals: a performer styled as "春官" with crown and ribbons, walking through the street; mild drum beats; an assistant hands out spring ox prints and solar-term posts.
- Action: "春官" calls out; background crowd offers respectful bows.
- Camera: slow left pan with gentle dolly-in; stable.
- VO: read the subtitle line clearly, celebratory but dignified.

5.1–7.2s (Government spring report, delivery)
- Subtitles: "官府派人向民众报春，送春牛帖子与立春帖子".
- Visuals: close/mid shots of prints: spring ox chart with 24 solar terms, and "立春" post; texture highlighted by right-side morning light.
- Camera: minimal dolly-in; steady.
- VO: read the line with informative tone.

7.3–9.0s (Chant: Spring arrives)
- Subtitles: "春来了！春来了！".
- Visuals: quick crowd response; banners gently wave; wind-chime rings softly.
- Camera: slight push-in; natural motion.
- VO: enthusiastic delivery; short pauses between the repeats.

9.1–11.0s (Chant 1)
- Subtitles: "一打风调雨顺，二打国泰民安".
- Visuals: clay spring ox in mid shot while symbolic light taps occur; small clay crumbs visible; drums synchronize.
- Physics: wind right-to-left; shadows consistent.
- VO: rhythmic delivery matching drum accents.

11.1–13.0s (Chant 2)
- Subtitles: "三打五谷丰登".
- Visuals: banners and crowd in mid shot; celebratory mood remains orderly.
- Camera: micro dolly-in; steady.
- VO: emphasize "五谷丰登" with positive cadence.

13.1–15.0s (Chant 3 / Closure)
- Subtitles: "春牛打得满地转，今年吃穿不用愁".
- Visuals: a final symbolic tap on the clay ox; the scene gently retracts via ink-ripple back to rice paper.
- Camera: slight pull-back to neutral; end on clean rice paper.
- VO: conclude warmly, hold a brief tail.

Continuity & constraints
- No modern school uniform or school emblem elements.
- Keep camera motion minimal for generation stability.
- Maintain physical logic: right-side light, wind right-to-left; shadows follow.
- If subtitles or VO fail to render, output visuals only; then overlay [lichun-2/subtitles_cn.srt] and TTS from [lichun-2/voiceover_cn.md] during editing.

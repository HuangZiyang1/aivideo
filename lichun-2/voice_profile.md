# Voice Profile — Unified Narration (CN)

Target timbre: mature Mandarin male baritone; warm, resonant, documentary style similar to “A Bite of China”.

- Register & tone: baritone; calm authority with gentle warmth; no theatrical exaggeration.
- Prosody: speaking rate ~0.92×; clear phrasing; slight downward inflection at phrase ends; micro-pauses between clauses (150–250ms).
- Diction: Standard Putonghua; clean finals (n/ng), accurate retroflex (zh/ch/sh/r), stable tone sandhi; avoid local accent.
- Recording style: single close mic, dry (no reverb), center-panned; light compression; peak around −3 dBFS; integrated loudness ≈ −16 LUFS; 48 kHz / 24-bit.
- Mix policy: VO on top; ambience −24 to −20 LUFS; music sidechained −3 dB during VO; gentle high-pass at 80 Hz on VO.
- Safety: avoid sibilance; de-esser at 6–8 kHz if needed.

## SSML Template (Azure TTS example)
Replace YOUR_REGION and YOUR_KEY. Use `zh-CN-YunxiNeural` or `zh-CN-YunjianNeural` as baritone-adjacent references; tune rate/pitch to match target.

```xml
<speak version="1.0" xml:lang="zh-CN">
  <voice name="zh-CN-YunxiNeural">
    <prosody rate="-8%" pitch="-2%" volume="0dB">
      <p>春官报春到，福气满门绕。</p>
      <p>一打风调雨顺，二打国泰民安；三打五谷丰登；春牛打得满地转，今年吃穿不用愁。</p>
    </prosody>
  </voice>
</speak>
```

## ElevenLabs (optional)
- Pick a Chinese male voice with baritone timbre; set stability 0.6–0.75, similarity >0.6, style 0.2–0.3, use low clarity boost.
- Keep sample rate 48 kHz for video.

## Usage
- Primary: let Sora synthesize VO using the above profile hints.
- Fallback: render visuals only; synthesize VO via SSML; then mix with the provided SRT timing.

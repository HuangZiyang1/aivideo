# MidJourney Keyframes — Egg Balancing (Equinoctial)

目标：为四段视频提供风格统一的静帧开场/衔接图；保证近午顶光、短直阴影与复古质感一致，便于 Sora 画面硬切对齐。

全局风格与约束（拷贝到每段提示前）
- 复古半写实，哑光材质，暖中性色调，适度去饱和。
- 近午顶光；阴影长度≈1–2 cm，直线、无柔化。
- 桌面木纹细致；时期陶碗、素布；无塑料、无现代标签、无金属高光。
- 三脚架构图稳定；浅景深但接触点/阴影需清晰。
- 避免：文字、水印、运动模糊、镜头变焦、自动构图。

全局 MJ 参数（保持一致）
--ar 16:9 --style raw --v 6 --seed 2424 --chaos 0 --quality 1

— 段 A：准备（鸡蛋与桌面）
Prompt（可直接粘贴）：
"vintage matte tabletop, warm neutral tones, a single plump white egg placed on fine-grain wooden desk, near-noon overhead sun casting short straight shadow 1–2 cm, period ceramic bowl and plain cloth in frame, macro texture clarity, tripod-stable composition, no hands, no text, no plastic --ar 16:9 --style raw --v 6 --seed 2424 --chaos 0 --quality 1"

— 段 B：平衡（支点与微摆）
Prompt（可直接粘贴）：
"balanced egg standing upright with tiny contact patch 3–5 mm visible, short straight shadow 1–2 cm under near-noon overhead light, vintage matte textures, fine wood grain desk, plain cloth, subtle focus on contact area, tripod-stable framing, no motion artifacts, no modern labels --ar 16:9 --style raw --v 6 --seed 2424 --chaos 0 --quality 1"

— 段 C：校验（轻呼气与阴影）
Prompt（可直接粘贴）：
"vintage tabletop scene with balanced egg, near-noon overhead sun, short straight shadow 1–2 cm, a subtle presence of a hand near frame edge implying a soft breath (no blur), plain cloth edge gently lifted, geometry unchanged, warm muted palette, tripod-stable, no text, no plastic --ar 16:9 --style raw --v 6 --seed 2424 --chaos 0 --quality 1"

— 段 D：成功（标记与合影）
Prompt（可直接粘贴）：
"balanced egg beside a small matte paper note with hand-written date, slight paper edge lift ≤3°, near-noon overhead sun casting short straight shadow 1–2 cm, vintage matte textures, warm neutral tones, fine wood grain desk, period ceramic bowl, clean static composition, no modern elements, no text overlay --ar 16:9 --style raw --v 6 --seed 2424 --chaos 0 --quality 1"
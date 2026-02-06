# ClayMotion 阶段3：Veo3 提示词生成

**目标：** 基于阶段2的分镜设计，生成完整的 Veo3 视频提示词。

---

## Veo3 提示词最佳实践

基于 Google Veo3 官方指南和实践经验：

### 核心原则

1. **明确声明风格**: 必须在开头声明 `stop-motion claymation` 或 `needle felting style`
2. **具体描述主体**: 详细描述外观、材质、颜色、状态
3. **使用电影术语**: Veo3 理解专业镜头语言（dolly, tracking, crane 等）
4. **指定镜头角度**: 明确 top-down, side view, close-up 等
5. **描述动态过程**: 起始→变化→结束的完整过程
6. **包含环境氛围**: 光线、色调、背景、情绪

### 提示词结构

```
[风格声明] + [镜头角度] + [场景环境] + [主体描述] + [动态过程] + [镜头运动] + [光影氛围]
```

---

## 风格关键词库

### Style A: 光面黏土风 (Smooth Polymer Clay)

```
Stop-motion claymation animation, smooth polymer clay with glossy surface and subtle fingerprint textures, vibrant saturated colors, cute miniature aesthetic, clean 3D render quality, soft rounded edges
```

### Style B: 暖心毛毡风 (Needle Felting)

```
Stop-motion claymation animation, needle felting style with wool texture and visible fibers, fuzzy surface with loose fibers, soft edges, warm cozy lighting, handcrafted felt aesthetic, fluffy and touchable quality
```

### Style C: 像素怀旧风 (Pixel-Nostalgia)

```
Pixel art animation, retro 16-bit game aesthetic, visible pixel grid with aliased stepped edges and blocky shapes, limited color palette with dithering gradients, crisp pixel-perfect details, nostalgic video game style, versatile scenes including warm cozy interiors panoramic landscapes atmospheric cityscapes and traditional Chinese architecture, adaptable color moods from soft pastels to vibrant saturated to desaturated tones
```

### Style D: 霓虹慢波风 (Neon-Lofi)

```
Detailed digital illustration animation, neon purple magenta and deep blue color scheme with glowing neon signs and screens, lo-fi anime aesthetic with dense intricate details, night or dusk atmosphere with warm interior lights contrasting cool exterior, versatile scenes including cozy gamer rooms Asian city streets at night and minimal calming spaces, cozy yet cyberpunk mood with pink clouds and ambient glow
```

### Style E: 水彩梦境风 (Watercolor-Dream)

```
Watercolor painting animation, visible paper texture with natural pigment bleeding and soft diffused edges, transparent color layering with hand-painted brushstroke quality, atmospheric washes and traditional watercolor technique, versatile scenes including majestic landscapes Studio Ghibli inspired daily life children's book illustration and urban sketching, dreamy and poetic mood with serene innocent and storytelling atmosphere
```

### Style F: 布艺温暖风 (Fabric-Craft)

**完整版关键词：**
```
Stop-motion fabric craft animation, coarse burlap and vintage fabric scraps with patchwork design, woven jute and felt texture, fraying edges and loose threads visible, thick hand stitching and seam details, mismatched button eyes, embroidered facial features, stuffed plushie aesthetic with handmade quality, natural cloth folds and wrinkles, shallow depth of field with soft bokeh background, jerky movement characteristic of stop-motion, 12fps feel, warm color palette with natural fabric tones, gentle diffused lighting with no harsh shadows, cozy comfortable and healing atmosphere, volumetric lighting with dust motes in sunlight, Laika Studios style blend of 3D render with practical effects, characters can be humans animals toys or anthropomorphic creatures
```

**精简版关键词：**
```
Stop-motion fabric craft animation, patchwork burlap and felt texture with visible stitching, fraying edges and loose threads, button eyes and embroidered features, shallow depth of field with bokeh background, jerky stop-motion movement, warm color palette with natural fabric tones, cozy handmade quality
```

**布艺风 Magic Words（Veos3 强化词）：**
- **材质词**: coarse burlap (粗麻布), felt (毛毡), fraying edges (磨损边缘), loose threads (松散线头), patchwork (拼布), woven jute (黄麻编织), thick stitching (粗针脚)
- **摄影词**: macro lens (微距镜头), shallow depth of field (浅景深/背景虚化), bokeh background (焦外背景), tilt-shift (移轴效果 - 玩具感), 85mm lens, f/1.8 aperture
- **动态词**: 12fps (低帧率感), stop-motion (定格), jerky movement (顿挫移动)

---

## 镜头角度关键词

| 角度 | Veo3 关键词 |
|------|------------|
| 正面 | `frontal view`, `facing camera`, `straight-on shot` |
| 侧面 | `side view`, `profile shot`, `lateral angle` |
| 背面 | `from behind`, `rear view`, `over-the-shoulder` |
| 俯视 | `top-down view`, `bird's eye view`, `overhead shot`, `looking down at` |
| 仰视 | `low angle shot`, `looking up at`, `worm's eye view` |
| 特写 | `close-up shot`, `macro shot`, `extreme close-up`, `detail shot` |
| 中景 | `medium shot`, `waist shot`, `mid shot` |
| 远景 | `wide shot`, `establishing shot`, `full shot` |
| 斜角 | `dutch angle`, `tilted frame`, `canted angle` |
| 环绕 | `orbiting shot`, `360 rotation`, `circular tracking` |

---

## 镜头运动关键词

| 运动 | Veo3 关键词 |
|------|------------|
| 静止 | `static camera`, `locked off shot`, `fixed frame` |
| 推近 | `dolly in`, `push forward`, `slow zoom in`, `camera moves closer` |
| 拉远 | `dolly out`, `pull back`, `zoom out`, `camera retreats` |
| 平移 | `pan left`, `pan right`, `horizontal pan` |
| 跟随 | `tracking shot`, `following movement`, `camera follows` |
| 环绕 | `orbiting around`, `circular tracking`, `rotating view` |
| 升起 | `crane up`, `rising shot`, `vertical ascent` |
| 下降 | `crane down`, `descending shot`, `lowering` |

---

## 提示词模板

### 模板 A: 无角色场景（物品/场景主导）

```
[Style], [camera angle] [shot type], [environment description], [main objects with detailed appearance], [object animation: starting state → action → ending state], [camera movement], [lighting and mood], [transition if needed]
```

**示例：**
```
Stop-motion claymation animation, needle felting style with wool texture and visible fibers, top-down view medium shot, on a warm wooden desk surface with soft ambient lighting, several felted banknotes with tiny wings flutter and take flight one by one, flying toward a small sign reading "AI Course ¥3999", a felted wallet in the center gradually deflates and flattens as money escapes, the last banknote hovers momentarily before flying away, static camera with subtle push in at the end, warm golden hour lighting with soft shadows, gentle cozy atmosphere
```

### 模板 B: 有角色场景（角色参与）

```
[Style], [camera angle] [shot type], [environment description], [character detailed appearance from head to toe], [character action and expression: starting → action → ending], [surrounding objects and their states], [camera movement], [lighting and mood]
```

**示例：**
```
Stop-motion claymation animation, needle felting style with fuzzy wool texture, medium shot from slight low angle, in a cozy craft room with warm lighting, a cute felted orange fox character with round black button eyes, wearing a yellow beret and teal sweater, stands next to an ornate treasure chest, the fox reaches out with tiny felted paws and slowly lifts the chest lid, golden light bursts out illuminating the fox's face with wonder, eyes widen and mouth forms an O shape of amazement, glowing cards labeled with tech logos float upward from the chest, camera slowly pushes in toward the treasure, warm magical glow fills the scene
```

### 模板 C: 特写/细节场景

```
[Style], extreme close-up / macro shot, [specific object or detail], [texture and material description], [micro animation or subtle movement], [shallow depth of field], [lighting highlighting texture]
```

**示例：**
```
Stop-motion claymation animation, smooth polymer clay style, extreme close-up shot, a felted finger pressing a glowing "Copy" button, the button depresses with satisfying tactile feedback, multiple document cards instantly duplicate and fan outward from the button, each card has visible paper texture and subtle wobble, shallow depth of field with soft bokeh background, cool blue accent lighting on the button glow, crisp and satisfying micro-animation
```

### 模板 D: 对比/并列场景

```
[Style], [split screen or side-by-side composition], [left side description], [right side description], [contrasting elements], [animation showing difference], [camera movement if any], [lighting emphasizing contrast]
```

**示例：**
```
Stop-motion claymation animation, needle felting style, medium wide shot with split composition, on the left side a stressed felted character surrounded by scattered expensive course materials and depleted wallet, on the right side the same character relaxed and smiling with free resources floating around glowing happily, a dividing line of light separates the two scenes, the contrast emphasizes the transformation, static camera, left side has dim frustrated lighting while right side glows with warm optimistic light
```

### 模板 E: 流程/变化场景

```
[Style], [appropriate angle for showing process], [starting state of scene/objects], [step-by-step transformation description], [ending state], [camera following the process], [lighting shifting with mood]
```

**示例：**
```
Stop-motion claymation animation, polymer clay style with slight sheen, top-down tracking shot, starting with a messy desk covered in scattered notes and question marks, felted hands enter frame and begin organizing, papers transform into neat stacked folders, question marks morph into lightbulb icons one by one, a progress bar made of clay fills from left to right, ending with a perfectly organized workspace with a glowing checkmark appearing, camera slowly tracks across the transformation, lighting gradually brightens from dim confusion to clear productive glow
```

---

## 输出格式

每个场景输出以下内容：

```markdown
## Scene X: [场景标题]

**分镜文案（中文）:**
[原文案，用于配音/字幕]

**视觉描述（中文）:**
[这个画面在展示什么，视觉隐喻说明]

**Veo3 Prompt:**
```
[完整的英文提示词，包含：风格声明 + 镜头角度+景别 + 场景环境 + 主体描述 + 动态过程 + 镜头运动 + 光影氛围]
```

**备注:**
[可选，补充说明，如转场建议等]
```

---

## 完整示例

### Scene 1: 开场 - 别花冤枉钱

**分镜文案（中文）:**
都2026年了，求求你们别再花几千块去报AI速成班了

**视觉描述（中文）:**
俯视桌面场景，钞票长出翅膀飞向"AI速成班"招牌，钱包逐渐瘪掉。无角色，用物品动态表达"浪费金钱"的概念。

**Veo3 Prompt:**
```
Stop-motion claymation animation, needle felting style with wool texture and visible fibers, top-down bird's eye view, on a warm wooden desk with cozy ambient lighting, multiple felted banknotes with tiny embroidered wings begin fluttering and taking flight one by one, they fly in a swirling pattern toward a small felt sign displaying "AI Speed Course ¥3999", a cute round felted wallet in the center of frame gradually deflates like a sad balloon as each note escapes, the wallet's button eyes droop downward in dismay, the last banknote pauses dramatically before joining the others, soft particles trail behind each flying note, static camera with very slow push in during climax, warm golden lighting with gentle shadows, whimsical yet cautionary mood
```

**备注:**
转场建议：溶解到下一场景

---

### Scene 2: 揭示 - 免费渠道

**分镜文案（中文）:**
今天我把官方下场喂饭学AI的免费渠道扒出来

**视觉描述（中文）:**
宝箱打开，金光涌出，带有各大平台Logo的卡片漂浮升起。可选角色（狐狸的手）从画面边缘伸入打开宝箱。

**Veo3 Prompt:**
```
Stop-motion claymation animation, needle felting style with fuzzy texture, medium shot from frontal low angle looking up at treasure, in a cozy dimly lit room, an ornate felted treasure chest with golden trim sits on a wooden pedestal, small felted orange fox paws reach in from the bottom of frame and slowly lift the heavy lid, as the lid opens golden light bursts outward illuminating the scene dramatically, multiple glowing cards rise and float upward from within the chest, each card displays recognizable logos - OpenAI green, Google colors, Microsoft blue - the cards orbit gently in the golden light beam, magical sparkle particles fill the air, camera holds steady then slowly pushes toward the glowing treasure, lighting transitions from dim mysterious to bright magical golden glow, sense of wonder and discovery
```

**备注:**
转场建议：硬切到下一场景

---

### Scene 3: 介绍 - OpenAI Academy

**分镜文案（中文）:**
NO.1 OpenAI Academy，这是ChatGPT的亲妈

**视觉描述（中文）:**
特写展示 OpenAI Logo 卡片，卡片发光旋转展示，背景出现 ChatGPT 气泡图标表示"亲妈"关系。

**Veo3 Prompt:**
```
Stop-motion claymation animation, smooth polymer clay style with slight glossy sheen, close-up shot with shallow depth of field, a beautifully crafted felted card featuring the OpenAI logo in signature green slowly rotates to face camera, the card has embossed text "Academy" below the logo, behind the card a larger translucent ChatGPT speech bubble icon fades into view creating a visual parent-child connection, a thin glowing line connects the card to the bubble icon, the card completes one gentle rotation while hovering, number "1" in gold appears briefly in corner with sparkle, soft gradient background shifting from deep green to light, orbiting camera movement around the card, clean professional lighting with green accent glow, prestigious and authoritative mood
```

**备注:**
转场建议：硬切

---

### Scene 4: 功能 - 提示词库

**分镜文案（中文）:**
官方怕你不会用，直接把压箱底的提示词库都公开了

**视觉描述（中文）:**
俯视桌面，一个保险箱打开，大量提示词卡片飞出散布满桌面。表达"压箱底宝贝公开"的概念。

**Veo3 Prompt:**
```
Stop-motion claymation animation, needle felting style with visible wool fibers, top-down overhead shot, on a warm felt desk surface, a small but heavy-looking felted safe with official OpenAI badge sits closed, the safe door slowly swings open with dramatic weight, immediately dozens of colorful prompt cards explode outward in all directions like confetti, each card has different colored borders and tiny text representing various prompt categories, cards scatter and land across the entire desk surface creating a beautiful spread, some cards spin and flutter as they land, the safe remains open and empty with a satisfied glow inside, static camera capturing the full explosion and settling, bright cheerful lighting with cards casting soft shadows, generous abundant mood
```

**备注:**
转场建议：溶解

---

### Scene 5: 应用 - 各行各业

**分镜文案（中文）:**
各行各业的高质量提示词都能免费获取：市场调研、营销文案、数据分析、品牌叙事

**视觉描述（中文）:**
四个职业/领域图标依次亮起，形成环绕排列。可以有角色在中间旋转指向，也可以纯图标动画。

**Veo3 Prompt:**
```
Stop-motion claymation animation, needle felting style with soft fuzzy texture, medium shot with centered composition, four beautifully crafted felted icons arranged in a circle on a rotating platform: a magnifying glass with chart for Market Research, a pencil with paper for Copywriting, a bar graph with arrow for Data Analysis, a megaphone with heart for Brand Storytelling, each icon lights up sequentially with a soft glow and gentle bounce animation, as each lights up a small label appears below it, the platform slowly rotates to showcase each icon, all four icons pulse together at the end in unified glow, warm ambient lighting with each icon having its own accent color, camera holds centered with subtle breathing movement, professional yet approachable educational mood
```

**备注:**
转场建议：硬切

---

### Scene 6: 行动 - 复制粘贴

**分镜文案（中文）:**
全是现成的，复制粘贴就行

**视觉描述（中文）:**
特写手指点击复制按钮，卡片自动复制并飞入文件夹。表达"简单高效"的概念。

**Veo3 Prompt:**
```
Stop-motion claymation animation, smooth polymer clay style with satisfying tactile quality, extreme close-up shot, a cute felted finger with tiny fingernail detail reaches toward a glowing blue "Copy" button, the finger presses down with satisfying depression animation, instantly a prompt card duplicates itself with a smooth split animation, the copy glows briefly then gracefully arcs through the air, it lands perfectly into an open folder icon with a soft satisfying thud, a small checkmark appears on the folder, the whole action feels effortless and magical, shallow depth of field with soft bokeh, camera follows the card's arc movement, crisp blue accent lighting on interactive elements, efficient and satisfying mood
```

**备注:**
转场建议：淡出

---

## 批量输出格式

当需要快速复制所有提示词时，使用此格式：

```
视频风格：[Style X: xxx风 - 风格描述]

=== SCENE 1: [标题] ===
[文案]
---
[Veo3 Prompt]

=== SCENE 2: [标题] ===
[文案]
---
[Veo3 Prompt]

...
```

---

## 质量检查清单

### 提示词检查
- [ ] 开头声明了风格（stop-motion claymation + 材质）
- [ ] 包含明确的镜头角度
- [ ] 包含景别描述（close-up/medium/wide）
- [ ] 描述了主体的详细外观
- [ ] 包含完整的动态过程（起始→变化→结束）
- [ ] 指定了镜头运动
- [ ] 包含光影和氛围描述
- [ ] 提示词长度 > 200 字符

### 内容检查
- [ ] 视觉隐喻与文案含义匹配
- [ ] 有角色的场景描述了角色外观和动作
- [ ] 无角色的场景用物品/场景动态表达
- [ ] 镜头选择服务于内容表达
- [ ] 整体风格一致

---

**完成本阶段后，用户获得：**
- ✅ 每个分镜的中文文案（用于配音/字幕）
- ✅ 每个分镜的视觉描述（理解画面内容）
- ✅ 完整的 Veo3 英文提示词（包含镜头角度、景别、运动等，可直接复制使用）
- ✅ 转场建议（可选备注）

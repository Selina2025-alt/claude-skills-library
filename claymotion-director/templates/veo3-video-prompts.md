# Google Veo3 视频提示词结构模版

## 用途
为 Google Veo3 视频生成模型提供结构化的提示词模版，确保生成的黏土定格动画视频风格一致、技术参数正确。

---

## Veo3 技术规格

| 参数 | 推荐值 | 说明 |
|------|--------|------|
| **分辨率** | 720P / 1080P | 默认 720P，精细场景用 1080P |
| **时长** | 4s / 6s / 8s | 默认 8s，简单场景 4s |
| **帧率** | 12 fps | 定格动画标准帧率，营造"逐帧"感 |
| **镜头运动** | 缓慢平移 / 固定镜头 | 定格动画特点，避免快速运动 |
| **转场** | 硬切 / 溶解 | 黏土动画常用转场 |

---

## 提示词结构模版

### 基础结构 (适用于所有场景)

```
[风格定义]
Stop-motion claymation animation, [风格材质], 12 fps,

[镜头语言]
[镜头类型 + 景别], [镜头运动],

[场景描述]
[场景环境], [主要角色形象], [次要角色/道具],
[核心动作], [互动关系],

[光影与技术]
[光照描述], [阴影风格], [背景],

[强制约束]
No text overlay, clean background, consistent clay texture throughout,
high quality stop-motion animation, handcrafted details visible

[负面提示]
(worst quality, low quality, blurry), realistic video, 3D CGI,
smooth motion, motion blur, live action footage
```

---

## Style A: Tech-Polymer 完整提示词

### 场景示例 1: 数据处理
```
Stop-motion claymation animation, glossy polymer clay texture with visible fingerprint details, 12 fps,

On a sleek metal laboratory desk with blue LED strips, a small blue polymer clay robot with glowing eyes is processing glowing data streams represented by liquid silver clay ribbons flowing into its chest compartment, the robot's arms move with mechanical precision as it organizes the data,

Sharp directional lighting with cool blue rim light, hard shadows, clean dark gray background with subtle grid pattern,

Medium shot, slight camera pan left,

No text overlay, consistent glossy clay texture, high quality stop-motion animation,

(worst quality, low quality), realistic video, 3D render, smooth motion, motion blur
```

### 场景示例 2: API 连接
```
Stop-motion claymation animation, smooth polymer clay with slight sheen, 12 fps,

Two geometric polymer clay shapes, a blue cube and a purple sphere, magnetically snap together on a minimal white surface, when connected they emit a pulse of light, small glowing particles transfer between them,

Cool-toned lighting with purple accent, soft reflections, white background with grid lines,

Close-up, static camera,

No text overlay, clean clay texture, handcrafted details, stop-motion,

(worst quality), photorealistic, CGI, smooth animation, motion blur
```

---

## Style B: Cozy-Felt 完整提示词

### 场景示例 1: 用户增长
```
Stop-motion claymation animation, fluffy needle-felted wool texture with visible fibers, 12 fps,

On a warm wooden table, a small orange felted character gently places a seed into the soil, a green vine grows upward with new leaves sprouting, each leaf transforms into a small smiling face representing new users,

Soft warm diffused lighting with golden hour tones, soft shadows, cozy living room background with blurred bookshelf,

Medium wide shot, slow upward tilt,

No text overlay, consistent wool felt texture, handcrafted aesthetic, stop-motion animation,

(worst quality, low quality), realistic video, 3D CGI, smooth motion, sharp details, plastic texture
```

### 场景示例 2: 团队协作
```
Stop-motion claymation animation, soft needle-felted wool material, 12 fps,

Three small felted creatures in different colors (blue, pink, yellow) work together to build a tower, they hand each other colorful felted blocks, supporting and encouraging one another with warm gestures,

Warm yellow ambient lighting, soft shadows, bright cheerful background with craft paper texture,

Wide shot, slight camera zoom in,

No text overlay, fluffy felt texture, handmade quality, stop-motion animation,

(worst quality), photorealistic, plastic, clay, smooth animation, motion blur
```

---

## Style C: Pixel-Nostalgia 完整提示词

### 场景示例 1: 温馨室内 (C1)
```
Pixel art animation, 16-bit retro game aesthetic, visible pixel grid with stepped aliased edges,

A cozy living room scene, a cute pixel couple sitting on a brown sofa eating snacks, rain falling outside the window with pixel raindrops, warm orange and pink color palette, coffee table with food items in pixel detail,

Warm indoor lighting with soft pixel gradients using dithering technique, nostalgic comfort atmosphere,

Medium shot, static camera with subtle pixel shimmer effects,

No text overlay, consistent pixel grid throughout, retro game cutscene style,

(worst quality), realistic video, smooth gradients, anti-aliased edges, 3D render
```

### 场景示例 2: 城市风景 (C2)
```
Pixel art animation, 16-bit retro game aesthetic, visible blocky pixel grid,

Panoramic cityscape view with twin towers dominating the skyline, blue ocean in background, scattered buildings in various pixel heights, chunky white clouds in bright blue sky, mountains on the horizon,

Bright saturated colors with clean pixel edges, epic scenic composition like retro game world map,

Wide establishing shot, slow horizontal pan across the city,

No text overlay, detailed architectural pixel work, game map aesthetic,

(worst quality), photorealistic, smooth lines, modern 3D graphics
```

---

## Style D: Neon-Lofi 完整提示词

### 场景示例 1: 游戏房间 (D1)
```
Detailed digital illustration animation, neon purple and hot pink dominant color palette,

Cluttered gamer room corner setup with dual monitors glowing, gaming chair, walls completely covered with anime posters and collectibles, shelves full of figurines and books, plants scattered around, pink and blue RGB lighting mixing with warm desk lamp,

Dense maximalist details with every surface filled, lo-fi anime aesthetic, cozy night atmosphere,

High angle wide shot looking down at the setup, subtle ambient animation like screen flicker and light pulse,

No text overlay, consistent neon color grading throughout,

(worst quality), minimalist, empty spaces, bright daylight, realistic photography
```

### 场景示例 2: 亚洲街头夜景 (D2)
```
Detailed digital illustration animation, neon signs and deep blue night sky with pink clouds,

Small Japanese-style convenience store at street level, old building rising above with multiple floors showing warm lit windows, ivy climbing up the walls with fairy lights, various shop signs in neon colors, air conditioners and wires visible on building exterior, starry night sky,

Warm yellow interior lights contrasting cool blue and purple exterior, lo-fi anime aesthetic, urban exploration mood,

Frontal medium shot of the building facade, gentle animation of lights flickering and stars twinkling,

No text overlay, dense urban details, Asian city atmosphere,

(worst quality), empty scene, daytime, western architecture, minimalist
```

---

## Style E: Watercolor-Dream 完整提示词

### 场景示例 1: 山水风景 (E1)
```
Watercolor painting animation, traditional landscape technique with visible paper texture,

Majestic snow-capped mountain peaks with purple and blue watercolor washes, dark green pine forest in middle ground, peaceful meadow with small stream in foreground, scattered wildflowers, morning mist between mountain layers,

Transparent color layers with deliberate white space for highlights, soft pigment bleeding at edges, atmospheric perspective with distant mountains fading,

Wide establishing shot, static with subtle water ripple animation,

No text overlay, traditional plein air watercolor aesthetic, serene mood,

(worst quality), digital art, sharp edges, photorealistic, oil painting texture
```

### 场景示例 2: 日常生活场景 (E2)
```
Watercolor painting animation, Studio Ghibli inspired warm aesthetic with visible brushstrokes,

Chinese urban street scene, mother holding young daughter's hand at bus stop, orange flowers in wooden planter nearby, summer afternoon with dappled sunlight through trees, bus stop signs showing route numbers, family eating at outdoor table in background,

Soft watercolor washes with warm golden afternoon light, nostalgic daily life atmosphere, gentle storytelling mood,

Medium shot, subtle character movement and leaf animation,

No text overlay, rounded cute character designs, detailed watercolor backgrounds,

(worst quality), anime cel shading, flat digital colors, sharp linework, dark mood
```

### 场景示例 3: 田园绘本风 (E3)
```
Watercolor painting animation, children's book illustration style with generous white space,

Single large tree with lush green foliage dominating the composition, small yellow house with pink roof beneath the tree, open green fields stretching to distant tree line, soft blue sky with light watercolor cloud washes,

Simple composition with delicate brushwork, fresh bright colors, visible watercolor bleeding and paper texture, innocent pure atmosphere,

Wide shot, gentle tree sway and cloud drift animation,

No text overlay, picture book aesthetic, minimal background details,

(worst quality), complex composition, dark colors, realistic rendering, busy background
```

---

## 提示词生成指南

### 步骤 1: 选择风格并填入材质
- **Style A**: `glossy polymer clay texture with visible fingerprint details`
- **Style B**: `fluffy needle-felted wool texture with visible fibers`
- **Style C**: `pixel art, 16-bit retro game aesthetic, visible pixel grid`
- **Style D**: `detailed digital illustration, neon purple and pink, lo-fi anime aesthetic`
- **Style E**: `watercolor painting, visible paper texture, soft diffused edges`

### 步骤 2: 描述场景 (参考 clay-02-storyboard.md 的分镜脚本)
- 场景环境 (实验室/家居/户外)
- 主要角色形象 (参考拟人化映射表)
- 核心动作 (搬运/连接/生长/拥抱等)
- 互动关系 (单人/双人/群体)

### 步骤 3: 定义光影
- **Style A**: `Sharp directional lighting + cool rim light`
- **Style B**: `Soft warm diffused lighting`
- **Style C**: `Pixel color blocks for lighting, dithering gradients`
- **Style D**: `Neon glow effects, warm interior vs cool exterior contrast`
- **Style E**: `Soft atmospheric washes, transparent color layering`

### 步骤 4: 镜头语言
- 镜头类型: `Close-up` / `Medium shot` / `Wide shot`
- 镜头运动: `static` / `pan left` / `slow tilt`
- 时长: `4 seconds` / `6 seconds` / `8 seconds`

### 步骤 5: 强制约束 (必须包含)
```
No text overlay, consistent clay texture, high quality stop-motion animation
```

### 步骤 6: 负面提示 (必须包含)
```
(worst quality, low quality, blurry), realistic video, 3D CGI, smooth motion, motion blur, live action
```

---

## 常见错误避免

| 错误 | 影响 | 解决方案 |
|------|------|----------|
| 忘记 "12 fps" | 失去定格动画感 | 必须在每个提示词开头包含帧率 |
| 使用 "smooth motion" | 变成普通动画 | 加入负面提示 `smooth motion` |
| 风格关键词不足 | 质感不统一 | 每个提示词都要包含完整材质描述 |
| 镜头运动过快 | 不符合定格动画特点 | 使用 `slow`, `gentle`, `slight` 修饰镜头运动 |
| 缺少 "stop-motion" | 模型理解偏差 | 必须在开头明确 "Stop-motion claymation" |

---

## 批量生成工作流

当需要生成多段视频时:

1. **统一风格**: 所有片段使用相同的风格关键词
2. **连贯性**: 保持角色造型、场景环境的一致性
3. **转场规划**: 相邻场景之间考虑色彩/运动的衔接
4. **编号管理**: 使用 `scene_01`, `scene_02` 编号便于后续剪辑

---

## 输出格式

在 `stages/03-generate.md` 中，每个场景的 Veo3 提示词应按以下格式输出:

```markdown
### Scene [编号]: [场景名称]

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

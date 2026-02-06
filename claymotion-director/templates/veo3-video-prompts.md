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

[场景描述]
[场景环境], [主要角色形象], [次要角色/道具],
[核心动作], [互动关系],

[光影与技术]
[光照描述], [阴影风格], [背景],

[镜头语言]
[镜头类型], [镜头运动], [时长],

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

Medium shot, slight camera pan left, 8 seconds,

No text overlay, consistent glossy clay texture, high quality stop-motion animation,

(worst quality, low quality), realistic video, 3D render, smooth motion, motion blur
```

### 场景示例 2: API 连接
```
Stop-motion claymation animation, smooth polymer clay with slight sheen, 12 fps,

Two geometric polymer clay shapes, a blue cube and a purple sphere, magnetically snap together on a minimal white surface, when connected they emit a pulse of light, small glowing particles transfer between them,

Cool-toned lighting with purple accent, soft reflections, white background with grid lines,

Close-up, static camera, 4 seconds,

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

Medium wide shot, slow upward tilt, 6 seconds,

No text overlay, consistent wool felt texture, handcrafted aesthetic, stop-motion animation,

(worst quality, low quality), realistic video, 3D CGI, smooth motion, sharp details, plastic texture
```

### 场景示例 2: 团队协作
```
Stop-motion claymation animation, soft needle-felted wool material, 12 fps,

Three small felted creatures in different colors (blue, pink, yellow) work together to build a tower, they hand each other colorful felted blocks, supporting and encouraging one another with warm gestures,

Warm yellow ambient lighting, soft shadows, bright cheerful background with craft paper texture,

Wide shot, slight camera zoom in, 8 seconds,

No text overlay, fluffy felt texture, handmade quality, stop-motion animation,

(worst quality), photorealistic, plastic, clay, smooth animation, motion blur
```

---

## 提示词生成指南

### 步骤 1: 选择风格并填入材质
- **Style A**: `glossy polymer clay texture with visible fingerprint details`
- **Style B**: `fluffy needle-felted wool texture with visible fibers`

### 步骤 2: 描述场景 (参考 clay-02-storyboard.md 的分镜脚本)
- 场景环境 (实验室/家居/户外)
- 主要角色形象 (参考拟人化映射表)
- 核心动作 (搬运/连接/生长/拥抱等)
- 互动关系 (单人/双人/群体)

### 步骤 3: 定义光影
- **Style A**: `Sharp directional lighting + cool rim light`
- **Style B**: `Soft warm diffused lighting`

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

在 `clay-03-generate.md` 中，每个场景的 Veo3 提示词应按以下格式输出:

```markdown
### Scene [编号]: [场景名称]

**分镜描述**: [来自 clay-02-storyboard.md 的描述]

**Midjourney 提示词**: (用于生成参考图)
```
[prompt content]
```

**Veo3 视频提示词**:
```
[prompt content]
```

**技术参数**:
- 分辨率: 720P / 1080P
- 时长: 4s / 6s / 8s
- 帧率: 12 fps
```

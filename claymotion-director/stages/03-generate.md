# ClayMotion 阶段3：完整提示词生成 (Full Prompt Generation)

**目标：** 为每个分镜生成完整的 Veo3 视频提示词，所有信息（场景/角色/动作/镜头/转场）都融入英文提示词中。

---

## 输入要求

### 来自阶段1的产物
- 风格选择 (Style A 光面黏土风 / Style B 暖心毛毡风)
- 画幅选择 (16:9 / 9:16 / 1:1)
- 隐喻对象映射表

### 来自阶段2的产物
- 完整的分镜脚本 (Scene 1-N)
- 每个分镜的文案 (≤30字)
- 每个场景的详细描述（环境/角色/动作/镜头）

---

## 核心原则

### 提示词结构

每个场景输出**两个部分**：

1. **分镜文案（中文）**: 1-3个短句，≤30字
2. **Veo3 Prompt（英文）**: 完整的视频生成提示词，包含所有信息

### Veo3 提示词结构

```
[风格定义] + [场景描述] + [角色与动作] + [镜头运动] + [转场]
```

**关键要素**：
1. **风格关键词**: 定格动画 + 材质（黏土/毛毡）
2. **场景描述**: 环境、背景、道具
3. **角色形象**: 主角和配角的造型、颜色、状态
4. **核心动作**: 起始→核心→结束的完整过程
5. **镜头运动**: 推/拉/摇/移/跟，快/慢/平滑
6. **转场方式**: 硬切/溶解/匹配剪辑/模糊过渡

### 文字显示规则

**涉及文字的元素使用英文显示**：
- 名字卡片 → `name card with text "xxx"`
- 对话气泡 → `speech bubble with text "xxx"`
- 日历/日期 → `calendar showing date "xxx"`
- 按钮/标签 → `button with label "xxx"`
- 字幕 → `subtitle "xxx"`
- 标志/Logo → 保持原样（OpenAI、Google、edX 等）

---

## 风格关键词库

### Style A: 光面黏土风 (Smooth Polymer Clay)
```
Stop-motion claymation animation, smooth polymer clay style with glossy surface and subtle fingerprints, clean 3d render quality, soft rounded edges, vibrant and fresh colors, cute anthropomorphic characters, miniature set
```

### Style B: 暖心毛毡风 (Needle Felting)
```
Stop-motion claymation animation, needle felting style with wool texture and visible fibers, fuzzy surface, loose fibers, soft edges, warm and cozy lighting, handcrafted felt dolls, stop motion aesthetic, felted fabric background, fluffy and touchable
```

---

## 输出格式

每个场景按以下格式输出：

```markdown
## Scene X: [场景标题]

**分镜文案（中文）：**
[1-3个短句，≤30字]

**Veo3 Prompt (英文):**
```
[风格关键词], [场景描述], [角色形象与动作], [镜头运动], [转场方式]
```
```

---

## 完整示例（暖心毛毡风）

### Scene 1: 开场引入

**分镜文案（中文）：**
说到改名，1月27日

**Veo3 Prompt (英文):**
```
Stop-motion claymation animation, needle felting style with wool texture and visible fibers, on a warm beige wool felt desk with soft cozy lighting, a cute anthropomorphic orange felted fox character with detailed appearance: round orange face with black button eyes and tiny white whisker dots, wearing a yellow felted beret hat with a small pom-pom on top, dressed in a teal blue cozy sweater with white buttons, orange felted hands with tiny claws, sitting cross-legged in front of a miniature computer, the fox turns its head slowly to look directly at the camera with curious expression, a small felted calendar appears in upper right corner showing text "Jan 27", warm golden hour sunlight streaming from upper left creating soft shadows, cozy craft room background with blurred elements, medium shot with static camera, focus on fox's face, hard cut transition
```

### Scene 2: Anthropic 的要求

**分镜文案（中文）：**
Anthropic 说"Clawd"太像，要求改名

**Veo3 Prompt (英文):**
```
Stop-motion claymation animation, needle felting style with wool texture, the same cute orange felted fox sitting at the warm desk looking upward with surprised expression: round eyes widened, mouth slightly open in surprise, wearing the same yellow beret and teal blue sweater, a large blue felted hand reaches slowly from above with visible fiber texture, the hand points with a felted finger at a name card on the desk displaying text "Clawd" in bold felted letters, soft dramatic warm lighting from above creating gentle shadows, handcrafted felt dolls aesthetic, medium shot with slow camera pushing forward to focus on fox's surprised face, dissolve transition
```

---

## 提示词生成指南

### Veo3 提示词完整结构

```
[风格关键词],
[场景环境 + 背景元素],
[角色形象: 从头到脚详细描述],
[核心动作: 起始→中间变化→结束状态，详细动作描述],
[镜头类型 + 运动方式 + 焦点],
[转场方式]
```

**角色形象详细描述要求**（从头到脚）：
- **头部**: 脸型、五官、表情、发型/发饰、帽子/头饰
- **上身**: 上衣类型、颜色、图案、装饰品（项链/胸针等）
- **下身**: 裤子/裙子类型、颜色、长度、腰带
- **鞋子**: 鞋子类型、颜色
- **手持物品**: 手里拿的东西（如果有）
- **动物特色**: 耳朵/尾巴/触角等（如果是动物角色）

**动态描述要求**：
- 细化每个动作步骤，不只说"做某事"
- 描述具体的手部/身体动作
- 描述表情变化
- 描述物体状态变化

### 镜头运动词汇

| 类型 | 英文描述 |
|------|---------|
| 固定 | static camera |
| 推近 | slow camera push forward / camera pushes in |
| 拉远 | camera pulls back / slow pull back |
| 平移 | camera pans left/right |
| 跟随 | camera follows [subject] |
| 上移 | camera moves upward |
| 下移 | camera moves downward |
| 摇摆 | camera swings left and right |

### 转场方式词汇

| 类型 | 英文描述 |
|------|---------|
| 硬切 | hard cut / cut to |
| 溶解 | dissolve / fade to |
| 模糊过渡 | blur transition |
| 匹配剪辑 | match cut |

---

## 批量复制格式

```
# Scene 1: [场景名称] | [分镜文案]
[完整的 Veo3 提示词]

# Scene 2: [场景名称] | [分镜文案]
[完整的 Veo3 提示词]

...
```

---

## 角色形象详细描述模板

### 人物角色（从头到脚）

```
[cute anthropomorphic animal/human character] with detailed appearance:
- Head & Face: [脸型 + 五官 + 表情状态]
- Hair & Accessories: [发型/发色 + 帽子/头饰 + 眼镜/装饰]
- Upper Body: [上衣类型 + 颜色 + 图案 + 扣子/拉链 + 装饰品（项链/胸针等）]
- Lower Body: [裤子/裙子类型 + 颜色 + 长度 + 腰带/口袋]
- Shoes: [鞋子类型 + 颜色 + 款式]
- Held Items: [手里拿的东西，如果有]
- Expression: [当前表情状态]
- Pose: [身体姿态/姿势]
```

### 动物角色（从头到脚）

```
[cute felted animal character] with detailed appearance:
- Head: [动物类型 + 毛绒质感 + 脸型 + 眼睛颜色 + 表情]
- Ears: [耳朵形状 + 位置 + 可动性]
- Body: [身体形状 + 颜色 + 质感 + 大小]
- Limbs: [手臂/腿形状 + 关节可动性 + 爪子/爪子]
- Tail: [尾巴形状 + 长度 + 摆动方式]
- Clothing: [穿着类型 + 颜色 + 配件]
- Accessories: [项圈/领结/背包等装饰]
- Held Items: [手持物品]
- Expression: [表情]
- Pose: [姿态]
```

---

## 动态描述详细模板

```
[核心动作: 起始→中间变化→结束状态，详细动作描述]

起始状态:
- [身体姿态描述]
- [面部表情]
- [物品位置]

中间变化:
- [具体手部动作: 手指如何移动、抓取、释放]
- [身体动作: 转头、弯腰、跳跃、摇摆等]
- [表情变化: 从XX表情变为XX表情]
- [物品状态变化: 移动、变形、出现、消失等]

结束状态:
- [最终定格画面]
- [最终表情]
- [物品最终状态]
```

---

## 质量检查清单

### Veo3 提示词检查
- [ ] 包含完整风格关键词（Style A/B）
- [ ] 场景描述清晰（环境/角色/动作/表情）
- [ ] 光影风格与选定风格一致
- [ ] 包含定格动画相关关键词
- [ ] 镜头运动方式明确
- [ ] 转场方式清晰
- [ ] 涉及文字的部分已标注英文显示
- [ ] 提示词长度 > 300 字符（确保足够详细）

### 一致性检查
- [ ] 同一角色描述一致
- [ ] 场景环境有延续性
- [ ] 风格不混用

---

## 使用建议

1. **直接复制使用**: Veo3 提示词已包含所有必要信息，可直接用于视频生成
2. **先生成 Midjourney 参考图**（可选）: 如果需要确定角色造型，先用简化版提示词生成参考图
3. **批量生成**: 使用批量复制包一次性生成所有场景

---

**完成本阶段后，用户获得：**
- ✅ 每个分镜的文案（≤30字）
- ✅ 完整的英文 Veo3 提示词（可直接使用）
- ✅ 所有信息融入提示词，无需额外中文指导
- ✅ 涉及文字的部分使用英文显示

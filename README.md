# Claude Code Skills 库

这是我的 Claude Code 技能和模板集中管理仓库。

## 📁 目录结构

- **`skills/`** - 通用技能库
  - [帮我写作](skills/帮我写作/) - 结合用户提供的材料进行文案写作
  - [来点选题](skills/来点选题/) - 视频创作选题灵感
  - [英文播客自动总结](skills/英文播客自动总结/) - 一键完成播客抓取、转录和分析
  - [字幕转markdown](skills/字幕转markdown/) - SRT字幕转markdown笔记

- **`templates/`** - 全局项目说明书模板
  - [通用_CLAUDE.md](templates/通用_CLAUDE.md) - 适用于所有项目的全局配置

## 🔄 同步机制

每当创建新 skill 时，Claude 会询问是否保存到此仓库。

**同步流程**：
1. 创建新 skill 后，Claude 询问是否保存到 GitHub
2. 如果确认，复制整个 skill 目录到 `skills/` 文件夹
3. 更新 [skills/README.md](skills/README.md) 添加技能说明
4. 提交到 Git 仓库

## 📝 使用方法

### 添加 Skills 到本地

```bash
# 复制整个 skill 目录到你的 Claude skills 目录
cp -r skills/技能名 "C:\Users\你的用户名\.claude\skills\"
```

### 使用模板

```bash
# 复制模板到新项目
cp templates/通用_CLAUDE.md 你的项目路径/CLAUDE.md
```

---

🤖 *由 Claude Code 自动维护*

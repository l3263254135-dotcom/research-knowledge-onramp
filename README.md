# Research Knowledge Onramp

一个面向 Codex 的研究学习插件，把本地课件、教材、论文、笔记和选题想法整理成可继续学习、复现与开题的研究入口。

插件不仅总结材料，还会区分 `source-backed`、`inference` 和 `to verify`，并在需要时从本科、研究生、博士三个层次解释概念、方法与研究边界。

## 核心输出

- **Research onramp pack**：领域地图、概念关系、方法谱系、数据/任务/指标与阅读顺序。
- **Paper mentor brief**：研究问题、真实创新、证据、假设、基线、局限与后续复现方向。
- **Proposal starter pack**：研究缺口、问题、假设、最小实验、基线、指标、风险与预期贡献。
- **Method boundary card**：方法适用范围、失效场景、比较方式与可能的改进方向。

同时支持课程复习模式，可生成章节讲解、公式含义、计算模板和最后冲刺版。

## 安装

先添加 Git marketplace：

```bash
codex plugin marketplace add l3263254135-dotcom/research-knowledge-onramp
```

再安装插件：

```bash
codex plugin add research-knowledge-onramp@research-knowledge-onramp
```

确认安装状态：

```bash
codex plugin list
```

## 使用示例

安装后可以直接描述任务，也可以明确调用 `research-knowledge-onramp`。

### 从零学习一个领域

```text
使用 research-knowledge-onramp，根据这个文件夹里的课件、教材和论文，
先给我建立研究导向的知识地图。我是零基础，请分别用本科、研究生和博士层次解释，
并明确区分材料直接支持的结论、你的推断和仍需验证的问题。
```

### 导师式带读论文

```text
使用 research-knowledge-onramp，像论文导师一样带我读这篇论文。
不要只做摘要，请分析真实研究问题、创新相对谁成立、证据是否充分、
隐藏假设、关键基线、局限和最值得复现或质疑的实验。
```

### 开题与研究设计

```text
使用 research-knowledge-onramp，把这个想法整理成开题 starter pack：
研究缺口、研究问题、可检验假设、最小可行实验、数据、基线、指标、
失败风险和预期贡献。不要虚构创新点。
```

### 课程复习

```text
使用 research-knowledge-onramp，根据本地 PPT 和教材按老师的章节顺序复习。
先建立课程地图，再详细解释知识点、公式和计算步骤，最后给出考试冲刺版。
```

## 更新与卸载

刷新 marketplace：

```bash
codex plugin marketplace upgrade research-knowledge-onramp
```

如需重新安装：

```bash
codex plugin remove research-knowledge-onramp@research-knowledge-onramp
codex plugin add research-knowledge-onramp@research-knowledge-onramp
```

## 本地开发与验证

验证 skill：

```bash
python3 ~/.codex/skills/.system/skill-creator/scripts/quick_validate.py \
  plugins/research-knowledge-onramp/skills/research-knowledge-onramp
```

验证 plugin：

```bash
python3 ~/.codex/skills/.system/plugin-creator/scripts/validate_plugin.py \
  plugins/research-knowledge-onramp
```

本地添加当前仓库作为 marketplace：

```bash
codex plugin marketplace add .
codex plugin add research-knowledge-onramp@research-knowledge-onramp
```

## 项目结构

```text
.
├── .agents/plugins/marketplace.json
├── plugins/research-knowledge-onramp/
│   ├── .codex-plugin/plugin.json
│   └── skills/research-knowledge-onramp/
│       ├── SKILL.md
│       ├── agents/openai.yaml
│       └── references/
├── LICENSE
└── README.md
```

## License

[MIT](LICENSE)

# Learning Skills

两个配合使用的中文学习 Skill：先理解真实改动，再将选定的知识点整理成独立 Demo。

| Skill | 作用 | 默认流程 |
| --- | --- | --- |
| [restudy](skills/restudy/SKILL.md) | 根据真实代码进行个人学习复盘 | 梳理改动 → 列大纲并等待确认 → 每次讲一个主题并等待继续 → 结束 |
| [发布垃圾 / publish-laji](skills/publish-laji/SKILL.md) | 将知识点提炼成独立 Demo 并发布 | 确定知识点 → 实现 Demo → 编写 README → 发布 GitHub |

## 使用示例

```text
用 $restudy 复盘这次功能改动，先列大纲。
```

确认大纲后，使用“开始”“继续”，或直接追问当前知识点。restudy 默认按一个主题一轮的节奏讲解，解释完用户选定的内容即结束。

```text
用 $publish-laji 把刚才的缓存失效知识点做成独立 Demo，写 README 并发布到我的 GitHub。
```

发布 Skill 会沿用已确认的仓库和授权；缺少目标仓库或必要权限时，说明缺少的信息。普通复盘不会自动触发发布。

## 安装到 Codex

下载或克隆本仓库，将 `skills/restudy` 和 `skills/publish-laji` 两个目录分别复制到个人 skills 目录：

- 默认目录：`~/.codex/skills/`。
- 已设置 `CODEX_HOME` 时，使用其下的 `skills/` 目录。
- 目录已存在时，先保留本地定制内容，再决定如何合并；特别注意个人学习档案。

也可以让 Codex 使用 `$skill-installer`，从本仓库的 `skills/restudy` 与 `skills/publish-laji` 路径安装。安装完成后，在后续对话中调用对应 Skill。

```text
用 $skill-installer 从 GitHub 仓库 bruceoxygenrain/learning-skills 安装 skills/restudy 和 skills/publish-laji。
```

## 个性化 restudy

公开版的 [learner-profile.md](skills/restudy/references/learner-profile.md) 是空白模板，不包含作者的个人学习档案或历史会话。安装后可以在本地填写讲解偏好、相关知识点的当前理解情况和证据日期。

将“接触过”“能解释”“能实现”“能迁移排错”分开记录。仅把档案用于调整讲解起点，不用它给学习者贴固定标签。当前用户指示与新反馈优先。

[teaching-example.md](skills/restudy/references/teaching-example.md) 提供一个虚构场景的大纲与单步讲解示例，用于说明节奏和深度，不代表任何真实项目结论。

## 仓库结构

```text
skills/
├── restudy/
│   ├── SKILL.md
│   ├── agents/openai.yaml
│   └── references/
│       ├── learner-profile.md
│       └── teaching-example.md
└── publish-laji/
    ├── SKILL.md
    └── agents/openai.yaml
```

## 验证与使用边界

本版本尚未运行 Skill 校验脚本，也未进行实际调用验证。两个 Skill 默认沿用原作者的协作分工：界面、样式和入口由使用者手动验证，构建、类型检查、lint 和代码检查由使用者另行安排；使用者的明确指示优先。

制作公开 Demo 时使用演示数据和配置示例，不上传私有项目源码、真实凭据或个人学习记录。

# Hi, I'm Wang Xinming 👋

**Student at Qilu University of Technology · AI applications & open-source contributions**

我关注大模型应用、AI Agent、MCP 与 RAG，喜欢从具体问题出发，通过复现、修复和回归测试改进软件的可靠性与兼容性。

## Open-source contributions

以下 PR 均已合并到对应项目的上游仓库。

| Project | Contribution | Merged |
| --- | --- | --- |
| [Windows-MCP](https://github.com/CursorTouch/Windows-MCP) | 为 UI 自动化树遍历增加路径级 RuntimeId 循环检测，避免重复祖先节点导致无限递归，同时保留兄弟分支的正常遍历。 [#429](https://github.com/CursorTouch/Windows-MCP/pull/429) | 2026-09-27 |
| [TraceMemo](https://github.com/Wxw-Gu/TraceMemo) | 合并 Query Agent 的连续 system messages，在保留会话范围语义的同时改善严格 OpenAI 兼容服务端的请求兼容性。 [#45](https://github.com/Wxw-Gu/TraceMemo/pull/45) | 2026-09-20 |
| [wmux](https://github.com/openwong2kim/wmux) | 修复 Windows 下 Ctrl+Shift+[ / ] 的标签切换快捷键，兼容 Shift 后上报为 { / } 的键值，并补充回归测试。 [#1424](https://github.com/openwong2kim/wmux/pull/1424) | 2026-09-18 |

[View all merged pull requests →](https://github.com/pulls?q=is%3Apr+author%3Ammhh256+is%3Amerged)

## Projects

| Project | What it does | Stack |
| --- | --- | --- |
| [llm-chat](https://github.com/mmhh256/llm-chat) | AI 聊天应用，支持多会话、流式响应、Markdown、代码高亮及文件预览。 | Vue 3 · Vite · Pinia · Element Plus |
| [weather-viz](https://github.com/mmhh256/weather-viz) | 天气可视化应用，支持城市搜索、实时天气、温度趋势、7 天预报和 Mock 数据模式。 | Vue 3 · TypeScript · Express · ECharts |

## Currently exploring

- **AI applications** — 流式交互、模型 API 兼容性与知识检索。
- **Agent & MCP** — 工具调用、桌面自动化与可靠的执行流程。
- **Engineering practice** — 问题复现、边界条件处理与回归测试。

### In progress

[DeerFlow #7185](https://github.com/bytedance/deer-flow/pull/7185) — 为端口等待脚本增加超时参数校验，避免非法输入导致持续等待。**Draft / 待审阅，尚未合并。**

---

欢迎围绕具体问题和项目交流。


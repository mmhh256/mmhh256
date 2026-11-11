# Wang Xinming · @mmhh256

齐鲁工业大学学生，关注 AI 应用、Agent 工程、MCP 与 RAG。

我喜欢从可复现的问题入手，给检索、模型调用和 Agent 运行时补齐边界条件与回归测试。

## 开源贡献

在 **6 个上游项目**有 **9 个公开 PR 已合并**。下面按项目整理了具体改动。

**WeKnora · 文档解析与 RAG 检索**

- [#4705](https://github.com/Tencent/WeKnora/pull/4705) 为含 EMF/WMF 矢量图的 PPTX 接回 docreader 的栅格化流程，使图片可用于浏览器展示与多模态索引。
- [#4584](https://github.com/Tencent/WeKnora/pull/4584) 将长文档的向量生成与写入改为分窗口处理，限制索引过程中同时留在内存里的新生成向量。
- [#4521](https://github.com/Tencent/WeKnora/pull/4521) 保留重排输入中代码块的原文，避免清洗误删 XML、URL 和运算符。
- [#4701](https://github.com/Tencent/WeKnora/pull/4701) 按服务端实际输出解释重排分数配置，避免把已经归一化的概率再次做 sigmoid。

**Agent 运行时、模型兼容性与桌面工具**

- **Octop** · 将记忆采集与召回注入的开关传递到运行时，保留显式关闭和独立配置。[#2296](https://github.com/TencentCloud/Octop/pull/2296)
- **DeerFlow** · 让沙箱的多个挂载路径复用一个用户数据 PVC 声明，保留各自的子路径与只读配置。[#7274](https://github.com/bytedance/deer-flow/pull/7274)
- **Windows-MCP** · 在当前 UI 自动化树路径上检测重复的 RuntimeId，避免无限递归，同时保留兄弟分支的遍历。[#429](https://github.com/CursorTouch/Windows-MCP/pull/429)
- **TraceMemo** · 合并 Query Agent 的连续系统消息，在保留会话范围的同时兼容对消息顺序要求严格的模型服务。[#45](https://github.com/Wxw-Gu/TraceMemo/pull/45)
- **wmux** · 用物理按键码识别 Windows 上的括号组合键，修复 Ctrl+Shift+[ / ] 切换标签页的行为。[#1424](https://github.com/openwong2kim/wmux/pull/1424)

## 项目

- **[knowflow-rag](https://github.com/mmhh256/knowflow-rag)** · 面向校园学习资料的 RAG 问答项目，包含文档管理与会话界面。Next.js · TypeScript · LangGraph · LanceDB · Prisma
- **[自托管数字员工平台](https://github.com/mmhh256/self-hosted-digital-workforce-platform)** · 基于 [Miniclaw](https://github.com/helsome/miniclaw) 的项目群协同方案，围绕群内唤起 Agent、项目资料查询、会议纪要和事项跟进组织工作。
- **[llm-chat](https://github.com/mmhh256/llm-chat)** · 支持多会话和流式输出的 AI 聊天应用，提供 Markdown 渲染、代码高亮、附件预览和本地会话历史。Vue 3 · Vite · Pinia · Element Plus
- **[weather-viz](https://github.com/mmhh256/weather-viz)** · 支持城市搜索、24 小时温度趋势和 7 天预报的天气可视化应用，可在和风天气 API 与本地 Mock 数据之间切换。Vue 3 · TypeScript · Express · ECharts
- **[interview-prep](https://github.com/mmhh256/interview-prep)** · 面向 AI 应用与 Agent 岗位的面试准备 Skill，沿项目源码核对简历描述和调用链，并据此设计追问与模拟面试。

另有一份 [Craft Agents 源码仓库](https://github.com/mmhh256/craft-agents)，原项目由 [Craft 团队](https://github.com/craft-ai-agents/craft-agents-oss) 开源。

## 其他公开 PR

<details>
<summary>进行中 · 9 个</summary>

- **FastGPT** · 在调用工具前拒绝因输出 token 上限被截断的参数，避免 JSON 修复后执行不完整的工具调用。[#8332](https://github.com/labring/FastGPT/pull/8332)
- **Hy-Memory** · 在桌面端重新连接已有运行时后保留其临时进程标记，使退出时可以正确停止该进程。[#272](https://github.com/Tencent-Hunyuan/Hy-Memory/pull/272)
- **Hy-Memory** · 给暂停的任务设置下次可领取时间，减少队列反复领取和释放同一任务的空转。[#271](https://github.com/Tencent-Hunyuan/Hy-Memory/pull/271)
- **Hy-Memory** · 逐条识别事实的语言，改善混有命令或路径的中文技术内容的提示词选择。[#269](https://github.com/Tencent-Hunyuan/Hy-Memory/pull/269)
- **DeerFlow** · 在端口探测开始前校验端口与超时参数，避免无效输入导致脚本一直等待。[#7185](https://github.com/bytedance/deer-flow/pull/7185)
- **pg-aiguide** · 更新 PostgreSQL 分批回填示例，按实际选中的主键推进检查点，避免主键稀疏或已有回填数据时提前退出。[#161](https://github.com/timescale/pg-aiguide/pull/161)
- **LiveKit Agents** · 让会话的结果标签、状态与失败原因保持一致，避免遥测报告错误的结果。[#7491](https://github.com/livekit/agents/pull/7491)
- **LobeHub** · 在 CLI 中区分等待人工审批、等待异步工具和任务完成。[#19810](https://github.com/lobehub/lobehub/pull/19810)
- **codex-acp** · 为 WSL 挂载的 Windows 路径采用不区分大小写的匹配，同时保留普通 Linux 路径的行为。[#526](https://github.com/agentclientprotocol/codex-acp/pull/526)

</details>

<details>
<summary>已关闭 · 未合并 · 5 个</summary>

- **Octop** · 为 macOS 用户级 LaunchAgent 补充 Apple Silicon 与 Intel 的 Homebrew 路径，帮助后台服务找到 adb 等工具。[#2883](https://github.com/TencentCloud/Octop/pull/2883)
- **FastGPT** · 提议在循环节点内支持并行节点，并处理嵌套后的画布移动、折叠与变量引用。[#8121](https://github.com/labring/FastGPT/pull/8121)
- **FastGPT** · 让全文、语义与混合召回结果保留文档片段的索引字段，供下游工作流直接使用。[#8073](https://github.com/labring/FastGPT/pull/8073)
- **DeerFlow** · 为腾讯 WSA 搜索接入原生异步 HTTP 调用，避免慢请求长时间占用默认线程池的工作线程。[#7192](https://github.com/bytedance/deer-flow/pull/7192)
- **txtai** · 让稀疏索引的 k-means 训练实际采用配置的特征数，未配置时沿用全维训练。[#1260](https://github.com/neuml/txtai/pull/1260)

</details>

[查看 GitHub 上的全部公开 PR](https://github.com/pulls?q=is%3Apr+author%3Ammhh256+is%3Apublic) · 状态核对于 2026-11-11

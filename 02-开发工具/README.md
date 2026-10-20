# 02-开发工具

让 agent 跑起来的骨架、模型网关、浏览器自动化、代码理解与记忆。共 **25** 个仓库。

覆盖分类：Agent 运行时 / 编排、代码理解 / 知识图谱、模型网关 / 推理基建、浏览器 / 桌面自动化、记忆 / 上下文管理

| 仓库 | 用途 | 标签 | ★ | 建议 |
|---|---|---|---:|---|
| [morluto/rea](https://github.com/morluto/rea) | 用 agent 做逆向：从应用行为一路拆到原生二进制 | `CLI` | 337,300 | 待定 |
| [deepseek-ai/deepseek-harness](https://github.com/deepseek-ai/deepseek-harness) | DeepSeek 官方 harness，一切皆插件；你本机的 dsh 就是它 | `CLI` `已装` | 254,522 | 保留 |
| [Graphify-Labs/graphify](https://github.com/Graphify-Labs/graphify) | 把代码库连同文档、SQL、配置、PDF 一起转成可查询的知识库 | `CLI` `重复` | 129,198 | 待定 |
| [browser-use/browser-use](https://github.com/browser-use/browser-use) | Python 里最主流的 AI 浏览器代理库，让 agent 操作网页 | `库` | 118,550 | 保留 |
| [thedotmack/claude-mem](https://github.com/thedotmack/claude-mem) | 跨会话持久记忆，把 agent 干过的事抓下来下次接着用 | `插件` | 101,817 | 保留 |
| [Panniantong/Agent-Reach](https://github.com/Panniantong/Agent-Reach) | 给 agent 装眼睛：读 Twitter、Reddit、YouTube 等内容源 | `库` | 99,730 | 待定 |
| [rtk-ai/rtk](https://github.com/rtk-ai/rtk) | Rust CLI 代理，把常见开发命令的输出压缩，省 60-90% 的 token | `CLI` | 83,988 | 保留 |
| [colbymchenry/codegraph](https://github.com/colbymchenry/codegraph) | 预索引的代码知识图谱，代码改动后自动同步，供多种编码 agent 使用 | `插件` `重复` | 74,465 | 待定 |
| [multica-ai/multica](https://github.com/multica-ai/multica) | 人和 AI agent 当一支队伍协作，可自托管 | `库` | 53,234 | 待定 |
| [QuantumNous/new-api](https://github.com/QuantumNous/new-api) | 把各家大模型聚合成统一 OpenAI 接口再分发，自建网关首选 | `Web` | 50,279 | 保留 |
| [abhigyanpatwari/GitNexus](https://github.com/abhigyanpatwari/GitNexus) | 零服务器的代码智能引擎，本地建索引不依赖后端 | `Web` `重复` | 47,955 | 待定 |
| [vercel-labs/agent-browser](https://github.com/vercel-labs/agent-browser) | Vercel 出的浏览器自动化 CLI，给 agent 用；你本机已有同名 skill 封装 | `CLI` `已装` | 44,268 | 保留 |
| [codewhale-hq/Codewhale](https://github.com/codewhale-hq/Codewhale) | Rust 写的 agent 引擎 + 终端客户端，可换模型供应商 | `CLI` | 41,106 | 待定 |
| [tirth8205/code-review-graph](https://github.com/tirth8205/code-review-graph) | 本地优先的代码智能图，走 MCP/CLI，用于代码评审时给足上下文 | `MCP` `重复` | 32,264 | 待定 |
| [alibaba/page-agent](https://github.com/alibaba/page-agent) | 阿里出的「页面内」GUI agent，注入网页用自然语言操作界面 | `库` | 29,514 | 待定 |
| [yamadashy/repomix](https://github.com/yamadashy/repomix) | 把整个仓库打包成一个 AI 友好的单文件，提问前先喂给它 | `CLI` | 28,914 | 保留 |
| [jarrodwatts/claude-hud](https://github.com/jarrodwatts/claude-hud) | Claude Code 插件，实时显示上下文占用、在跑的工具、后台任务 | `插件` | 28,657 | 保留 |
| [yetone/magpie](https://github.com/yetone/magpie) | 菜单栏里做模型路由：Codex 接 DeepSeek、Claude Code 接 Kimi，你之前研究过 | `桌面端` | 17,065 | 保留 |
| [mindfold-ai/Trellis](https://github.com/mindfold-ai/Trellis) | 自称「最好的 agent harness」，管工具与上下文的运行骨架 | `CLI` | 14,982 | 待定 |
| [CursorTouch/Windows-MCP](https://github.com/CursorTouch/Windows-MCP) | 让 MCP 客户端直接操作 Windows 桌面（点击、输入、截图） | `MCP` | 9,583 | 待定 |
| [iflytek/astron-agent](https://github.com/iflytek/astron-agent) | 科大讯飞的企业级 agent 工作流平台，Java 技术栈、偏商用私有化 | `库` | 8,916 | 待定 |
| [xiaotianfotos/homerail](https://github.com/xiaotianfotos/homerail) | 语音优先的本地 agent 编排，跑可审计的 DAG 工作流 | `库` `低星` | 996 | 可取消 |
| [EvovexAI/EvoFlow](https://github.com/EvovexAI/EvoFlow) | 原生 agent runtime：智能体员工、编排、知识库、长任务 | `桌面端` `中文` `低星` | 483 | 可取消 |
| [fancy1108/Clutch](https://github.com/fancy1108/Clutch) | Tauri + LangGraph 的本地多智能体桌面应用，作者个人项目 | `桌面端` `低星` | 90 | 可取消 |
| [AtreideJZ/personalized-llm-wiki](https://github.com/AtreideJZ/personalized-llm-wiki) | 按 Karpathy 的 LLM-Wiki 概念初始化一套个人知识库 | `教程` `低星` | 2 | 可取消 |

---

[← 返回索引](../README.md) · [标签索引](../TAGS.md)

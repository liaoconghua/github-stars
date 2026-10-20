# GitHub Stars 整理看板

把 `liaoconghua` 的 83 个 GitHub star 逐个归类，并为每个仓库写了一句中文的「这玩意儿是干啥的」。

**在线查看**：`https://liaoconghua.github.io/github-stars/`（Pages 开启后生效）

---

## 文件说明

| 文件 | 用途 |
|---|---|
| `index.html` | 整理看板。可按用途筛选、按关键词搜索，含收藏节奏与语言分布图表 |
| `stars.csv` | 同一份数据的表格版，Excel 可直接打开，适合排序和二次处理 |

打开 `index.html` 即可，无需联网（字体走 CDN，离线时回退系统字体）。搜索框按 `/` 聚焦，`Esc` 清空。

---

## 核心结论

### 1. 收藏高度集中在最近半年

83 个收藏里 **80 个是 2026 年 5 月之后收的**，几乎没有沉淀期。「记不住是干啥的」是囤积的必然结果，不是记性问题。

### 2. 真正的问题是同质内容重复囤

| 重复簇 | 收了几份 | 实际关系 |
|---|---|---|
| Agent Skills 合集 | 5+ | `agency-agents` 与 `agency-agents-zh` 是同一项目的中英文版；`awesome-claude-code` 与 `awesome-claude-code-subagents` 是索引与其子集 |
| 代码知识图谱 | 4+1 | `graphify`／`codegraph`／`GitNexus`／`code-review-graph` 是同赛道四个竞品，另加轻量版 `repomix` |
| Agent 运行时 | 6 | 其中 3 个星数不足 1000，属早期个人项目 |

同一生态位收 4–5 份，大脑无法为每个分配记忆位置。

### 3. 判读结果

- **保留 22**：值得长期留着
- **待定 45**：需要实际用一次再决定
- **可取消 16**：重复、或信息不足难以判断

判读依据是重复度、成熟度（星数、描述完整度）以及本地已安装组件，不是对项目本身的客观评价。取消 star 不影响项目本身。

---

## 建议的整理方式

GitHub 原生 Lists 比平铺的星标好用得多。建议分 5 组：

| 列表 | 内容 | 数量 |
|---|---|---|
| `01-Agent技能` | 技能包与专家视角蒸馏 | 19 |
| `02-开发工具` | 运行时、网关、自动化、代码理解 | 25 |
| `03-内容生产` | 写作、设计、影音处理 | 14 |
| `04-业务系统` | 后端自托管与自媒体运营 | 12 |
| `05-学习生活` | 教材课程与杂项 | 13 |

---

## 如何更新

数据来自 GitHub 公开 REST API，重新生成即可：

1. 拉取最新 stars（`per_page=100` 单页即可覆盖）：
   ```bash
   curl -H "Accept: application/vnd.github.star+json" \
     "https://api.github.com/users/liaoconghua/starred?per_page=100&page=1" \
     -o stars_raw.json
   ```
2. 修改生成脚本里的 `META` 字典（新增仓库需补一条中文用途说明）
3. 重跑生成器，覆盖 `index.html` 与 `stars.csv`

> 生成器不随仓库分发，保存在本地工作区。判定标准：新增收藏后如果不能一句话说清它解决什么具体问题，就不要收。

---

## 数据快照

- 抓取时间：2026-10-20
- 来源：`GET /users/liaoconghua/starred`（公开数据，无需鉴权）
- ★ 数为抓取时的快照值

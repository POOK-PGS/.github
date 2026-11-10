# POOK PGS · 企业智能增长系统

> **POOK Growth System（PGS）** — 企业智能增长系统与组织智能工作系统。
> 把经营信号、资料与人员授权关联到同一事项，让 Agent 在证据与审批的边界内协同执行。

中文 · [English Summary](#english-summary)

## 概述

POOK PGS 覆盖企业经营场景的**产品面 + 基础设施 + 行业应用**：从官网、账号、控制台，到 Agent 控制面、企业 AI 网关、质量与数据基础设施，再到增长、关系、HR、舆情等经营模块。

我们坚持四条工程底线：

- **证据优先**：每个结论可追溯到代码、测试输出、扫描结果或引用来源；不以信心代替证据。
- **人在环内**：Agent 起草与执行，人负责审批与签收；LLM 输出不能授权、计薪或付款。
- **规格即契约**：UI 以像素级规格为唯一真源；数字从常量来，一切文本转义。
- **可验收交付**：全量 CI 验证、发布证据与运行手册随交付走，未执行的用例不宣称通过。

## 项目版图

| 领域 | 仓库 | 说明 |
| --- | --- | --- |
| 产品 | `PGS-OS` | 组织智能工作系统：官网 · 账号 · 控制台 · Kernel · DEMO 后端 · 部署单元 |
| 产品 | `pgs-soar` | PGS 凌云：有依据、可跟进的企业个人工作台与受控 Agent 执行内核 |
| Agent 控制面 | `pgs-infra-a2a` | PGS Agent OS：案卷、A2A 协作、证据、审批与持久执行的集团控制面 |
| 基础设施 | `pgs-infra-api` | 集团企业 AI 网关：模型接入、项目授权、预算预占、用量账本（sub2api 内核 · Go + Vue） |
| 基础设施 | `pgs-infra-codereviewer` | 代码与能力质量控制面：固定 SHA 审查、Capability Studio、确定性内核与交付证据 |
| 基础设施 | `pgs-infra-data` | Agent-native 可信数据源运行时：授权采集、证据保全、可信度评分、知识包 |
| 经营应用 | `pgs-growpilot-agent-mcn` | GrowPilot：小红书经营实验的企业级 Agent 控制内核（GrowthRun · Android Fleet · 证据链） |
| 经营应用 | `pgs-infra-growpilot` | 企业 AI 关系基础设施：WeCom 优先、租户隔离、人工复核的 Agent |
| 经营应用 | `pgs-infra-geo` | 品牌 GEO 经营闭环：目标、证据、干预、归因、ROI |
| 经营应用 | `pgs-infra-hr` | AI HR：本地工作台、在线底稿、请假审批与桌面交付工程 |
| 经营应用 | `pgs-insight` | PGS Insight（Sentinelle 哨兵）：多品牌舆情清洗、AI 分析与报告生成 |
| 已归档 | `pgs-device-gateway` | 历史源码保留；活跃设备运行时已并入 `pgs-infra-a2a` |

> 部分仓库当前为私有，组织成员可见。

## 技术栈

TypeScript monorepo（Node 24/26 · esbuild · Playwright）· Go + Vue（AI 网关）· Python · PostgreSQL 17 · Next.js / Vercel · Cloudflare Workers · Docker / Kubernetes / Helm · GitHub Actions

<a name="english-summary"></a>

## English Summary

**POOK PGS (POOK Growth System)** — an enterprise growth system and organizational intelligent workspace. Product surfaces (website, accounts, console, Kernel-backed workspace), an Agent OS control plane (cases, A2A collaboration, evidence, approvals, durable execution), an enterprise AI gateway (model access, project authorization, budget reservation, usage ledger), quality and data infrastructure, and industry growth applications (social-commerce pilots, CRM relations, GEO attribution, HR workbench, sentiment insight).

Engineering principles: evidence over confidence; humans approve and sign off while agents draft and execute; specs are the single source of truth for the UI; every delivery ships with verifiable evidence — unexecuted cases are never claimed as passed.

Some repositories are currently private and visible to organization members.

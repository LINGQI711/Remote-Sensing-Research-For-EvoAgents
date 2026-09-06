# RS Skills & Evolution

遥感智能体、技能表示、工具探索与自进化研究文献库。

**9 篇论文 · 2025–2026 · Private 私有仓库**

参考 [Remote Sensing Research for Disasters](https://github.com/LINGQI711/Remote-Sensing-Research-for-Disasters) 的组织方式，按年份列出论文、发表场所、内容简介与资源链接，并提供主题索引及 PDF 归档。

## 归档规则

- 已核实会议接收的论文按会议年份归档；其余按首次预印本年份归档，标注 `arXiv preprint`。未核实录用不代表被拒稿。
- 发表信息核对日期：**2026-09-06**。证据来自 arXiv 元数据、论文首页及作者公开资源；投稿声明、模板样式和参考文献中的会议名称不作为录用证据。
- PDF 保留本地提供版本；最新网页可能对应更新稿。每篇条目注明本地版本，摘要也以本地文件为基础。
- 仅收录经选择的公开论文 PDF；不纳入未公开稿件、个人研究笔记、代码项目或压缩包。仓库应持续保持 Private。

## Papers

[2026](#2026) · [2025](#2025) · [主题索引](#主题索引)

### 2026

- **HiRS-Agent: A Hierarchical Multi-Agent System for Reliable Long-Horizon Remote Sensing Task Solving** — **ACM Multimedia 2026（已接收）** [[arXiv](https://arxiv.org/abs/2608.30672)] [[PDF](papers/2026/ACM-MM/HiRS-Agent%20-%20A%20Hierarchical%20Multi-Agent%20System%20for%20Reliable%20Long-Horizon%20Remote%20Sensing%20Task%20Solving.pdf)] [[作者资源](https://github.com/IntelliSensing/HiRS-Agent)]
  - **遥感多智能体与可靠执行**：以 Manager–Specialist 两层结构组织长流程遥感任务：管理层负责路由、逐步验证和重规划，专家层调用领域工具；结合监督微调和分层强化学习提升执行可靠性。
  - 版本：[v1](https://arxiv.org/abs/2608.30672v1)。arXiv Comments 明确标注 ACM Multimedia 2026 接收；本地首页包含会议与 DOI。

- **XSkill: Continual Learning from Experience and Skills in Multimodal Agents** — **ICML 2026（已接收）** [[arXiv](https://arxiv.org/abs/2603.12056)] [[PDF](papers/2026/ICML/XSkill%20-%20Continual%20Learning%20from%20Experience%20and%20Skills%20in%20Multimodal%20Agents.pdf)] [[作者资源](https://github.com/XSkill-Agent/XSkill)]
  - **经验与技能持续学习**：将任务级技能与动作级经验作为两条互补知识流，从多模态执行轨迹中提炼、合并、检索并适配，在不更新模型参数的情况下持续改善工具使用与任务规划。
  - 版本：[v2](https://arxiv.org/abs/2603.12056v2)。arXiv 最新版本 Comments 与作者代码仓库均确认 ICML 2026 接收；本地 PDF 为早期预印本 v2。

- **GeoForge: Non-Parametric Self-Evolving Agents for Earth-Observation Reasoning** — **arXiv preprint 2026** [[arXiv](https://arxiv.org/abs/2608.10494)] [[PDF](papers/2026/arXiv/GeoForge%20-%20Non-Parametric%20Self-Evolving%20Agents%20for%20Earth-Observation%20Reasoning.pdf)]
  - **地球观测非参数自进化**：将已完成轨迹沉淀为工作流图记忆、动作级经验和适配的技能 SOP；按传感上下文约束工具空间，并通过带安全门控的蒸馏实现执行知识积累与复用。
  - 版本：[v1](https://arxiv.org/abs/2608.10494v1)。未核实正式会议或期刊录用。

- **MMSkills: Towards Multimodal Skills for General Visual Agents** — **arXiv preprint 2026** [[arXiv](https://arxiv.org/abs/2605.13527)] [[PDF](papers/2026/arXiv/MMSkills%20-%20Towards%20Multimodal%20Skills%20for%20General%20Visual%20Agents.pdf)] [[作者资源](https://github.com/DeepExperience/MMSkills)]
  - **多模态技能表示与调用**：将文本步骤、运行时状态卡和视觉关键帧组成可复用技能包；从公开交互轨迹生成技能，并在临时分支中查阅视觉证据，向主智能体返回与当前状态匹配的操作指导。
  - 版本：[v3](https://arxiv.org/abs/2605.13527v3)。未核实正式会议或期刊录用；简介对应本地 PDF。

- **OpenEarth-Agent: From Tool Calling to Tool Creation for Open-Environment Earth Observation** — **arXiv preprint 2026** [[arXiv](https://arxiv.org/abs/2603.22148)] [[PDF](papers/2026/arXiv/OpenEarth-Agent%20-%20From%20Tool%20Calling%20to%20Tool%20Creation%20for%20Open-Environment%20Earth%20Observation.pdf)] [[作者资源](https://github.com/walking-shadow/OpenEarth-Agent)]
  - **开放环境工具创建**：针对未见过的数据和任务动态规划工作流并创建专用工具，支持跨领域地球观测全流程；提出 OpenEarth-Bench，评估开放环境下的适应规划与工具创建能力。
  - 版本：[v1](https://arxiv.org/abs/2603.22148v1)。未核实正式会议或期刊录用。

- **RS-Claw: Progressive Active Tool Exploration via Hierarchical Skill Trees for Remote Sensing Agents** — **arXiv preprint 2026** [[arXiv](https://arxiv.org/abs/2605.13391)] [[PDF](papers/2026/arXiv/RS-Claw%20-%20Progressive%20Active%20Tool%20Exploration%20via%20Hierarchical%20Skill%20Trees%20for%20Remote%20Sensing%20Agents.pdf)]
  - **分层技能树与主动工具探索**：把工具描述组织成分层技能树，先读取摘要选择分支，再按需加载细节并调用工具；缓解全量注册的上下文负担及检索遗漏，在 Earth-Bench 上验证长流程工具选择。
  - 版本：[v1](https://arxiv.org/abs/2605.13391v1)。本地首页仅写明 submitted to IEEE，不能据此认定已被 IEEE 期刊录用。

- **SkillsBench: Benchmarking How Well Agent Skills Work Across Diverse Tasks** — **arXiv preprint 2026** [[arXiv](https://arxiv.org/abs/2602.12670)] [[PDF](papers/2026/arXiv/SkillsBench%20-%20Benchmarking%20How%20Well%20Agent%20Skills%20Work%20Across%20Diverse%20Tasks.pdf)] [[作者资源](https://www.skillsbench.ai/)]
  - **技能效果评测基准**：通过任务、技能包与确定性验证器比较无技能、人工整理技能及自生成技能等设置，研究技能的收益、负迁移与文档粒度；为遥感技能评测提供通用实验设计参考。
  - 版本：[v3](https://arxiv.org/abs/2602.12670v3)。未核实正式会议或期刊录用。本地为 v3；在线已有 v4，任务数量与统计结果有变化，未替换本地文件。

### 2025

- **GeoEvolve: Automating Geospatial Model Discovery via Multi-Agent Large Language Models** — **arXiv preprint 2025** [[arXiv](https://arxiv.org/abs/2509.21593)] [[PDF](papers/2025/arXiv/GeoEvolve%20-%20Automating%20Geospatial%20Model%20Discovery%20via%20Multi-Agent%20Large%20Language%20Models.pdf)]
  - **地理空间算法自动发现**：使用多智能体与嵌套进化循环自动生成、修改和评估地理空间算法，结合 GeoKnowRAG 注入领域理论；在空间插值与地理空间保形预测任务上研究知识引导的模型发现。
  - 版本：[v1](https://arxiv.org/abs/2509.21593v1)。未核实正式会议或期刊录用；公开投稿版本不作为会议接收证据。

- **RingMo-Agent: A Unified Remote Sensing Foundation Model for Multi-Platform and Multi-Modal Reasoning** — **arXiv preprint 2025** [[arXiv](https://arxiv.org/abs/2507.20776)] [[PDF](papers/2025/arXiv/RingMo-Agent%20-%20A%20Unified%20Remote%20Sensing%20Foundation%20Model%20for%20Multi-Platform%20and%20Multi-Modal%20Reasoning.pdf)]
  - **多平台多模态遥感基础模型**：基于 RS-VL3M 图文数据，结合模态自适应表示和任务专用 token，统一卫星与无人机平台上光学、SAR、红外影像的感知与推理；主要作为基础模型方向参考。
  - 版本：[v2](https://arxiv.org/abs/2507.20776v2)。按首次预印本年份 2025 归档；本地 v2 修订于 2026-01-05，在线已有 v3。未核实正式会议或期刊录用。

## 主题索引

| 研究方向 | 代表论文 | 可关注的问题 |
| --- | --- | --- |
| 遥感工具选择与长流程执行 | RS-Claw、HiRS-Agent、OpenEarth-Agent | 如何选择、验证、重规划或动态创建工具 |
| 技能、经验与非参数自进化 | XSkill、GeoForge | 如何提炼轨迹、积累知识并在后续任务中复用 |
| 多模态技能表示 | MMSkills、XSkill | 如何把视觉状态与可执行步骤关联 |
| 技能评测与消融 | SkillsBench | 如何比较无技能、整理技能与生成技能，识别收益和负迁移 |
| 地理空间模型发现 | GeoEvolve | 如何用地理知识引导代码进化与算法搜索 |
| 遥感多模态基础模型 | RingMo-Agent | 如何统一跨平台、跨传感模态的感知与推理 |

同一论文可以对应多个主题。XSkill、MMSkills、SkillsBench 是通用智能体方法或评测参考；RingMo-Agent 侧重基础模型，不等同于外部工具编排系统。

## 文件组织

```text
papers/
  2026/
    ACM-MM/     # HiRS-Agent
    ICML/       # XSkill
    arXiv/      # 5 篇预印本
  2025/
    arXiv/      # GeoEvolve、RingMo-Agent
metadata.json   # 题目、年份、发表场所、摘要、链接、版本与 SHA-256
```

PDF 按完整论文名命名。文件散列记录在 [metadata.json](metadata.json)，用于核对上传副本与本地文件一致性。`.gitignore` 采用文件白名单；新增论文需先核实可收录范围，再明确添加允许路径。

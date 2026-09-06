# Remote-Sensing-Research-For-EvoAgents

Papers and reading notes on remote sensing agents and reusable agent skills.

The collection contains **30 papers**: **18** in remote sensing and **12** in general-purpose skills, workflows, and experience learning. Each paper has an English note covering the problem, method, experiments, and conclusions.

- [Part I: Remote Sensing Agents](#part-i-remote-sensing-agents)
- [Part II: General-Purpose Skills](#part-ii-general-purpose-skills)
- [Reading Notes](notes/README.md)

## Part I: Remote Sensing Agents

Tool-using systems, multi-agent collaboration, agent training, memory evolution, and evaluation. GeoEvolve and RingMo-Agent are included as supporting work on algorithm and foundation-model evolution.

### 2026

| Paper | Venue | Focus | Links |
| --- | --- | --- | --- |
| **Earth-Agent** — Earth-Agent: Unlocking the Full Landscape of Earth Observation with Agents | ICLR 2026 | Multimodal Earth observation tools and evaluation | [PDF](papers/remote-sensing/2026/ICLR/Earth-Agent%20-%20Unlocking%20the%20Full%20Landscape%20of%20Earth%20Observation%20with%20Agents.pdf) · [Notes](notes/remote-sensing/Earth-Agent.md) · [arXiv](https://arxiv.org/abs/2509.23141) · [Publication](https://openreview.net/forum?id=dkIXAbWuxO) |
| **GeoEvolver** — Experience-Driven Multi-Agent Systems Are Training-free Context-aware Earth Observers | arXiv preprint | Experience-driven exploration and memory | [PDF](papers/remote-sensing/2026/arXiv/Experience-Driven%20Multi-Agent%20Systems%20Are%20Training-free%20Context-aware%20Earth%20Observers.pdf) · [Notes](notes/remote-sensing/GeoEvolver.md) · [arXiv](https://arxiv.org/abs/2602.02559) |
| **GeoForge** — GeoForge: Non-Parametric Self-Evolving Agents for Earth-Observation Reasoning | arXiv preprint 2026 | Non-parametric evolution for Earth observation | [PDF](papers/remote-sensing/2026/arXiv/GeoForge%20-%20Non-Parametric%20Self-Evolving%20Agents%20for%20Earth-Observation%20Reasoning.pdf) · [Notes](notes/remote-sensing/GeoForge.md) · [arXiv](https://arxiv.org/abs/2608.10494) |
| **GeoMMAgent** — GeoMMBench and GeoMMAgent: Toward Expert-Level Multimodal Intelligence in Geoscience and Remote Sensing | CVPR 2026 (Highlight) | Expert multimodal geoscience reasoning | [PDF](papers/remote-sensing/2026/CVPR/GeoMMBench%20and%20GeoMMAgent%20-%20Toward%20Expert-Level%20Multimodal%20Intelligence%20in%20Geoscience%20and%20Remote%20Sensing.pdf) · [Notes](notes/remote-sensing/GeoMMAgent.md) · [arXiv](https://arxiv.org/abs/2604.08896) · [Publication](https://openaccess.thecvf.com/content/CVPR2026/papers/Xiao_GeoMMBench_and_GeoMMAgent_Toward_Expert-Level_Multimodal_Intelligence_in_Geoscience_and_CVPR_2026_paper.pdf) · [Project](https://github.com/Shihao-Cheng/GeoMMAgent) |
| **HiRS-Agent** — HiRS-Agent: A Hierarchical Multi-Agent System for Reliable Long-Horizon Remote Sensing Task Solving | ACM Multimedia 2026 (accepted) | Hierarchical remote sensing agents and reliable execution | [PDF](papers/remote-sensing/2026/ACM-MM/HiRS-Agent%20-%20A%20Hierarchical%20Multi-Agent%20System%20for%20Reliable%20Long-Horizon%20Remote%20Sensing%20Task%20Solving.pdf) · [Notes](notes/remote-sensing/HiRS-Agent.md) · [arXiv](https://arxiv.org/abs/2608.30672) · [Project](https://github.com/IntelliSensing/HiRS-Agent) |
| **OpenEarth-Agent** — OpenEarth-Agent: From Tool Calling to Tool Creation for Open-Environment Earth Observation | arXiv preprint 2026 | Tool creation for open-environment Earth observation | [PDF](papers/remote-sensing/2026/arXiv/OpenEarth-Agent%20-%20From%20Tool%20Calling%20to%20Tool%20Creation%20for%20Open-Environment%20Earth%20Observation.pdf) · [Notes](notes/remote-sensing/OpenEarth-Agent.md) · [arXiv](https://arxiv.org/abs/2603.22148) · [Project](https://github.com/walking-shadow/OpenEarth-Agent) |
| **OpenEarthAgent** — OpenEarthAgent: A Unified Framework for Tool-Augmented Geospatial Agents | arXiv preprint | Training compact geospatial tool-using agents | [PDF](papers/remote-sensing/2026/arXiv/OpenEarthAgent%20-%20A%20Unified%20Framework%20for%20Tool-Augmented%20Geospatial%20Agents.pdf) · [Notes](notes/remote-sensing/OpenEarthAgent.md) · [arXiv](https://arxiv.org/abs/2602.17665) · [Project](https://mbzuai-oryx.github.io/OpenEarthAgent/) |
| **RemoteAgent** — RemoteAgent: Bridging Vague Human Intents and Earth Observation with RL-based Agentic MLLMs | arXiv preprint | Resolving vague intents with reinforcement learning | [PDF](papers/remote-sensing/2026/arXiv/RemoteAgent%20-%20Bridging%20Vague%20Human%20Intents%20and%20Earth%20Observation%20with%20RL-based%20Agentic%20MLLMs.pdf) · [Notes](notes/remote-sensing/RemoteAgent.md) · [arXiv](https://arxiv.org/abs/2604.07765) |
| **RS-Agent** — RS-Agent: Automating Remote Sensing Tasks through Intelligent Agent | Science China Information Sciences | Domain knowledge and remote sensing tool orchestration | [PDF](papers/remote-sensing/2026/SCIS/RS-Agent%20-%20Automating%20Remote%20Sensing%20Tasks%20through%20Intelligent%20Agent.pdf) · [Notes](notes/remote-sensing/RS-Agent.md) · [arXiv](https://arxiv.org/abs/2406.07089) · [Publication](https://doi.org/10.1007/s11432-026-5026-5) · [Project](https://github.com/IntelliSensing/RS-Agent) |
| **RS-Claw** — RS-Claw: Progressive Active Tool Exploration via Hierarchical Skill Trees for Remote Sensing Agents | arXiv preprint 2026 | Hierarchical skills and active tool exploration | [PDF](papers/remote-sensing/2026/arXiv/RS-Claw%20-%20Progressive%20Active%20Tool%20Exploration%20via%20Hierarchical%20Skill%20Trees%20for%20Remote%20Sensing%20Agents.pdf) · [Notes](notes/remote-sensing/RS-Claw.md) · [arXiv](https://arxiv.org/abs/2605.13391) |
| **RSMeM** — RSMeM: Knowledge-Enhanced Memory Evolution for Remote Sensing Agents with Systematic Evaluation | ACL 2026 | Knowledge-guided memory evolution | [PDF](papers/remote-sensing/2026/ACL/RSMeM%20-%20Knowledge-Enhanced%20Memory%20Evolution%20for%20Remote%20Sensing%20Agents%20with%20Systematic%20Evaluation.pdf) · [Notes](notes/remote-sensing/RSMeM.md) · [arXiv](https://arxiv.org/abs/2607.24772) · [Publication](https://aclanthology.org/2026.acl-long.1519/) |

### 2025

| Paper | Venue | Focus | Links |
| --- | --- | --- | --- |
| **GeoEvolve** — GeoEvolve: Automating Geospatial Model Discovery via Multi-Agent Large Language Models | arXiv preprint 2025 | Automated geospatial algorithm discovery | [PDF](papers/remote-sensing/2025/arXiv/GeoEvolve%20-%20Automating%20Geospatial%20Model%20Discovery%20via%20Multi-Agent%20Large%20Language%20Models.pdf) · [Notes](notes/remote-sensing/GeoEvolve.md) · [arXiv](https://arxiv.org/abs/2509.21593) |
| **GeoLLM-Squad** — Multi-Agent Geospatial Copilots for Remote Sensing Workflows | IGARSS 2025 | Specialist collaboration and workflow memory | [PDF](papers/remote-sensing/2025/IGARSS/Multi-Agent%20Geospatial%20Copilots%20for%20Remote%20Sensing%20Workflows.pdf) · [Notes](notes/remote-sensing/Multi-Agent-Geospatial-Copilots.md) · [arXiv](https://arxiv.org/abs/2501.16254) · [Publication](https://www.2025.ieeeigarss.org/view_paper.php?PaperNum=5591&SessionID=1614) |
| **RingMo-Agent** — RingMo-Agent: A Unified Remote Sensing Foundation Model for Multi-Platform and Multi-Modal Reasoning | arXiv preprint 2025 | Multi-platform, multi-modal remote sensing foundation models | [PDF](papers/remote-sensing/2025/arXiv/RingMo-Agent%20-%20A%20Unified%20Remote%20Sensing%20Foundation%20Model%20for%20Multi-Platform%20and%20Multi-Modal%20Reasoning.pdf) · [Notes](notes/remote-sensing/RingMo-Agent.md) · [arXiv](https://arxiv.org/abs/2507.20776) |
| **ThinkGeo** — ThinkGeo: Evaluating Tool-Augmented Agents for Remote Sensing Tasks | arXiv preprint | Step-level evaluation of remote sensing tool use | [PDF](papers/remote-sensing/2025/arXiv/ThinkGeo%20-%20Evaluating%20Tool-Augmented%20Agents%20for%20Remote%20Sensing%20Tasks.pdf) · [Notes](notes/remote-sensing/ThinkGeo.md) · [arXiv](https://arxiv.org/abs/2505.23752) |

### 2024

| Paper | Venue | Focus | Links |
| --- | --- | --- | --- |
| **Change-Agent** — Change-Agent: Towards Interactive Comprehensive Remote Sensing Change Interpretation and Analysis | IEEE Transactions on Geoscience and Remote Sensing | Interactive change detection and description | [PDF](papers/remote-sensing/2024/IEEE-TGRS/Change-Agent%20-%20Towards%20Interactive%20Comprehensive%20Remote%20Sensing%20Change%20Interpretation%20and%20Analysis.pdf) · [Notes](notes/remote-sensing/Change-Agent.md) · [arXiv](https://arxiv.org/abs/2403.19646) · [Publication](https://doi.org/10.1109/TGRS.2024.3425815) · [Project](https://github.com/Chen-Yang-Liu/Change-Agent) |
| **GeoLLM-Engine** — GeoLLM-Engine: A Realistic Environment for Building Geospatial Copilots | CVPR 2024 Workshops · EarthVision | Executable environments for geospatial copilots | [PDF](papers/remote-sensing/2024/CVPR-Workshops/GeoLLM-Engine%20-%20A%20Realistic%20Environment%20for%20Building%20Geospatial%20Copilots.pdf) · [Notes](notes/remote-sensing/GeoLLM-Engine.md) · [arXiv](https://arxiv.org/abs/2404.15500) · [Publication](https://openaccess.thecvf.com/content/CVPR2024W/EarthVision/html/Singh_GeoLLM-Engine_A_Realistic_Environment_for_Building_Geospatial_Copilots_CVPRW_2024_paper.html) |
| **RS-ChatGPT** — Remote Sensing ChatGPT: Solving Remote Sensing Tasks with ChatGPT and Visual Models | IGARSS 2024 | Language-driven orchestration of visual models | [PDF](papers/remote-sensing/2024/IGARSS/Remote%20Sensing%20ChatGPT%20-%20Solving%20Remote%20Sensing%20Tasks%20with%20ChatGPT%20and%20Visual%20Models.pdf) · [Notes](notes/remote-sensing/Remote-Sensing-ChatGPT.md) · [arXiv](https://arxiv.org/abs/2401.09083) · [Publication](https://doi.org/10.1109/IGARSS53475.2024.10640736) · [Project](https://github.com/HaonanGuo/Remote-Sensing-ChatGPT) |

## Part II: General-Purpose Skills

Skill extraction, validation, routing, executable libraries, workflow memory, and experience learning.

### 2026

| Paper | Venue | Focus | Links |
| --- | --- | --- | --- |
| **EvoSkill** — EvoSkill: Automated Skill Discovery for Multi-Agent Systems | arXiv preprint | Validated iterative skill discovery | [PDF](papers/general-skills/2026/arXiv/EvoSkill%20-%20Automated%20Skill%20Discovery%20for%20Multi-Agent%20Systems.pdf) · [Notes](notes/general-skills/EvoSkill.md) · [arXiv](https://arxiv.org/abs/2603.02766) · [Project](https://github.com/sentient-agi/EvoSkill) |
| **MemSkill** — MemSkill: Learning and Evolving Memory Skills for Self-Evolving Agents | arXiv preprint | Learning and evolving memory operations | [PDF](papers/general-skills/2026/arXiv/MemSkill%20-%20Learning%20and%20Evolving%20Memory%20Skills%20for%20Self-Evolving%20Agents.pdf) · [Notes](notes/general-skills/MemSkill.md) · [arXiv](https://arxiv.org/abs/2602.02474) · [Project](https://github.com/ViktorAxelsen/MemSkill) |
| **MMSkills** — MMSkills: Towards Multimodal Skills for General Visual Agents | arXiv preprint 2026 | Multimodal skill representation and runtime consultation | [PDF](papers/general-skills/2026/arXiv/MMSkills%20-%20Towards%20Multimodal%20Skills%20for%20General%20Visual%20Agents.pdf) · [Notes](notes/general-skills/MMSkills.md) · [arXiv](https://arxiv.org/abs/2605.13527) · [Project](https://github.com/DeepExperience/MMSkills) |
| **SkillCAT** — SkillCAT: Contrastive, Assessment-Augmented and Topology-Aware Skill Self-Evolution for LLM Agents | arXiv preprint | Contrastive extraction, patch assessment, and skill routing | [PDF](papers/general-skills/2026/arXiv/SkillCAT%20-%20Contrastive%2C%20Assessment-Augmented%20and%20Topology-Aware%20Skill%20Self-Evolution%20for%20LLM%20Agents.pdf) · [Notes](notes/general-skills/SkillCAT.md) · [arXiv](https://arxiv.org/abs/2606.13317) |
| **SkillOpt** — SkillOpt: Executive Strategy for Self-Evolving Agent Skills | arXiv preprint | Controlled optimization of textual agent skills | [PDF](papers/general-skills/2026/arXiv/SkillOpt%20-%20Executive%20Strategy%20for%20Self-Evolving%20Agent%20Skills.pdf) · [Notes](notes/general-skills/SkillOpt.md) · [arXiv](https://arxiv.org/abs/2605.23904) · [Project](https://github.com/microsoft/SkillOpt) |
| **SkillsBench** — SkillsBench: Benchmarking How Well Agent Skills Work Across Diverse Tasks | arXiv preprint 2026 | Benchmarking the effectiveness of agent skills | [PDF](papers/general-skills/2026/arXiv/SkillsBench%20-%20Benchmarking%20How%20Well%20Agent%20Skills%20Work%20Across%20Diverse%20Tasks.pdf) · [Notes](notes/general-skills/SkillsBench.md) · [arXiv](https://arxiv.org/abs/2602.12670) · [Project](https://www.skillsbench.ai/) |
| **Trace2Skill** — Trace2Skill: Distill Trajectory-Local Lessons into Transferable Agent Skills | arXiv preprint | Distilling portable skills from execution traces | [PDF](papers/general-skills/2026/arXiv/Trace2Skill%20-%20Distill%20Trajectory-Local%20Lessons%20into%20Transferable%20Agent%20Skills.pdf) · [Notes](notes/general-skills/Trace2Skill.md) · [arXiv](https://arxiv.org/abs/2603.25158) · [Project](https://github.com/Qwen-Applications/Trace2Skill) |
| **XSkill** — XSkill: Continual Learning from Experience and Skills in Multimodal Agents | ICML 2026 (accepted) | Continual learning from experiences and skills | [PDF](papers/general-skills/2026/ICML/XSkill%20-%20Continual%20Learning%20from%20Experience%20and%20Skills%20in%20Multimodal%20Agents.pdf) · [Notes](notes/general-skills/XSkill.md) · [arXiv](https://arxiv.org/abs/2603.12056) · [Project](https://github.com/XSkill-Agent/XSkill) |

### 2025

| Paper | Venue | Focus | Links |
| --- | --- | --- | --- |
| **AWM** — Agent Workflow Memory | ICML 2025 | Reusable workflow memory for web agents | [PDF](papers/general-skills/2025/ICML/Agent%20Workflow%20Memory.pdf) · [Notes](notes/general-skills/AWM.md) · [arXiv](https://arxiv.org/abs/2409.07429) · [Publication](https://proceedings.mlr.press/v267/wang25bx.html) · [Project](https://github.com/zorazrw/agent-workflow-memory) |
| **SkillWeaver** — SkillWeaver: Web Agents can Self-Improve by Discovering and Honing Skills | arXiv preprint | Discovering and refining callable web skills | [PDF](papers/general-skills/2025/arXiv/SkillWeaver%20-%20Web%20Agents%20can%20Self-Improve%20by%20Discovering%20and%20Honing%20Skills.pdf) · [Notes](notes/general-skills/SkillWeaver.md) · [arXiv](https://arxiv.org/abs/2504.07079) · [Project](https://github.com/OSU-NLP-Group/SkillWeaver) |

### 2024

| Paper | Venue | Focus | Links |
| --- | --- | --- | --- |
| **ExpeL** — ExpeL: LLM Agents Are Experiential Learners | AAAI 2024 | Natural-language lessons and experience retrieval | [PDF](papers/general-skills/2024/AAAI/ExpeL%20-%20LLM%20Agents%20Are%20Experiential%20Learners.pdf) · [Notes](notes/general-skills/ExpeL.md) · [arXiv](https://arxiv.org/abs/2308.10144) · [Publication](https://ojs.aaai.org/index.php/AAAI/article/view/29936) |
| **Voyager** — Voyager: An Open-Ended Embodied Agent with Large Language Models | Transactions on Machine Learning Research | Executable skill libraries and automatic curricula | [PDF](papers/general-skills/2024/TMLR/Voyager%20-%20An%20Open-Ended%20Embodied%20Agent%20with%20Large%20Language%20Models.pdf) · [Notes](notes/general-skills/Voyager.md) · [arXiv](https://arxiv.org/abs/2305.16291) · [Publication](https://openreview.net/forum?id=ehfRiF0R3a) · [Project](https://voyager.minedojo.org) |

# Phase 2 — Existing Solutions Research

> 状态：进行中
>
> 目标：研究现有方法、产品、开源项目与实际工作流，回答：
>
> 1. 别人已经解决了哪些部分？
> 2. 哪些长期存在的问题仍没有被很好解决？
> 3. 哪些机制值得进入后续 Product Directions，哪些不值得？

## 1. 研究框架

Phase 2 不按“App 类型”分类，而优先按 Phase 1 的五层能力链做映射：

> 知道 → 想到 → 用出来 → 被纠正 → 迁移与内化

研究对象至少覆盖：

- mental models learning
- decision journal
- reflective practice
- deliberate practice
- case-based learning / problem-based learning
- Socratic tutoring
- spaced repetition / retrieval practice
- knowledge management
- AI tutor
- critical thinking training
- decision-making training
- 开源项目 / GitHub
- 社区个人工作流

## 2. 第一轮研究发现

### 2.1 Spaced Repetition / Retrieval Practice

代表：
- Anki / FSRS
- Obsidian Spaced Repetition
- FSRS4Anki

主要解决：
- 知道
- 记忆保持
- 部分迁移

证据：
- Retrieval practice 的 meta-analysis 显示测试式学习不仅有助于记忆，也能产生一定的迁移效应，但迁移强弱高度取决于测试形式、应用/推理任务设计等。

初步判断：
- SRS 擅长“记住模型”，但不等于“会在现实问题中主动调用”。
- 如果把模型训练直接做成卡片，可能会把“思考能力”降维成“术语记忆”。
- 因此 spaced repetition 更可能是辅助机制，而不是产品主轴。

### 2.2 Deliberate Practice

核心机制：
- 明确技能目标
- 有难度的针对性任务
- 重复练习
- 反馈
- 修正

研究显示：
- deliberate practice 与表现有关，但不能被神化为解释一切的单一机制；
- 在需要具体技能训练的领域，结构化练习 + 反馈通常有效。

初步判断：
- 与 Phase 1 的“用了但不知道自己用得对不对”高度相关。
- 但思维模型不像运动技能那样容易定义唯一正确动作，因此“反馈标准”会比传统 deliberate practice 更难。

### 2.3 Case-Based Learning / Problem-Based Learning

核心机制：
- 从真实或近真实问题出发；
- 在不完整、复杂、甚至模糊的情境中分析；
- 让学习者自己发现信息需求；
- 教师/导师主要提供引导和反馈。

研究信号：
- PBL/CBL 对技能、长期知识保持与知识应用有积极证据；
- 不同问题类型需要不同案例设计；
- “一个统一案例模板”并不适合所有训练目标。

初步判断：
- 与我们的目标高度相关，尤其覆盖“想到 → 用出来 → 迁移”。
- 这也支持 Phase 1 的一个结论：不同思维模型可能需要不同类型的训练任务，而不是统一题型。

### 2.4 Reflective Practice / Reflective Writing

核心机制：
- 保存当时的判断；
- 事后重新观察；
- 区分当时知道什么、后来才知道什么；
- 从经验中形成下一次可调用的认识。

研究信号：
- 系统综述中，reflective practice 与反思、决策、问题解决、critical thinking 等能力提升相关。

初步判断：
- 很适合“被纠正 → 内化”；
- 但单纯写反思容易变成叙事性日记，缺少结构化校正。

### 2.5 Decision Journal

代表：
- Farnam Street Decision Journal
- 若干开源 decision-journal 项目

典型机制：
- 决策发生时记录背景、假设、理由和信心；
- 结果出现后复盘；
- 尝试区分判断质量与运气；
- 防止 hindsight bias。

值得注意的开源案例：
- 有项目明确提出“预尸检必须自己写，AI 应在用户先思考之后补盲区”；
- 有项目强调不可修改的原始决策日志，再叠加后续反思。

初步判断：
- 很强于“被纠正”和长期校准；
- 但通常假设用户已经知道如何分析问题，并不负责系统训练模型调用和多模型联动。

### 2.6 Critical Thinking / Decision Training

代表：
- Clearer Thinking

当前可见模块包括：
- 校准判断
- sunk cost
- Bayes
- Explanation Freeze
- Fail-Safing
- Decision Advisor
- Mental Traps

初步判断：
- 说明“认知偏差 + 决策训练 + 小型互动工具”已经是成熟方向；
- 优点是具体、可操作；
- 但训练往往被拆成很多独立工具/课程，是否能形成长期迁移和统一个人模型体系仍需继续研究。

### 2.7 Socratic Tutoring / AI Tutor

研究信号：
- 2025 年对 ChatGPT 与人工导师的研究表明，AI 的优势包括可访问性、非评判性和随时可用；人工导师在个性化反馈、信任、复杂理解等方面仍有优势。
- 近期研究和 study protocol 越来越强调 AI 不应直接代替思考，而应通过提问、scaffolding 和 iterative reflection 支持推理。
- 同时存在明确风险：AI 可能给出“听起来很合理但其实错误”的反馈，或导致认知外包。

初步判断：
- AI 很适合承担挑战者、反馈者、反例生成器、盲区提示者；
- 但把 AI 设成“真理裁判”风险很高。
- 这与 Phase 1 的担忧完全一致。

## 3. 第一轮能力覆盖矩阵

| 方法 / 产品类型 | 知道 | 想到 | 用出来 | 被纠正 | 迁移内化 |
|---|---|---|---|---|---|
| SRS / Anki | 强 | 弱 | 弱 | 弱 | 中 |
| Mental Model Library | 强 | 弱-中 | 弱 | 弱 | 弱 |
| Case / PBL | 中 | 强 | 强 | 中-强 | 强 |
| Deliberate Practice | 中 | 中 | 强 | 强 | 中-强 |
| Reflective Practice | 弱 | 弱 | 中 | 强 | 中-强 |
| Decision Journal | 弱 | 中 | 中 | 强 | 中 |
| Critical Thinking Tools | 中 | 中 | 中-强 | 中 | 中 |
| Socratic AI Tutor | 中 | 强 | 强 | 强但有可靠性风险 | 尚不确定 |

> 这是 Phase 2 的暂定分析，不是最终结论。

## 4. 当前最重要的早期发现

1. 现有成熟方法往往只解决五层链路的一部分。
2. “记住模型”与“现实调用”之间确实存在明显断层。
3. Case/PBL + deliberate practice + feedback 与目标的契合度目前明显高于纯知识库/SRS。
4. Decision Journal 很适合长期校准，但它通常发生在“已经做出判断”之后。
5. AI 可以提供高频反馈，但“AI 反馈是否可信”本身必须成为产品风险，而不能默认成立。
6. 不同思维模型可能需要不同训练任务；统一模板存在把训练做僵的风险。

## 5. 下一轮研究

下一轮继续深入：

- mental model learning 的成熟产品与课程
- decision journal 的真实长期使用工作流
- metacognition / transfer / analogical reasoning
- cognitive flexibility
- argumentation training
- forecasting / calibration training
- 社区中的个人思考系统
- AI tutor 防止认知外包的设计
- 是否存在真正覆盖“现实问题 → 多模型调用 → 反馈 → 长期复盘”的产品

最终 Phase 2 要形成：
- Existing Solutions Map
- Mechanism Map
- Coverage Gaps
- Unsolved Problems
- 可进入 Phase 3 的独立产品方向输入

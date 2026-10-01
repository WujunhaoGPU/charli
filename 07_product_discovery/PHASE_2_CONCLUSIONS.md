# Phase 2 — Existing Solutions Research: Conclusions

> 项目：个人长期使用的「思维模型 / 思考训练软件」
>
> 状态：Phase 2 收束
>
> 本文不是产品方案，而是对现有方法、产品、研究和开源项目的阶段性结论。它的作用是为 Phase 3 — Independent Product Directions 提供边界和约束。

## 1. Phase 2 的核心问题

Phase 2 不是为了“找一个产品抄”，而是回答三个问题：

1. 现有方法已经解决了哪些部分？
2. 哪些问题长期没有被很好解决？
3. 如果我们要做新产品，它到底必须比现有工具组合多解决什么？

研究始终围绕 Phase 1 的五层能力链：

> 知道 → 想到 → 用出来 → 被纠正 → 迁移与内化

## 2. 现有方法已经解决得不错的部分

### 2.1 知道 / 记住模型
成熟方法：
- Mental Model Library
- Spaced Repetition
- Retrieval Practice
- Anki / FSRS 一类工具

已经比较成熟的问题：
- 模型发现
- 定义学习
- 记忆保持
- 基础例子
- 复习调度

结论：

> “做一个思维模型知识库”本身并不是明显空白。

### 2.2 单项判断技能训练
代表：
- Clearer Thinking 等 interactive tools

已经能较好训练：
- calibration
- sunk cost
- fail-safing
- mental traps
- decision framing

结论：

> 把复杂思考拆成可练习的小技能，本身已有成熟实践。

### 2.3 决策记录与事后复盘
代表：
- Decision Journal
- append-only / immutable decision record 项目

已经比较成熟的机制：
- 保存当时判断
- 保存理由和假设
- 保存置信度
- review date
- outcome review
- 防 hindsight bias
- 区分判断质量与运气

结论：

> “记录决策 + 以后复盘”本身也不是新的产品命题。

### 2.4 概率判断与长期校准
代表：
- Metaculus / forecasting platforms

已经成熟的机制：
- 明确 resolution criteria
- probability forecast
- belief update
- re-affirm
- stale forecast withdrawal
- calibration curve
- long-term track record

结论：

> 有明确可验证结果的判断，已经存在非常成熟的反馈范式。

### 2.5 苏格拉底式 AI 追问
代表：
- Socratic AI tutor 类产品

已经可以做到：
- 不直接给答案
- 追问
- 要求解释
- 暴露假设
- 提供提示
- 挑战盲区

结论：

> “AI 不直接回答，而是提问”本身也不是足够独特的产品方向。

### 2.6 论证结构训练
代表：
- argument mapping
- debate training
- Toulmin-style tools

成熟能力：
- claim
- evidence
- counterargument
- rebuttal
- persuasion
- structure feedback

结论：

> “把论证质量显性化并进行训练”已经是成熟子领域。

### 2.7 专业领域案例推理
代表：
- 医疗 / 临床 reasoning trainer
- virtual patient / simulation training

成熟能力：
- 情境识别
- 信息采集
- 判断
- 行动
- feedback
- debriefing
- repeated case training

结论：

> “通过案例练推理”本身也不是新想法；真正困难的是把它扩展到开放现实生活。

## 3. 最重要的学习科学结论

### 3.1 迁移不会自动发生

核心结论：

> 知道一个模型，不等于现实中会主动调用。

near transfer 相对容易，far transfer 很难。

因此不能假设：

> 学模型 → 记住 → 自然变得更会思考

### 3.2 真正需要迁移的是“关系结构”

现实问题表面不同，但底层结构可能相同。

例如：
- 项目负责人为了奖金强推上线
- 销售为了季度指标提前确认订单
- 平台司机受补贴规则影响改变行为

共同结构可能是：

> 激励结构改变行为选择。

因此训练的关键不是只记案例，而是学会抽象：
- 角色
- 激励
- 约束
- 因果
- 风险
- 信息结构

### 3.3 多案例比较比单案例更利于抽象

更有潜力的训练机制：

> 多个表面不同但结构相同的案例
> → 主动比较
> → 抽象共同结构

而不是：

> 一个模型定义 + 一个经典案例

### 3.4 会用 ≠ 会主动想到

必须区分：
- cued performance：给模型名后会不会用
- spontaneous performance：不给提示时会不会自己想到

这对未来产品评估非常重要。

### 3.5 Interleaving 的价值是“区分相邻模型”

它不是简单随机打乱题目。

真正值得借鉴的是训练：
- 激励机制 vs 心理偏差
- 安全边际 vs 反向思维
- 能力圈 vs 暂时信息不足

也就是：

> 什么时候该选哪个模型，以及什么时候多个模型同时成立。

### 3.6 Self-explanation 很重要

用户不能只回答：
> “这是激励机制。”

还应该能说：
> 为什么适用？
> 哪些条件对应模型结构？
> 哪些证据支持？
> 哪些替代解释仍然存在？

### 3.7 Scaffold 必须最终撤掉

初期给予示范、提示并不一定是坏事。

但训练最终必须测试：
> 没有提示还能不能自主调用。

因此需要考虑：
> support → fading → no-cue test

而不是永久提供模型菜单。

## 4. 判断质量不能被压成一个 AI 总分

“判断质量”至少有三条不同轨道。

### 4.1 Prediction Quality
适合：
- 有未来结果的问题

可以看：
- probability
- calibration
- Brier score
- discrimination / resolution

### 4.2 Argument Quality
适合：
- 人际
- 人生决策
- 复杂问题
- 没有干净 outcome 的问题

可以看：
- claim
- evidence
- assumption
- alternative explanation
- counterargument
- rebuttal

### 4.3 Metacognitive Quality
跨所有任务：
- 我有多确定？
- 哪些是事实？
- 哪些是假设？
- 什么信息会让我改变观点？
- 新证据出现后我会不会更新？

结论：

> “AI 给你 87 分”这种设计非常可疑。

## 5. AI 的角色边界

### 5.1 AI 的高价值位置
更适合：
- challenge
- 反例
- 证据追问
- 生成变式案例
- 暴露遗漏变量
- 跨历史记录找模式
- 对比相似案例
- 检查结构一致性

### 5.2 AI 的高风险位置
风险很大的用法：
- 一开始就替用户分析
- 直接选择模型
- 把模糊猜想润色成漂亮论证
- 充当“最终真理裁判”
- 永久提供模型菜单

核心风险：

> cognitive offloading

因此目前较强的原则候选是：

> 用户先想，AI 后挑战。

## 6. Decision Journal 的长期使用结论

### 6.1 一条记录必须有未来

一个很强的 Product Principle 候选：

> A record should have a future.

一条记录至少应该存在某种未来用途：
- review
- resolution
- stale check
- 相似案例召回
- 跨记录模式分析

否则只是数字垃圾。

### 6.2 原始判断必须冻结

“当时怎么想”和“后来怎么看”不能混成一个对象。

因此：
> update, don't rewrite

### 6.3 不要记录所有事情

更合理的是 selective capture：
- 高影响
- 高不确定
- 高代价
- 可验证
- 反复出现
- 值得训练

而不是追求每日 streak。

### 6.4 搜索不是关键，未来召回才是

真正重要的不是：
> 我以后能搜到过去。

而是：
> 当过去经验再次相关时，它会不会重新进入当前问题。

## 7. 真实经历如何变成训练

研究后最重要的判断是：

> experience 本身不是 learning。

真实事件需要经过某种加工：

> 事件
> → 关键线索
> → 关系结构
> → 当时判断
> → 行动
> → 结果
> → debrief
> → 可迁移模式

### 7.1 Real → Abstract
从真实事件中抽象可迁移结构。

### 7.2 Abstract → Synthetic Variants
生成：
- 表面不同、结构相同
- 表面相似、结构不同
- 隐藏条件
- 干扰信息
- 反例

### 7.3 Synthetic → Real
最终回到无提示的现实调用。

因此当前很强的学习循环候选是：

> Reality → Abstraction → Variation → Reality

## 8. Existing Solutions Map 的总体结论

现有产品并不是能力弱，而是高度分工：

| 类别 | 最擅长解决 |
|---|---|
| Mental Model Apps | 学习、记忆 |
| Clearer Thinking | 单项认知技能 |
| Decision Journals | 保存判断、复盘 |
| Metaculus | 概率校准 |
| Socratic AI Tutor | 当场追问 |
| Argumentation Tools | 论证结构 |
| Domain Case Trainers | 案例推理与反馈 |

最重要的发现不是“这些工具不好”，而是：

> 它们通常没有围绕同一个人的长期现实问题，把训练、判断、反馈、现实结果和迁移串起来。

## 9. 目前最明显的 Coverage Gaps

### Gap A — Open-world spontaneous retrieval

现实问题没有模型菜单。

真正需要训练的是：

> 在一个开放问题里，用户自己能否想到相关模型或思考角度。

### Gap B — Model discrimination & combination

缺少成熟训练：

> 哪个模型更相关？
> 哪个模型不适用？
> 哪几个模型可以组合？
> 哪些解释互相冲突？

### Gap C — Real experience ↔ Training

现有工具往往分裂为：
- Journal：只存真实经历
- Trainer：只给人工案例

缺少明显成熟的：

> 真实经历 → 抽象 → 变式训练 → 迁移回现实

### Gap D — Multi-track correction

缺少统一但不混淆的：
- 结构纠错
- 证据纠错
- 置信度纠错
- 现实纠错

### Gap E — Longitudinal Personal Reasoning Model

缺少长期回答：

> 我在哪类问题上容易错？
> 我经常漏掉什么？
> 哪些模型经常被我误用？
> 哪些高置信判断经常翻车？
> 哪些结构在我的生活里反复出现？

### Gap F — AI Without Cognitive Offloading

核心设计问题仍未解决：

> 如何利用 AI 的反馈、生成、对比和跨记录分析能力，同时保证“第一遍思考”仍然属于用户。

## 10. Do Nothing / Existing Tools Stack 是强候选

今天完全可以组合现有工具：

- 模型学习：Mental Model Apps
- 微技能：Clearer Thinking
- 概率校准：Metaculus
- 真实决策：Decision Journal
- AI challenge：ChatGPT / Socratic Tutor
- 长期存储：Markdown / Notion / Obsidian

因此 Phase 3 必须把以下方案作为正式候选：

> Do Nothing / Existing Tools Stack

新的独立产品只有在以下方面明显优于工具组合，才有理由存在：

- integration
- continuity
- lower cognitive switching cost
- better transfer
- better feedback loop
- better recall of past experience
- better longitudinal personal learning

## 11. 目前最重要的 Product Discovery 判断

Phase 2 到这里，最强的结论不是：

> “我们应该做一个思维模型 App。”

而是：

> 真正未被很好解决的，可能是“训练、现实问题、反馈、长期经验与迁移之间的整合”。

因此未来产品的核心对象未必是：
- 模型

也可能是：
- case
- judgment
- decision
- belief
- episode
- reasoning pattern
- personal case network

这个问题必须留到 Phase 3，让不同产品范式竞争，不能现在提前决定。

## 12. 一个当前很强但尚未决策的机制链

结合 Phase 2 研究，当前较有证据支持的训练机制假设是：

> 具体案例
> → 同模型多案例比较
> → 抽象关系结构
> → 相邻模型对比
> → interleaved discrimination
> → 无标签检索
> → self-explanation
> → 用户先判断
> → AI / 外部挑战
> → 现实反馈
> → debrief
> → 跨领域变式
> → scaffold fading
> → 真实开放问题中自发调用

重要：

> 这不是产品流程。
> 它只是 Phase 2 得到的学习机制假设。

Phase 3 不应该被迫按照这条链设计产品。

## 13. Phase 2 明确排除的早期陷阱

后续 Product Directions 不应默认：

- 思维模型是一级对象；
- 模型越多越好；
- 每个模型都需要卡片；
- spaced repetition 是主轴；
- 每天训练是必要条件；
- 训练准确率等于能力；
- AI 总分有意义；
- 所有现实事件都值得记录；
- 所有模型使用都有唯一正确答案；
- 所有模型应该使用统一训练模板；
- 只要 AI 用苏格拉底方式提问就能避免认知外包；
- 做一个 Decision Journal 就完成了闭环。

## 14. Phase 2 输出给 Phase 3 的要求

下一阶段提出 Independent Product Directions 时，每个方案必须回答：

1. 它的一级核心对象是什么？
2. 用户最常做的行为是什么？
3. 它主要解决五层能力链中的哪些层？
4. 哪些部分直接复用成熟方法，而不是重造？
5. 它怎样避免 cognitive offloading？
6. 它怎样促进 real-world transfer？
7. 它如何利用真实经历，而不是只做人工题库？
8. 它为什么比 Existing Tools Stack 更值得长期使用？
9. 如果这个方向错了，最便宜的验证实验是什么？

## 15. Phase 2 最终结论

Phase 2 可以暂时收束为一句话：

> **现有市场已经分别解决了“学模型、练单项技能、记决策、做概率校准、苏格拉底追问、论证训练和专业案例推理”，但目前没有发现成熟方案把“现实经验 → 模型化理解 → 自主调用 → 反馈纠错 → 现实验证 → 跨案例迁移 → 长期个人推理模式”作为一个统一的长期训练闭环。**

这不证明该产品一定值得做。

它只说明：

> 如果 Phase 3 要提出一个真正有价值的新方向，价值不应该来自“更多模型”或“多一个 AI 聊天框”，而应该来自对这些断裂环节的更好整合。

## 16. 下一阶段

Phase 3 — Independent Product Directions

要求：
- 至少提出 4–6 种彼此明显不同的产品范式；
- 核心对象、用户行为、训练方式必须真正不同；
- 不提前综合；
- 保留 Do Nothing / Existing Tools Stack；
- 每种方案后续进入独立 Challenge。

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

## 5. 第二轮专题：为什么知识不会自动迁移成现实思维方式

### 5.1 远迁移不是默认结果

认知训练研究中长期存在一个稳定现象：

> 人通常会在被训练的任务和相似任务上进步，但这种进步很难自动扩展到结构不同、表面不同的现实任务。

关于 working memory、棋类、音乐、电子游戏等认知训练的 meta-analysis / second-order meta-analysis 都显示：near transfer 比较常见，而 far transfer 很小，控制 placebo 与 publication bias 后甚至可能接近于零。

对本项目最直接的含义：

> “学过很多思维模型”不能被当作“现实判断自然会变好”的代理指标。

如果训练只让用户在“看到模型名字 → 回忆定义”“看到典型案例 → 选出正确模型”上越来越熟练，完全可能出现训练内表现很好、现实调用仍然很差。

### 5.2 迁移的关键不是表面相似，而是识别关系结构

类比推理研究反复区分两类相似：

- surface similarity：人物、行业、物体、事件表面像；
- relational / structural similarity：背后的关系结构、因果关系、约束模式相同。

现实调用之所以难，一个重要原因是：

> 新问题表面上往往与学模型时的例子完全不像。

例如：

- “项目负责人为了奖金强推上线”
- “销售为了季度指标把未来订单提前确认”
- “平台司机为了奖励规则改变接单行为”
- “自己设置运动打卡奖励后反而开始刷形式”

表面完全不同，但都可能包含同一种“激励改变行为”的结构。

专家与成熟推理者更容易按照深层关系结构组织问题，而新手更容易被表面特征吸引。

因此，思维模型训练不能只教“模型 → 典型案例”；还需要训练：

> 从杂乱的现实描述中抽取关系结构。

### 5.3 单个案例往往不够，多案例比较更容易抽象出模型

case comparison / analogical encoding 是目前与本项目最相关的证据之一。

研究发现：
- 比较两个体现同一原则的案例，能帮助学习者抽象出共同结构；
- 在 negotiation 研究中，让学习者比较两个案例并提炼共同原则，比把两个案例分别分析更容易迁移到新的面对面谈判；
- 经典实验中，comparison 条件在后续真实谈判里使用目标策略的概率显著更高；
- 57 个实验、336 个测试的 meta-analysis 中，case comparison 相对其他学习方式总体产生中等程度的学习优势（d≈0.50）。

这直接挑战一种常见设计：

> 一张“激励机制”卡片 + 一个经典案例 + 一道练习题

可能远远不够。

更有潜力的训练方式是：

> 多个表面不同、结构相同的案例 → 主动比较 → 自己说出共同结构 → 再到一个表面更远的新场景中识别。

### 5.4 “会推理”与“会主动调用推理”是两件事

较新的 relational reasoning 综述特别强调一个区分：

> ability to reason relationally ≠ likelihood of spontaneously doing so.

也就是说，一个人可能具备类比推理能力，但现实中根本不会主动使用。

这与 Phase 1 的“知道 → 想到”断层高度一致。

因此，我们不能只测：
- 给出激励机制后，用户会不会分析；

还要关心：
- 不告诉任何模型的情况下，用户是否会主动注意到激励结构。

这是“提示下会用”与“自发调用”的区别。

### 5.5 元认知的作用：让人监控“我是怎么想的”

Metacognition 通常包含：
- planning
- monitoring
- evaluation

computer-based learning 环境中的 meta-analysis 显示，metacognitive prompts 对 self-regulated learning 和学习结果都有中等正向效果，而且效果会受到反馈、提示具体性、是否个性化/自适应等因素影响。

这意味着：
- “你用了什么模型？”
- “这个判断依赖什么假设？”
- “你有什么证据？”
- “还有什么解释没有排除？”
- “你为什么认为这个模型适用？”

这类问题不是装饰性反思，它们可能帮助用户把隐性的思维过程显性化，从而更容易得到反馈和修正。

但也存在重要限制：

> prompt 本身可能变成拐杖。

如果系统每次都提醒用户“考虑激励机制 / 安全边际 / 机会成本”，用户可能只是学会跟随提示，而没有形成自主调用。

所以真正需要验证的是：

> 如何逐步撤掉 scaffold，让“被提示会用”变成“不提示也会用”。

### 5.6 认知灵活性并不等于“会很多模型”

2024 年关于 cognitive flexibility training 的综述将认知灵活性描述为多成分能力，包括：
- 学习环境结构；
- 在不同特征、维度、任务之间切换注意；
- 在不确定环境中采用新规则。

研究者强调 real-world transfer 需要考虑：
- 个体差异；
- engagement / motivation；
- adaptive / personalized training；
- 多成分训练，而不是单一任务反复刷。

这提示我们：

> “掌握很多模型”只是工具库存，不代表能灵活选择和切换视角。

真正要训练的还包括：
- 什么时候坚持当前模型；
- 什么时候切换；
- 什么时候组合多个模型；
- 什么时候承认现有模型不足。

### 5.7 当前最强的机制假设：对比 → 抽象 → 自发检索 → 应用 → 反馈 → 变式再迁移

结合这一轮证据，目前比“模型卡片 + 复习”更有依据的训练机制假设是：

1. **Concrete cases**：先接触具体情境；
2. **Contrast / comparison**：比较多个案例，而不是只看一个；
3. **Structure extraction**：主动提炼共同关系结构；
4. **Retrieval**：在不告诉模型名称的新情境中自己想起来；
5. **Application**：把模型真正用于解释、判断或行动；
6. **Feedback / metacognition**：检查模型是否适用、证据是否足够、是否存在替代解释；
7. **Variation**：换领域、换表面、换尺度再次练习；
8. **Scaffold fading**：逐步减少提示，测试是否形成自发调用。

这仍然是 Hypothesis，不是产品流程。

## 6. 对五层能力链的修正理解

### 知道
不能只记定义，还需要建立多个具体实例与反例。

### 想到
核心不是“记忆强度”本身，而是能否从现实问题中识别关系结构，并从记忆中检索出相关模型。

### 用出来
不仅识别模型名称，而要完成结构映射：当前情境中的角色、关系、约束、因果分别对应模型中的什么。

### 被纠正
反馈既要检查结论，也要检查：
- 模型匹配是否合理；
- 是否只因表面相似而误用；
- 是否漏掉更合适的模型；
- 是否把一个模型解释成万能因果。

### 迁移与内化
不能只靠重复同类题；需要：
- 表面差异很大的多案例；
- 主动比较；
- 新领域变式；
- 提示逐渐消失；
- 在真实问题中的 spontaneous retrieval。

## 7. 对产品 Discovery 的重要影响

### 7.1 一个重大反例：不要把“模型数量”当成核心成功指标

知道 100 个模型可能不如能把 10 个模型跨场景调用。

### 7.2 单模型单案例学习存在结构性风险

它容易让用户把模型与某种“典型故事外观”绑定，而不是理解底层关系结构。

### 7.3 多案例对比可能比更多解释更重要

真正形成抽象结构的过程可能来自：
- “这三个案例哪里不一样？”
- “它们为什么实际上是同一个问题？”

而不是 AI 再解释一次模型定义。

### 7.4 AI 的角色可能应该包含“制造变式”

AI 的一个潜在优势不是单纯讲解，而是：
- 生成表面不同但结构相同的案例；
- 生成结构接近但模型不适用的反例；
- 故意加入噪声信息；
- 隐藏关键条件；
- 根据用户错误改变下一道训练。

### 7.5 必须防止提示依赖

如果模型名称、候选列表、分析框架始终摆在用户面前，训练结果可能只证明：

> 用户在看到提示时会使用模型。

而我们的目标是：

> 用户在没有提示的现实问题里也会主动调用。

因此未来实验需要显式区分：
- cued performance
- spontaneous performance

## 8. 下一轮研究

继续深入：
- transfer-appropriate processing / retrieval cues
- interleaving / varied practice 对模型选择的影响
- analogical retrieval failure 与专家/新手差异
- worked examples vs self-explanation
- fading scaffolds
- forecasting / calibration 如何训练判断反馈
- AI tutor 如何在不替代思考的情况下提供反馈

最终 Phase 2 要形成：
- Existing Solutions Map
- Mechanism Map
- Coverage Gaps
- Unsolved Problems
- 可进入 Phase 3 的独立产品方向输入


## 9. 第三轮专题：为什么现实里想不起来，以及如何训练模型选择

### 9.1 Analogical Retrieval Failure：想不起来，往往是编码方式出了问题

类比迁移研究长期发现：
- 人更容易被表面相似性提醒，而不是被深层关系结构提醒；
- 经典实验中，表面相似的旧案例被检索出来的频率可达到表面不相似案例的 2–4 倍；
- 专家相比新手，更容易按结构特征表示问题，因此更容易发生跨表面、跨情境迁移；
- 2025 年 ADAPTER 模型进一步强调：检索是否能基于结构，很大程度取决于原始案例是如何被编码的，以及学习者是否已经拥有合适的抽象类别。

对本项目的含义：

> “想到一个模型”不只是记忆强不强，而是模型在记忆里以什么形式被编码。

如果学习时把“激励机制”绑定成：
> 老板给奖金 → 项目负责人拼命上线

那么现实里遇到：
> 平台补贴导致司机改变接单策略

可能完全想不起来。

更有迁移价值的编码应逐渐抽象为：
> 奖励 / 惩罚结构改变行为选择。

因此，“模型学习”至少需要同时形成：
- 具体案例记忆；
- 抽象关系结构；
- 多种可能检索线索。

### 9.2 Inert Knowledge：知识存在，但处于“惰性”状态

Gentner 等关于 inert knowledge 的研究指出，人可能已经拥有可用于解决新问题的知识，却无法在新场景中主动检索出来。

这解释了 Phase 1 中的关键现象：

> “我学过，也会解释，但现实里没想到。”

通过多个案例做 relational comparison / analogical abstraction，可以提高后续关系性检索。

因此，“知道”与“想到”之间不是简单的熟练度差异，而存在真实的检索断层。

### 9.3 Retrieval Practice 有用，但关键是怎么检索

关于 test-enhanced learning transfer 的 meta-analysis（122 个实验，N=10,382）发现：
- retrieval practice 对迁移总体有正效应（d≈0.40）；
- 对 application / inference 类任务的迁移更明显；
- elaborated retrieval practice 是重要 moderator；
- 并不是所有检索形式都同样有效。

2025 年 retrieval practice vs elaborative encoding 的 meta-analysis 进一步显示：
- retrieval practice 整体只有小幅优势；
- 没有反馈时，一些 elaborative encoding 方法反而更有效；
- 自由回忆比强提示式回忆的优势更明显。

对本项目的含义：

不应该只做：
> “安全边际的定义是什么？”

更值得验证的是：
> 给一个新场景，不提供模型名，让用户自己检索可能相关的模型，并解释为什么。

也就是说，训练需要从：
> model → recall definition

逐渐转成：
> situation → retrieve candidate models

### 9.4 Interleaving 的真正价值：训练“区分”，不是简单打乱

Interleaving 的 meta-analysis 显示总体存在中等学习优势，但效果依赖任务性质。

较稳定的解释是 discriminative-contrast hypothesis：

> 把容易混淆的类别交错出现，会迫使学习者注意“它们到底哪里不同”。

Interleaving 在：
- 类别很相似；
- 必须做 discrimination；
- 规则容易混淆

时效果尤其明显。

而当任务根本不需要区分类别时，interleaving 未必有效。

因此，对本项目而言，interleaving 不应该理解成：

> 随机把各种思维模型题目混在一起。

真正值得借鉴的是：

> 把“容易一起想到、容易误用、边界接近”的模型放在一起训练区分。

例如：

#### 激励机制 vs 心理偏差
问题：
> 对方为什么这么做？

区分：
- 是外部收益结构在驱动？
- 还是认知偏差 / 情绪 / 身份在驱动？

#### 安全边际 vs 反向思维
问题：
> 如何降低失败风险？

区分：
- 是先找失败路径？
- 还是为预测误差和不可知因素留余量？

#### 能力圈 vs 信息不足
问题：
> 我为什么不该现在下结论？

区分：
- 是这个领域长期超出自己的知识边界？
- 还是当前只是缺少一条可以补齐的信息？

这类训练比“连续练十道安全边际题”更接近真实世界。

### 9.5 Blocked Practice 和 Interleaved Practice 可能承担不同阶段的任务

Blocked practice 并不是“坏方法”。

它更适合：
- 刚接触一个模型；
- 先形成基本结构；
- 找到同类案例的共同点。

Interleaved practice 更适合：
- 已经知道多个相邻模型；
- 需要学会区分；
- 需要在没有标签的情况下选择。

所以一种更符合证据的训练 progression 可能是：

> Blocked：先看清“它是什么”  
> → Contrast：再看清“它和谁不一样”  
> → Interleaved：再练“什么时候该选谁”  
> → Open-world：最后在没有候选列表的现实问题里自己调用

这仍然只是机制假设，不是产品流程决定。

### 9.6 Self-Explanation：逼用户说出“为什么选这个模型”

Self-explanation 的 meta-analysis 显示总体有中等正效应（g≈0.55）。

它的关键不是让用户多写字，而是迫使用户生成：
- 因果关系；
- 概念关系；
- 为什么这一步成立；
- 为什么这个模型适用。

对本项目来说，一道题只回答：

> “激励机制”

远远不够。

更有训练价值的回答是：

> “我认为这里主要是激励机制，因为负责人在‘按时上线’和‘产品质量’之间承担的个人收益/成本不对称；如果奖金与准时上线绑定，而严重 bug 的后果由团队或公司承担，那么其行为在个人激励下是可解释的。”

这一步既训练模型应用，也能让 AI 有东西可以纠正。

### 9.7 Worked Examples + Fading：新手不一定应该一开始就裸做

Worked example 研究以及 scaffolding 研究表明：
- 新手通常受益于示范；
- self-explanation 能增强示范学习；
- 随着能力增加，逐步撤掉步骤 / 提示，有助于迁移；
- adaptive fading 可能优于一刀切。

因此，“一开始完全不给提示才算真正思考”并不一定科学。

更合理的是：

> 初期支持足够多 → 中期减少支持 → 后期无提示测试。

关键不是永远不给帮助，而是帮助必须最终被撤掉。

### 9.8 当前对“模型选择”的机制假设

现实模型选择可以暂时拆成四种难度：

#### Level A：给模型名
> “请用安全边际分析。”

主要测“用出来”。

#### Level B：给候选集合
> “安全边际 / 反向思维 / 能力圈里哪个更相关？”

主要测模型 discrimination。

#### Level C：不给模型名，但问题来自已学模型范围
> “你会从哪些角度分析？”

主要测 spontaneous retrieval。

#### Level D：开放现实问题
模型可能：
- 一个；
- 多个；
- 当前学过的都不合适。

主要测真正的开放世界判断。

这个梯度比简单的 L1-L5 “熟练度等级”更有认知机制依据，但目前仍只是研究假设。

## 10. 当前形成的更强训练假设

结合三轮研究，目前一个较强但仍待实验验证的机制链是：

> 具体案例
> → 同模型多案例比较
> → 抽象关系结构
> → 相邻模型对比
> → interleaved discrimination
> → 无标签情境检索
> → self-explanation
> → AI / 外部反馈纠错
> → 跨领域变式
> → scaffold fading
> → 开放现实问题自发调用

这个链条最重要的不是步骤数量，而是它同时处理三个不同困难：

1. **理解模型**：形成结构，而不是背定义；
2. **检索模型**：现实中能够自己想起来；
3. **选择模型**：多个可能模型之间能区分和组合。

## 11. 新的 Product Discovery 风险

### 11.1 模型菜单可能伤害真实迁移
长期显示“可选模型列表”，会把现实不存在的检索线索永久留给用户。

### 11.2 训练准确率可能是假指标
如果训练题明确属于某几个模型，用户可以学会猜题型，而不是学会思考。

### 11.3 AI 过早提示会污染测量
AI 一旦提示“考虑激励”，就无法再知道用户本来是否能自主想到。

### 11.4 相似模型的边界需要允许重叠
现实问题通常不是单标签分类任务。Interleaving 用于训练辨别，但不能把“选模型”误做成只有一个标准答案的分类器。

### 11.5 “没想到模型”不一定是错误
有时不用任何命名模型，也能做出高质量分析。最终评价仍应回到判断过程，而不是模型召回数量。

## 12. 下一轮值得继续查的问题

1. Forecasting / calibration：怎样给“判断质量”建立长期反馈？
2. Argumentation training：怎样训练证据、反例、论证质量？
3. AI tutor：怎样提供反馈而不污染自主思考测量？
4. Real-world reflection：真实经历如何进入训练，而不是永远做人工案例？
5. 是否已有产品真正把 retrieval + discrimination + reflection + real-world decision journal 连起来。


## 13. 第四轮专题：怎样判断“判断质量”真的变好了

### 13.1 不能用一个总分评价所有判断

“判断质量”至少应区分三个对象：

1. **预测质量（forecast quality）**
   - 对未来事件给出概率判断；
   - 能否长期校准；
   - 是否区分 55%、70%、90% 这种置信程度。

2. **论证质量（argument quality）**
   - claim 是否明确；
   - evidence 是否相关、充分；
   - 是否考虑 counterargument；
   - rebuttal 是否真正回应反方；
   - 是否能协调多种竞争解释。

3. **元认知质量（metacognitive quality）**
   - 自信与真实表现是否匹配；
   - 是否知道哪些是事实、哪些是猜测；
   - 是否知道自己在哪些部分信息不足；
   - 是否会根据新证据主动降置信度或改观点。

这三个对象不能被压成一个“AI 思考分”。

### 13.2 Forecasting / Calibration：把部分判断变成可验证概率

Good Judgment Project 等 forecasting tournament 的核心贡献之一，是把模糊判断转换成概率预测。

例如不是说：
> “这个项目大概率会延期。”

而是：
> “在 5 月 20 日前按原范围正常上线的概率是 35%。”

这类判断可以在结果出现后通过 proper scoring rules（如 Brier score）长期评价。

Brier score 的意义不是“猜中没猜中”，而是同时惩罚：
- 错误预测；
- 过度自信。

如果一个人长期说 70% 会发生，那么这些事件最终应该大约 70% 真正发生，才算 calibration 较好。

2025 年基于 Good Judgment Project 39,481 个初始预测、851 名 forecaster 的研究显示：
- probabilistic reasoning training 能显著降低一类 compensatory miscalibration；
- 对另一类偏差的改善更有限，而且第二年才出现。

这意味着：
> calibration 是可训练的，但不是一次教程就能完全解决。

### 13.3 只看 Brier score 也不够

Forecasting 文献本身提醒：
- calibration 只是预测质量的一部分；
- 一个永远预测 50% 的人可能显得不极端，却没有 discrimination / resolution；
- 需要区分“概率是否诚实”与“能不能把高概率事件和低概率事件区分出来”。

因此未来若用概率判断，不应把单一 Brier score 当成万能能力指标。

### 13.4 Feedback 为什么有效：必须让人看见“自信与现实”的偏差

判断预测研究显示：
- 人常见过度自信；
- 给出 outcome feedback 后，置信区间预测可以明显改善；
- 改善不仅仅来自“以后都说得保守一点”，而可能来自学习任务本身的噪声与不确定性。

这提示一种重要机制：

> “我错了”本身反馈太弱。
> 更重要的是：“我当时有多自信？实际又怎样？”

例如：
- 判断：项目 80% 可以准时上线；
- 结果：失败；
- 复盘：当时为什么给 80%，而不是 55%？
- 哪条证据被高估？
- 哪个变量完全没考虑？

长期积累后才能看到：
> 我是不是经常把 60% 的事情当成 90%。

### 13.5 Argumentation：复杂现实判断不能只靠最终结果评价

很多人生决策、人际关系、复杂问题，并没有干净的 binary outcome。

这时 argumentation research 提供了另一套评价对象：

- claim；
- evidence；
- counterargument；
- rebuttal；
- integration of competing claims。

2024 年 Kuhn 等人的研究显示：
- 单独做 argument training 可以提升 argument skill；
- 在其中加入 inquiry training 后，学习者在 evidence use、counterargument、以及整合对立主张方面获得更大提升。

重要启示：

> 好判断不只是“能为自己的观点找理由”，还包括主动调查、寻找证据和处理相反观点。

这与我们之前“AI 找反例”的设想相比更进一步：
> 不是 AI 替你生成一个反例就结束，而是训练你自己形成 inquiry + counterargument 的习惯。

### 13.6 “反驳自己”可能是判断训练的核心动作之一

多项 argumentation 研究表明：
- counterargument 和 rebuttal 可以被显式训练；
- 更成熟的 reasoning 不只是单边支持自己的 claim；
- 能处理 opposing claims、evidence 和 rebuttal 与更高质量的 critical thinking 相关。

2026 年一项关于 far transfer 的研究甚至发现：
- 在中性话题上进行 argumentation + reflection 训练；
- 能迁移到具有个人立场和情绪负荷的社会议题；
- 改善 evidence use、counterargument 和 two-sided reasoning。

研究者将这种迁移部分归因于形成了 meta-level 的：
- evidence orientation；
- multiperspectivity。

对本项目的意义：

> “有没有想到反方为什么可能是对的”可能比“用了几个模型”更接近判断质量。

### 13.7 论证结构评分存在，但不能简单让 AI 当裁判

Computer-supported argumentation learning 的 2025 systematic review 显示：
- argumentation graph 是常见工具；
- 自动化、可扩展 feedback 越来越常见；
- 面向个人学习者的系统数量已经超过纯协作系统。

这说明：
> claim-evidence-counterargument-rebuttal 的结构化训练已经有成熟基础。

但风险是：
- 一个论证结构完整，不等于它的事实是真的；
- AI 能判断“形式上有没有反例”，不代表能可靠裁决复杂现实真相；
- 因此 AI 更适合指出结构缺口、要求证据、生成挑战，而不是给最终“正确/错误”判决。

### 13.8 元认知校准：高质量判断必须知道自己“不知道”

confidence 与 accuracy 并不天然一致。

临床判断 meta-analysis 显示：
- confidence 与 accuracy 只有较弱正相关；
- 说明“感觉自己很确定”不能作为正确性的代理。

因此，一个成熟判断体系应该允许并鼓励：
- 30%；
- 55%；
- 80%；
- “目前证据不足，无法判断”。

而不是把所有分析都包装成一个确定结论。

### 13.9 AI 反馈最大的风险：把表达质量误当判断质量

LLM 特别擅长：
- 补全理由；
- 把逻辑写顺；
- 增加术语；
- 生成结构漂亮的 argument。

这会产生一个严重风险：

> 用户原本只有一个模糊猜想，AI 把它润色成了一个看起来高度合理的论证，于是用户误以为自己的判断变强了。

所以 AI feedback 必须尽量发生在：
> 用户先输出自己的判断、依据、置信度之后。

然后 AI 才能：
- challenge；
- ask for evidence；
- generate counterexamples；
- surface missing variables；
- compare alternative hypotheses。

而不是先替用户完成分析。

### 13.10 2026 年关于 AI cognitive offloading 的新证据

2026 年一项 preregistered experiment（N=704）研究了 LLM 辅助下的 cognitive offloading：
- metacognitive feedback 显著降低直接向 AI 索要答案的行为；
- 并提升之后无 AI 测试中的表现；
- 单纯用奖励鼓励“少问 AI”没有显示同样效果。

虽然实验任务是分数运算，不能直接外推到思维模型训练，但它提供了一个很重要的设计信号：

> 与其禁止 AI，不如让用户清楚意识到“这一步外包给 AI 会失去什么练习机会”。

另一个 2026 年大样本研究（N=1237）发现：
- 用户普遍认为 AI 会明显提高简单认知任务速度；
- 但实际完成时间并没有显著更快；
- 主观 effort 却更低。

这说明：
> AI 会制造“我更高效了”的主观感觉，而这种感觉可能并不对应真实能力提升。

### 13.11 当前更合理的反馈体系：三条轨道

#### Track A — Prediction Calibration
适用于：
- 有未来可验证结果的判断；
- 项目是否延期；
- 某方案能否成功；
- 自己能否在期限内完成目标。

记录：
- prediction；
- probability；
- deadline / resolution condition；
- reasoning。

结果出现后：
- resolve；
- 计算 calibration / proper score；
- 复盘过度或不足自信。

#### Track B — Argument Quality
适用于：
- 人际冲突；
- 人生决策；
- 复杂系统解释；
- 很难得到干净 outcome 的问题。

检查：
- claim；
- evidence；
- assumptions；
- alternatives；
- counterarguments；
- rebuttals；
- missing information；
- model applicability。

#### Track C — Metacognitive Quality
跨所有任务：

检查：
- 哪些是事实；
- 哪些是假设；
- 我多确定；
- 哪些信息会让我改变观点；
- 我是否在寻找支持自己观点的证据；
- 新证据出现后有没有及时更新。

### 13.12 一个关键 Product Discovery 判断

未来产品如果只有：
> AI 给你 85 分：分析得很好

那几乎没有意义。

更有价值的是保存可追踪的判断对象：

> 当时我认为 X；
> 我的置信度是 70%；
> 我依据 A/B/C；
> 我忽略了 D；
> AI 当时挑战了 E；
> 后来现实反馈是 F；
> 下一次我的判断发生了什么变化。

训练对象从“回答质量”变成：
> 判断如何随证据和反馈演化。

### 13.13 当前最强的“被纠正”机制假设

目前可以把 Phase 1 的“被纠正”层进一步拆成：

1. **结构纠错**
   - 推理有没有缺口；
   - 模型是否误用；
   - 是否缺反例。

2. **证据纠错**
   - 事实是否成立；
   - 信息来源是否可信；
   - 是否存在缺失变量。

3. **置信度纠错**
   - 自信是否和证据强度匹配；
   - 是否长期过度自信 / 过度保守。

4. **现实纠错**
   - 后续事件发生后，原判断哪些成立；
   - 是判断差还是外部随机性；
   - 有没有新的可重复经验。

### 13.14 下一步研究

下一轮值得继续查：

1. Decision Journal / Forecasting Platform 的真实长期工作流；
2. 哪些现有产品已经在保存 probability + reasoning + outcome；
3. 如何把真实生活事件变成可 resolution 的 prediction；
4. source credibility / lateral reading 如何进入证据纠错；
5. AI feedback 如何做到“challenge first, answer later”；
6. 哪些 judgment metrics 适合个人长期使用，而不会把产品变成统计工具。


## 14. 第五轮专题：Decision Journal / Forecasting 的真实长期工作流

### 14.1 长期可用系统的共同点：不是“多记录”，而是让旧判断重新回到工作流

对 Metaculus、Decision Journal 类产品和若干开源项目的比较显示，一个长期可用的判断记录系统通常包含四个阶段：

1. **Capture now**
   - 在决策发生时保存当时判断；
   - 不要求事后回忆；
   - 尽可能保留当时信息状态。

2. **Freeze / preserve**
   - 原始判断不被后见之明覆盖；
   - 后续变化通过追加记录，而不是修改过去。

3. **Revisit**
   - 在未来某个明确时点重新拉回；
   - review due / re-affirm / update / resolution。

4. **Learn across decisions**
   - 不只看单条记录；
   - 查看长期 calibration、反复偏差、经常翻车的条件和判断模式。

这比“建一个可搜索的日志库”更重要。

### 14.2 Metaculus：判断不是一次提交，而是持续更新的时间序列

Metaculus 的 forecasting 工作流具有几个值得注意的机制：

- 问题在创建时就有明确 resolution criteria；
- 用户给出精确概率，而不是模糊词；
- 在问题关闭前可以随时更新预测；
- 即使观点没有变化，也可以 re-affirm；
- 预测如果长时间不更新，会自动 withdrawal，减少 stale forecast 对当前判断的影响；
- 每次预测最终都进入个人 track record；
- track record 展示 calibration curve、分数分布、长期趋势。

核心思想：

> 判断不是一个静态结论，而是一条 belief trajectory。

真正有价值的信息不仅是：
> “最后我猜了 70%。”

还包括：
> 我什么时候从 40% 调到 55%，又因为什么证据升到 70%。

这对我们很重要，因为“根据新证据及时更新”本身就是判断能力。

### 14.3 Forecasting 平台解决了一个 Decision Journal 常见问题：resolution 必须预先定义

传统日记很容易写：
> “我觉得这个工作应该还不错。”

半年后根本不知道怎样算“判断对了”。

Metaculus 强制问题具备客观 resolution criteria。

对个人决策训练的启示：

> 不是所有人生问题都能量化，但凡是可以验证的部分，最好在事前明确“什么事件发生后可以认为这个判断被检验”。

例如：
> “新项目三个月内是否会延期超过两周”
比：
> “我觉得项目节奏很差”
更容易产生有效反馈。

### 14.4 Immutable / Append-only 是非常稳定的设计模式

多个独立 Decision Journal / Decision Record 项目都采用类似原则：

- 原始 context、reasoning、assumption 不覆盖；
- 后续 reflection 通过 timestamped layers 追加；
- 决策被 reversed / superseded 时，新建后继记录并引用旧记录。

原因不是技术审计，而是认知审计：

> 如果允许事后修改原始理由，就会把 hindsight bias 写进数据本身。

因此对个人思维训练而言：
- “当时我怎么想”；
- “后来我怎么看”；

必须是两个不同对象。

### 14.5 Review date 是“日志不变坟场”的第一道机制

成熟/新兴 Decision Journal 项目反复出现：
- expected outcome；
- review date；
- due-for-review；
- overdue review；
- reminders；
- weekly digest。

DecisionOS 甚至把 overdue reviews、upcoming reviews 做成单独页面，并通过 Slack DM / email 拉回负责人。

这说明：

> 单纯保存没有闭环，必须存在未来触发器。

对个人系统而言，一个判断记录如果没有：
- resolution event；
- review date；
- 或现实事件触发；

很容易永远不再被看见。

### 14.6 Metaculus 的 re-affirm 机制比“定期复盘”更细

一个很值得借鉴的概念是 re-affirm：

> 我重新看过了，但观点没变。

这和“什么都没发生”不同。

因为它把：
- 没有重新检查；
- 检查后仍然维持判断；

区分开来。

Metaculus 甚至会对陈旧预测自动 withdrawal，以减少 stale beliefs。

对个人思维训练来说，这是一个重要认识：

> “没有修改观点”也应该区分成：
> 1. 我没重新看；
> 2. 我重新看过，仍然认为原判断成立。

### 14.7 Decision Journal 的真正价值不是单条复盘，而是 longitudinal pattern

个人 Decision Journal 类工具常见的长期分析包括：
- confidence vs outcome；
- mental state vs accuracy；
- category-specific patterns；
- reversal rate；
- high-confidence failures；
- reflection rate；
- recurring assumptions / biases。

例如一些 2026 开源 Decision Journal 已经显式做：
- 高确信翻车高亮；
- 确信度 × 准确度；
- 情绪 × 准确度；
- 预判偏差与结果归因；
- 批量导出多条决策给 AI 分析模式。

因此真正的长期价值可能不是：
> “这一条我学到了什么。”

而是：
> “过去一年，我在哪类问题上反复过度自信？”
> “什么情绪状态下我的判断最差？”
> “我是不是经常低估执行成本？”
> “哪些模型我经常误用？”

### 14.8 不应该记录所有决定

这是对“日志坟场”问题的重要推论。

如果所有日常小决定都进入系统：
- review backlog 会迅速膨胀；
- 用户很快停止复盘；
- 高价值判断被噪声淹没。

DecisionOS 等系统使用 impact level；很多 decision record 方法也强调只记录 consequential decisions。

因此未来可能需要一个 capture threshold：
> 什么判断值得进入长期学习闭环？

候选标准：
- 后果明显；
- 不确定性高；
- 不可逆 / 代价高；
- 未来可验证；
- 涉及重复出现的判断模式；
- 用户明确想训练某种模型。

### 14.9 记录摩擦不是越低越好，也不是越高越好

长期日记研究（EMA / mobile EMA）显示：
- 短期 repeated assessment 的 compliance 可以达到约 79%–82%；
- 但不同协议之间异质性很高；
- prompt 数、项目数、时长等设计变量并不能简单解释依从性；
- 更长时间段在部分群体中会降低 compliance。

这说明：
> “把记录表单做得超级短”并不能保证长期使用；
> “每天提醒几次”也不是简单越少越好。

对我们的意义是：
- 应尽量只在有真实认知价值时要求用户记录；
- 不能把每日 streak 当成核心机制；
- review trigger 应和决策生命周期绑定，而不是单纯日历签到。

### 14.10 “完整记录”与“低摩擦捕获”需要分层

DecisionOS 的一个有趣方向是 quick capture：
- 先快速记录 title + rationale；
- 之后再补完整结构。

Sage 等项目则把低摩擦、append-only 作为核心。

这提示：
> 决策发生时，用户未必有耐心填写十几个字段。

可能更合理的是两个阶段：
- **Capture**：冻结最低必要信息；
- **Deepen**：真正准备训练/复盘时再补 evidence、models、alternatives、probability。

但这仍需实验，不能直接定成产品方案。

### 14.11 搜索不是核心，Recall Back Into Context 才是

大多数 Decision Journal 都有：
- tags；
- full-text search；
- filters；
- timeline。

这些很容易做，却不能自动产生学习。

真正能让过去记录产生价值的机制是：
- 到期复盘；
- 相似新决策出现时召回过去案例；
- 高置信翻车模式重新出现时提醒；
- 某个模型训练时召回过去真实案例。

也就是说：

> 重点不是“我以后能找到旧记录”，
> 而是“当旧经验再次相关时，系统能不能把它带回来”。

这是传统知识库与判断训练系统的关键区别之一。

### 14.12 AI 的长期角色更可能是“跨记录找模式”，而不是替每一条做决定

单条判断上，AI 有认知外包风险。

但在积累几十甚至几百条历史记录后，AI 有一种人类手工很难完成的价值：
- 找反复出现的 assumptions；
- 比较相似决策；
- 找模型使用模式；
- 发现高置信翻车聚类；
- 找“当时条件相似，但你两次做法完全不同”的 inconsistency。

因此 AI 的高杠杆场景可能发生在：
> 用户已经留下原始思考之后，对跨时间数据做 second-order analysis。

这比“每次先问 AI 怎么做”更符合 Phase 1 的目标。

### 14.13 当前关于“避免日志坟场”的机制假设

目前可归纳为：

> **Selective Capture**
> 只记录值得学习的判断
>
> → **Freeze Original State**
> 保留当时上下文、假设、置信度
>
> → **Explicit Future Trigger**
> review date / resolution event / stale check
>
> → **Update, Don't Rewrite**
> 新证据产生 belief update，而不是修改旧结论
>
> → **Resolve**
> 能验证的部分真正揭晓
>
> → **Reflect**
> 区分逻辑错误、执行问题、随机性、遗漏变量
>
> → **Cross-case Pattern Mining**
> 看长期 calibration、bias、model-use pattern
>
> → **Recall Into Future Decisions**
> 相似问题再次出现时，把旧经验带回当前情境

这比“记日记 → 偶尔看看”完整得多。

### 14.14 当前一个重要的产品原则候选

> **A record should have a future.**

如果一条记录没有任何未来触发方式：
- 不会 resolve；
- 不会 review；
- 不会在相似场景被召回；
- 不会进入跨记录分析；

那么它很可能只是在制造数字垃圾。

这是 Phase 2 当前很强的 Product Principle 候选，但还未正式进入 Product Hypothesis。

### 14.15 还没有解决的问题

1. 怎样决定哪些现实问题值得 capture？
2. 对没有明确 outcome 的人生决策，review 如何定义？
3. 怎样归因“判断错了” vs “执行错了” vs “随机事件”？
4. 相似历史案例应该自动召回还是由用户主动搜索？
5. AI 跨记录分析怎样避免事后合理化？
6. 长期使用中应该多频繁触发 review，才不会变成新的负担？
7. 真实事件和训练案例之间如何互相转化？

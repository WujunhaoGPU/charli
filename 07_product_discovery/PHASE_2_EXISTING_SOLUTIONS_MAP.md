# Phase 2 — Existing Solutions Map

> Status: Working draft (2026-10-02)
>
> Purpose: Map existing products and open-source systems against the Phase 1 capability chain:
>
> **知道 → 想到 → 用出来 → 被纠正 → 迁移与内化**
>
> This is not a ranking. It is a coverage map.

## 1. Mental model learning products

### Mind Models
- 50+ mental models
- personalized learning path
- streaks
- spaced repetition
- one-model-per-session learning

Coverage:
- 知道：强
- 想到：弱-中
- 用出来：弱
- 被纠正：弱
- 迁移与内化：弱-中

Main strength:
- model discovery + retention.

Main gap:
- does not visibly center real-world open-ended retrieval, model discrimination, longitudinal decision review, or reality-based feedback.

### ThinkingKit
- interactive mental model / decision framework library
- scenario-oriented discovery
- interactive tools
- tracks models learned/applied

Coverage:
- 知道：强
- 想到：中
- 用出来：中
- 被纠正：弱
- 迁移与内化：弱-中

Main strength:
- bridges library → guided application better than a pure model encyclopedia.

Main gap:
- still framework-centric; limited evidence of long-term calibration, case abstraction, or closed-loop real-world review.

### Reframo / MindModels.net
- mental-model guides
- real-world examples
- prompts / interactive application
- scenario/category filtering

Coverage:
- 知道：强
- 想到：中
- 用出来：中
- 被纠正：弱
- 迁移与内化：弱

Main strength:
- low-friction access to models and use cases.

Main gap:
- little visible support for feedback loops, personal case memory, spontaneous retrieval testing, or long-term calibration.

## 2. Research-backed thinking / decision training

### Clearer Thinking
- 80+ interactive tools
- calibration training
- sunk-cost training
- mental traps
- decision advisor
- fail-safing
- quarterly life review
- personalized paths

Coverage:
- 知道：中-强
- 想到：中
- 用出来：中-强
- 被纠正：中
- 迁移与内化：中

Main strength:
- unusually broad coverage of decision-making and critical-thinking micro-skills;
- interactive rather than article-only;
- some longitudinal progress tracking.

Main gap:
- skill modules remain relatively separated;
- limited visible evidence of a persistent personal case network connecting real decisions, models, outcomes, and future retrieval.

## 3. Decision journal systems

### DecisionJournal.ai
- capture reasoning before outcome
- expected outcome / review later
- conversation-style workflow

Coverage:
- 知道：弱
- 想到：弱
- 用出来：中
- 被纠正：强
- 迁移与内化：中

Main strength:
- freezes pre-outcome reasoning and creates review loop.

Main gap:
- assumes the user already knows how to analyze the problem;
- not a systematic model-learning or model-selection trainer.

### SifisoScS/decision-journal
- immutable decision logs
- layered reflections
- confidence calibration
- outcome trends
- timeline
- guided reflection prompts

Coverage:
- 知道：弱
- 想到：弱
- 用出来：中
- 被纠正：强
- 迁移与内化：中

Main strength:
- preserves evolution of thought instead of rewriting the past.

Main gap:
- reflection system, not a full reasoning-training environment.

### YINJIE99/decision-journal
- self-written pre-mortem before AI
- AI supplements blind spots after user work
- separates judgment from luck
- two-round confidence capture

Coverage:
- 知道：弱
- 想到：中
- 用出来：中-强
- 被纠正：强
- 迁移与内化：中

Main strength:
- explicitly protects against cognitive offloading;
- unusually aligned with “user first, AI challenge later.”

Main gap:
- small structured decision journal, not broad model learning / transfer training.

### sinameraji/decision-journal-electron
- local-first, offline, encrypted
- decision → months-later outcome review
- private data for career / relationship / money / risk decisions

Coverage:
- 知道：弱
- 想到：弱
- 用出来：中
- 被纠正：强
- 迁移与内化：中

Main strength:
- privacy + long-term review discipline.

Main gap:
- journal-centered rather than training-centered.

## 4. Forecasting / calibration platforms

### Metaculus
- explicit probability forecasts
- precise resolution criteria
- forecast revision over time
- re-affirm
- auto-withdraw stale forecasts
- calibration curve
- score history / track record

Coverage:
- 知道：弱
- 想到：中
- 用出来：强 for probabilistic judgment
- 被纠正：强
- 迁移与内化：强 within forecasting

Main strength:
- the clearest mature implementation of “belief trajectory + reality feedback + calibration.”

Main gap:
- narrow task type: forecastable questions;
- does not train broad mental-model selection, human relations, or open-ended personal decisions.

## 5. Socratic AI tutors

### Socra
- Socratic dialogue
- recall / explain / reason in own words
- blind-spot detection
- reusable notes

### Guided
- guiding questions and hints instead of finished solutions
- stepwise understanding checks

### AcademiChat
- Socratic guided dialogue
- reasoning explanation
- assumption challenge
- automated grading schemas

Coverage as a category:
- 知道：中
- 想到：中-强
- 用出来：强
- 被纠正：强
- 迁移与内化：尚不明确

Main strength:
- high-frequency guided feedback without immediately giving the answer.

Main gap:
- usually curriculum/topic centered;
- weak visible linkage to long-term personal decisions, future outcomes, cross-case pattern mining, or spontaneous open-world retrieval.

## 6. Argumentation / debate systems

### Toulmin Lab
- claim / grounds / warrant / backing / qualifier / rebuttal
- AI coach asks questions instead of writing
- argument construction from scratch

### Symbai
- argument mapping + debate
- AI-powered practice
- progress measurement

### Toron
- AI debate opponent
- drills and full rounds
- real-time coaching
- post-session report card

Coverage as a category:
- 知道：中
- 想到：中
- 用出来：强
- 被纠正：强
- 迁移与内化：中

Main strength:
- makes reasoning structure explicit;
- trains counterargument, rebuttal, evidence, persuasion.

Main gap:
- argument quality is not the same as overall judgment quality;
- weak linkage to models, real-life decisions, outcome resolution, and calibration.

## 7. Domain-specific case reasoning trainers

### Atrium / Meksi Clinical Reasoning
- simulated cases
- information gathering
- decision selection
- reflection on outcomes
- reasoning scorecard / structured feedback

Coverage as a category:
- 知道：中
- 想到：强
- 用出来：强
- 被纠正：强
- 迁移与内化：强 within domain

Main strength:
- probably the closest mature pattern to “practice reasoning, not just memorize content.”

Main gap:
- works because the domain supplies:
  - known competency targets
  - expert models
  - constrained scenarios
  - clearer feedback standards

That scaffolding is much weaker in open-ended life reasoning.

## 8. Coverage matrix

| Category | 知道 | 想到 | 用出来 | 被纠正 | 迁移/内化 | Real-life longitudinal loop |
|---|---|---|---|---|---|---|
| Mental model apps | 强 | 弱-中 | 弱-中 | 弱 | 弱-中 | 弱 |
| Clearer Thinking | 中-强 | 中 | 中-强 | 中 | 中 | 弱-中 |
| Decision journals | 弱 | 弱-中 | 中 | 强 | 中 | 强 |
| Metaculus | 弱 | 中 | 强 | 强 | 强(预测域) | 强 |
| Socratic tutors | 中 | 中-强 | 强 | 强 | 未明 | 弱 |
| Argumentation systems | 中 | 中 | 强 | 强 | 中 | 弱 |
| Domain case trainers | 中 | 强 | 强 | 强 | 强(领域内) | 中 |

## 9. What existing products already solve well

Existing systems already solve many pieces well:

1. **Model discovery / retention**
   - mental-model apps + SRS.

2. **Interactive micro-skill practice**
   - Clearer Thinking.

3. **Freeze pre-outcome reasoning**
   - decision journals.

4. **Reality-based probabilistic calibration**
   - Metaculus.

5. **Socratic challenge**
   - AI tutor products.

6. **Argument structure**
   - Toulmin Lab / Symbai / debate trainers.

7. **Case-based reasoning + feedback**
   - clinical reasoning trainers.

Therefore, “build another model library,” “build another generic Socratic chatbot,” or “build another decision journal” would likely duplicate mature partial solutions.

## 10. Main coverage gaps

### Gap A — Cross-domain spontaneous retrieval
Few systems visibly test:
> In an open real-world problem with no model list, does the user independently retrieve useful models?

### Gap B — Model discrimination and combination
Few products train:
> Which model fits, which does not, and when multiple models should be combined.

### Gap C — Real experience ↔ training transformation
Decision journals store experiences.
Case trainers provide synthetic cases.
Mental-model apps teach abstractions.

Few systems visibly connect:
> personal real event → abstraction → synthetic variants → transfer test → future real event.

### Gap D — Multi-track correction
Existing products tend to specialize:
- forecasting → calibration
- argument tools → argument structure
- journals → retrospective review

Few integrate:
- structural correction
- evidence correction
- confidence correction
- reality correction

### Gap E — Longitudinal personal reasoning model
Few systems build an evolving view of:
- recurring blind spots
- model misuse
- high-confidence failure patterns
- domains of overconfidence
- changing belief trajectories
- recurring decision structures

### Gap F — AI without cognitive offloading
Some systems explicitly protect user-first reasoning, but this is not yet a universal mature pattern.

The unresolved design problem is:
> how to exploit AI for challenge, comparison, variation and cross-record pattern mining without letting it become the first thinker.

## 11. Strongest Phase 2 finding so far

No single product found so far appears to combine all of these as its core loop:

> **learn models**
> → **compare cases**
> → **retrieve without labels**
> → **select / combine models**
> → **apply to real problems**
> → **record original judgment**
> → **receive structured challenge**
> → **observe reality**
> → **calibrate**
> → **abstract personal cases**
> → **generate cross-domain variants**
> → **recall the experience in future decisions**

This does not prove that no such product exists.

It does suggest the whitespace is not “mental models” in general, but the **integration between training, real-world reasoning, feedback, and longitudinal personal learning**.

## 12. Do Nothing / Tool Combination is already viable

A credible non-product solution can be assembled today:

- mental-model learning: Mind Models / ThinkingKit / Reframo
- interactive decision skills: Clearer Thinking
- probability calibration: Metaculus
- real decisions: Decision Journal
- Socratic challenge: ChatGPT / Socratic tutor
- notes / history: Markdown / Notion / Obsidian

This is important for Phase 3:

> A new product must outperform this combination on integration, continuity, cognitive load, feedback quality, or transfer.

Otherwise there is no strong reason to build it.

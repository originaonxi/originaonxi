# Sam Anmol

**CTO @ Aonxi · Santa Monica, CA**
Ex-Meta Ads ML (billions of decisions/day) · Ex-Apple Face ID (500M devices)
origin@aonxi.com · aonxi.today · [linkedin.com/in/samisanmol](https://linkedin.com/in/samisanmol)

---

> I am building the world's first AGI agent for revenue and capital.
>
> Not a chatbot. Not a copilot. An autonomous system that researches,
> decides, acts, learns, and compounds — the way a senior operator
> would, but at infinite scale and zero marginal cost.
>
> The lab is not a university. It is a live production system
> generating $650K ARR. Every experiment runs on real money,
> real prospects, real outcomes. That is the only eval that matters.

---

## What I am building

### Aonxi — Autonomous Revenue Agent

Most revenue tools are databases pretending to be engines.
Aonxi is a living revenue engine.

The agent wakes up every morning, finds the right companies,
researches each one using 30+ data sources, writes a
hyper-personalized email proving it did the research,
scores intent using dual-LLM judgment, and sends.
You review. You approve. Meetings land on your calendar.
You pay per meeting. No SDR. No guessing. No waste.

**Production numbers — real, not projected:**

| Month    | Leads | Meetings | Sales | ARR      | Meet→Sale | Lead→Sale |
|----------|-------|----------|-------|----------|-----------|-----------|
| Oct 2025 | 360   | 42       | 5     | $314,472 | 11.9%     | 1.39%     |
| Nov 2025 | 647   | 51       | 4     | $361,092 | 7.8%      | 0.62%     |
| Dec 2025 | 138   | 27       | 9     | $491,592 | 33.3%     | 6.52%     |
| Jan 2026 | 288   | 26       | 4     | $386,592 | 15.4%     | 1.39%     |
| Feb 2026 | 408   | 42       | 8     | $484,508 | 19.9%     | 2.02%     |
| Mar 2026 | 611   | 62       | 12    | $650,458 | 19.9%     | 2.02%     |

**$650K ARR. 5 months. $0 raised. Bootstrapped. Organic.**

The December anomaly is the most important data point:
138 leads produced 9 sales (33.3% meet→sale).
November had 647 leads and only 4 sales (7.8%).
**10.5x efficiency difference. Same agent. Same verticals.**
The agent had no memory of why December worked.
That single observation became a research program.

---

## The research program

I do not separate research from production.
Every paper I replicate gets deployed into a live system
and tested against real outcomes. This is the laboratory.

### Why these papers matter for AGI

The path to AGI is not bigger models.
It is agents that can operate reliably over long horizons —
planning across steps, remembering what mattered,
recovering from failure, and improving without human input.

Every paper below attacks one part of that problem.
Every replication I build tests whether the theory
holds when money is on the line.

---

### Paper 1 — ASM-Outreach
**Anchored State Memory for Multi-Session Autonomous Revenue Agents**
*Domain transfer of AndroTMem (arxiv:2603.18429, March 2026)*
**Target: NeurIPS 2026**

**Why it matters for AGI:**
Long-horizon agents fail primarily because of memory failures,
not intelligence failures. AndroTMem proved this on 1,069
Android GUI tasks: as step count grows, agents forget
causally important intermediate states. They repeat mistakes.
They lose track of dependencies. They think they are making
progress when they are not.

This is not a GUI problem. It is a fundamental agent problem.
An AGI that forgets why something worked cannot improve.

**My contribution over the paper:**
The original handles single-session tasks (max 65 steps).
I handle multi-session campaigns (6 months, 2,452 leads).
First production validation of ASM on real financial outcomes.

**Real experiment results:**

| Condition       | Avg Score | Beats Raw | Calibration Gap |
|-----------------|-----------|-----------|-----------------|
| Raw (no memory) | 6.67/10   | —         | 1.33            |
| Coarse summary  | 7.17/10   | —         | —               |
| ASM (ours)      | 7.67/10   | 83%       | 1.67 ✓          |

ASM beats raw scoring on 83% of prospects.
The December "quality over quantity" insight now lives
as a causal anchor. The agent retrieves it every time
it scores a similar prospect. It will never repeat
November again.

→ [github.com/originaonxi/asm-replication](https://github.com/originaonxi/asm-replication)

---

### Paper 2 — TDAD Replication
**Trajectory-Driven Agent Design**
*Replication + extension*

**Why it matters for AGI:**
Trajectory data is the ground truth of agent behavior.
Not what the agent said it would do — what it actually did,
step by step, under real conditions.
TDAD formalizes how to design agents whose trajectories
remain coherent across long horizons.
For AGI: coherent trajectories are how you verify
an agent is actually reasoning, not pattern-matching.

→ [github.com/originaonxi/tdad-replication](https://github.com/originaonxi/tdad-replication)

---

### Paper 3 — PRM Replication
**Process Reward Models**
*Replication + extension*

**Why it matters for AGI:**
Outcome reward is not enough. An agent that only learns
from final results cannot improve the quality of its
reasoning process. PRM rewards intermediate steps —
it teaches the agent to think well, not just to get lucky.
For AGI: you cannot scale intelligence without
rewarding the quality of the reasoning chain itself.

→ [github.com/originaonxi/prm-replication](https://github.com/originaonxi/prm-replication)

---

### Paper 4 — RewardFlow Replication
**Multi-step reward propagation in agentic pipelines**
*Replication + extension*

**Why it matters for AGI:**
Single-step reward is local. RewardFlow propagates
reward signals across the full action chain —
crediting or penalizing decisions that caused
outcomes several steps later.
For AGI: an agent that cannot attribute causality
across time cannot learn from complex outcomes.
Revenue attribution IS RewardFlow in the wild.

→ [github.com/originaonxi/rewardflow-replication](https://github.com/originaonxi/rewardflow-replication)

---

### Paper 5 — Information Architecture Thesis
**Long-horizon agent state management**

**Why it matters for AGI:**
State is the unsolved problem of production agents.
What information do you keep? What do you compress?
What do you discard? How do you structure it so
retrieval is fast, relevant, and causally grounded?
This thesis formalizes the information architecture
decisions that determine whether an agent stays
coherent over thousands of steps.

→ [github.com/originaonxi/information-architecture-thesis](https://github.com/originaonxi/information-architecture-thesis)

---

## The AGI thesis

I think about AGI every day. Here is what I actually believe:

**The bottleneck is not intelligence. It is reliability.**

GPT-4 can reason. Claude can reason. Gemini can reason.
None of them can operate a live business autonomously
for 6 months without accumulating failures that compound.

The path to AGI runs through:

**1. Memory that survives sessions**
Not context windows. Structured causal anchors.
What happened, what caused it, what it means for next time.
ASM is the first architecture that formalizes this.
I am validating it in production.

**2. Reward that propagates through time**
Not "did this email get a reply" but "did this decision
pattern produce meetings across 6 months of campaigns."
PRM + RewardFlow are the theoretical foundation.
My production data is the experimental ground truth.

**3. Trajectories that stay coherent**
An AGI that drifts off its intended path after
100 steps is not AGI — it is a very expensive random walk.
TDAD gives us the framework to measure and enforce coherence.
I measure it every day with real campaign data.

**4. Human-in-the-loop as a feature, not a patch**
The HAGI (Human-AGI Interface) architecture I built into
Aonxi is not a safety hack. It is a learning signal.
Every time a human approves or rejects an agent decision,
the agent gets a real-world preference signal.
That is RLHF running live in production, continuously.

**The world's first AGI agent for revenue and capital**
is not science fiction. It is the logical endpoint of
exactly what I am building right now:
Memory (ASM) +
Process Reward (PRM) +
Causal Attribution (RewardFlow) +
Coherent Trajectories (TDAD) +
Human Feedback (HAGI loop) +
Production data (Aonxi $650K ARR)
= An agent that improves itself continuously,
operates reliably over months,
attributes outcomes to decisions,
and gets better every single day
without human intervention.

That is AGI for a bounded domain.
Revenue and capital is the domain I chose
because it has the clearest eval:
did the meeting happen? did the deal close?
No ambiguity. No cheating the metric.

---

## What I do every day
Morning:    Read one new paper or arxiv preprint
            Run aonxi-outreach (20+ new emails sent)
Afternoon:  Review replies, close clients
            aonxi-sequence (follow-up emails)
Evening:    Build or improve one thing
            Push to GitHub
Weekly:     Write up what I learned
            Update paper outline with new data
Always:     Connect every paper I read to a
            real experiment I can run on
            production data

I am not reading papers to understand them.
I am reading papers to deploy them.
The production system is the lab.
The ARR is the p-value.

---

## Papers on my desk right now

| Paper | Why I am reading it |
|-------|---------------------|
| AndroTMem (2026) — arxiv:2603.18429 | Active replication → NeurIPS 2026 |
| Constitutional AI — Anthropic, 2022 | HAGI loop design, preference learning |
| LoRA — Microsoft, 2021 | Fine-tuning persona models on production data |
| ReAct — Google, 2022 | Reasoning + acting loops in live agent |
| Toolformer — Meta, 2023 | Tool use architecture for 30+ source agent |
| Sleeper Agents — Anthropic, 2024 | Alignment in long-running production agents |
| PRM — OpenAI | Process reward in multi-step outreach decisions |

---

## Stack
Agent core:    Python · Anthropic API (Claude Haiku/Sonnet)
               Grok API · dual-LLM scoring
Discovery:     Apollo · Exa · Hunter · 30+ source waterfall
Memory:        SQLite ASM anchor bank · Airtable sync
Delivery:      Gmail SMTP · SendGrid
Research:      PyTorch · vLLM · Qdrant (vector retrieval)
Infra:         Kubernetes · Temporal.io (durable execution)
Observability: Custom revenue attribution dashboard

---

## All repos

| Repo | What it is | Status |
|------|-----------|--------|
| [asm-replication](https://github.com/originaonxi/asm-replication) | Multi-session ASM. NeurIPS 2026. Real data. | Active |
| [information-architecture-thesis](https://github.com/originaonxi/information-architecture-thesis) | Long-horizon agent state management | Published |
| [tdad-replication](https://github.com/originaonxi/tdad-replication) | TDAD paper replication | Published |
| [prm-replication](https://github.com/originaonxi/prm-replication) | Process Reward Model replication | Published |
| [rewardflow-replication](https://github.com/originaonxi/rewardflow-replication) | RewardFlow replication | Published |
| [blueprint-trust-engine](https://github.com/originaonxi/blueprint-trust-engine) | Trust scoring for agent decisions | Published |
| [agi-possible-agent](https://github.com/originaonxi/agi-possible-agent) | AGI architecture experiments | Active |
| aonxi-outreach-agent | Production autonomous revenue agent | Private |

---

## Numbers

| Metric | Number |
|--------|--------|
| ARR | $650,458 |
| Months to get there | 5 |
| Funding raised | $0 |
| Total leads processed | 2,452 |
| Meetings booked | 250 |
| Sales closed | 42 |
| ASM beats raw scoring | 83% of prospects |
| Papers replicated | 4 + 1 thesis |
| NeurIPS 2026 submissions | 1 (in progress) |
| Papers read this month | ongoing |

---

## If you are building at the frontier

I want to talk to people working on:
- Long-horizon agent reliability
- Production evals that use real outcomes
- Memory architectures beyond context windows
- RLHF from live human-in-the-loop systems
- AGI that operates in bounded real-world domains

origin@aonxi.com · aonxi.today

Santa Monica, CA · Shipping every day

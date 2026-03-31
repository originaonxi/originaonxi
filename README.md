# Sam Anmol (Anmol Chaudhary)

ML + AGI Agent Engineer · Ex-Meta Ads ML · Ex-Apple Face ID · 
---

> **AGI agents are not chatbots. They are not copilots.**
>
> They are revenue-making, P&L-responsible autonomous systems
> that compound value the way a senior operator would -
> but at infinite scale and zero marginal cost.
>
> Imagine giving your agent an unlimited corporate credit card.
> It can buy any API, spin up GPUs, run experiments, hire compute.
> But it must bring qualified meetings, pipeline, and closed-won revenue.
> Every dollar it spends must return more dollars than it cost.

---

## The vision I am executing

Most people talk about AGI in the abstract.
I am building it in the concrete - one bounded domain at a time.

The domain I chose is revenue and capital. GTMe (AI GTM Engineer) 
not because it is easy. Because it has the clearest eval in existence:

**Did the meeting happen? Did the deal close? Did money land in the bank?**

No ambiguity. No benchmark gaming. No cherry-picked demos.
The production system is the laboratory.
**The ARR is the p-value.**

---

## What makes this possible

At Meta I shipped ranking and bidding models at billions of daily inferences.
At Apple I reduced Face ID false positives by 15% and published the GAN refiner
that made synthetic training viable (machinelearning.apple.com/research/gan).
At Lotus Interworks I took ARR from $25K to $4M in 9 months,
cut the sales cycle from weeks to under 5 days, and lifted close rate from 10% to 34%.
At Aonxi I built the agent from scratch. Alone. $0 raised. $199K collected. $8K peak day. $2.9M ARR velocity in 60 days of launch fully autonomous money making agent. 
Creating AGI agents in education/coaching now.  

The combination nobody else runs at scale:
**Deep ML research + agent systems engineering + production revenue data**

I replicate frontier papers the week they drop.
I deploy the architecture into the live system.
I measure whether the theory holds when money is on the line.
If it does not, I fix it or throw it out.

---

## The guardrails that make it safe

An agent with an unlimited credit card and no constraints is not AGI.
It is a liability.

The architecture I engineered to keep it safe, auditable, and production-grade:

**Multi-agent swarms with 4-layer quality gates**
No single agent makes a final decision.
Every action passes through intent verification, confidence scoring,
compliance checking, and human escalation logic before execution.

**Human-in-the-loop (HITL) nodes everywhere**
Y/N vetoes. Approval gates. Override controls. Rich feedback loops.
Every human decision becomes a training signal.
Low-confidence cases escalate to humans automatically.
Human labels feed continuous iteration.
This is RLHF running live in production, every day.

**Uncertainty-based routing**
When the agent is not sure, it asks.
When it is sure and wrong, it learns.
The confidence threshold for autonomous action rises
only when production eval data supports it.

**Economic ledger with hard gates**
Every execution logs cost per task, variance, and outcome delta.
Scaling is gated on probabilistic ROI - not task success percentage.
No logs, no scale. No proven ROI, no autonomy increase.

**Kill switches at every layer**
Agents are stateless and short-lived.
They can be terminated mid-task without corruption.
The orchestrator owns workflow state - not the agents.
This means I can pull the plug on anything, instantly, at any layer.

Winners auto-replicate and compound.
Losers terminate with zero drama.
**Better data beats better algorithms.** I have lived this truth at Meta scale.

---

## The research program

Every paper I read gets deployed.
Every architecture I replicate gets tested on production revenue data.
Here is what I am working from and why each one matters for AGI:

## Super Brain — The Connective Tissue

50+ repos. All connected. All learning from each other.

**[super-brain](https://github.com/originaonxi/super-brain)** — The living memory + orchestrator connecting every repo, agent, and engine into one unified intelligence layer. V2 now live.

- Complete registry of all 50+ repos with dependency graph
- Daily health checks, pattern detection, improvement suggestions
- Cross-repo learning: what AROS learns, ARIA inherits immediately
- Hybrid memory: Mem0 cloud + MemoryMesh local SQLite
- Orchestrator scans at 5am daily — reports without human input

**The compound loop:**
Research improves agents → Agents generate production data → Data improves research → Brain detects patterns → Every repo gets smarter → Repeat forever.

---

## All repos

**Core (shared infrastructure)**

| Repo | What it is | Status |
|------|-----------|--------|
| [super-brain](https://github.com/originaonxi/super-brain) | Living memory + orchestrator — connects all 50+ repos | Live |
| [aonxi-router](https://github.com/originaonxi/aonxi-router) | Intelligence routing — best model for every task | Live |
| [aonxi-safeguard](https://github.com/originaonxi/aonxi-safeguard) | Behavioral integrity — 0.42% breaks vs 99.6% earns | Live |
| [aonxi-memcollab](https://github.com/originaonxi/aonxi-memcollab) | Cross-agent shared memory — every AROS win teaches ARIA | Live |
| [aonxi-claw](https://github.com/originaonxi/aonxi-claw) | Living orchestrator — all agents self-optimize | Live |
| [aonxi-pkm](https://github.com/originaonxi/aonxi-pkm) | PKM content flywheel — feeds AROS, ARIA, Outreach | Live |
| [memorymesh](https://github.com/originaonxi/memorymesh) | Shared memory for all AI tools. pip install memorymesh. | Live |

**Revenue & Capital**

| Repo | What it is | Status |
|------|-----------|--------|
| [aros-agent](https://github.com/originaonxi/aros-agent) | Autonomous Revenue Operating System — finds new revenue | Live |
| [ARIA](https://github.com/originaonxi/ARIA) | Autonomous Relationship Intelligence — finds capital | Live |
| [aonxi-outreach-agent](https://github.com/originaonxi/aonxi-outreach-agent) | Self-correcting outreach v8 — $200K proved | Live |
| [pkm-analyzer](https://github.com/originaonxi/pkm-analyzer) | Defense profiling — [try live](https://originaonxi.github.io/pkm-analyzer/) | Live |

**GTM Engines**

| Repo | What it is | Status |
|------|-----------|--------|
| [nova-gtm](https://github.com/originaonxi/nova-gtm) | 17-agent progressive autonomy GTM. $2M ARR/60 days. | Live |
| [simplenursing-gtm-engine](https://github.com/originaonxi/simplenursing-gtm-engine) | 4.38M nursing student TAM engine | Live |
| [techm-intel](https://github.com/originaonxi/techm-intel) | F500 account intelligence — C-suite mapping, real-time | Live |
| [attentive-gtm-agent](https://github.com/originaonxi/attentive-gtm-agent) | AI outbound for Attentive.ai — 5 agents, 5 verticals | Live |
| [bre-gtm-engine](https://github.com/originaonxi/bre-gtm-engine) | GTM for BRE Group — £50B green building market | Live |
| [myhq-gtm-engine](https://github.com/originaonxi/myhq-gtm-engine) | India workspace sales — 25+ demand signals, 5 channels | Live |

**Daily Autonomous Fleet (cron)**

| Repo | Schedule | What it delivers |
|------|----------|-----------------|
| [news-briefing-agent](https://github.com/originaonxi/news-briefing-agent) | 6:30am PST | Bias-aware AI + startup news |
| [echo](https://github.com/originaonxi/echo) | 7:05am PST | Curated AI insights |
| [agi-possible-agent](https://github.com/originaonxi/agi-possible-agent) | 8:00am PST | 5 most AGI-relevant ML papers |
| [space-wonder-agent](https://github.com/originaonxi/space-wonder-agent) | Daily | Space/astronomy intelligence |
| [stock-analyst-agent](https://github.com/originaonxi/stock-analyst-agent) | Daily | Market intelligence |

**Research → Production (NeurIPS 2026 pipeline)**

| Repo | What it is | Status |
|------|-----------|--------|
| [asm-replication](https://github.com/originaonxi/asm-replication) | Multi-session ASM. NeurIPS 2026. Real revenue data ($199K). | Active |
| [moe-efficiency-study](https://github.com/originaonxi/moe-efficiency-study) | MoE routing paper. Original metric. Published. | Published |
| [information-architecture-thesis](https://github.com/originaonxi/information-architecture-thesis) | Long-horizon agent state management | Published |
| [tdad-replication](https://github.com/originaonxi/tdad-replication) | Trajectory-Driven Agent Design replication | Published |
| [prm-replication](https://github.com/originaonxi/prm-replication) | AI grades its own reasoning — proved | Published |
| [rewardflow-replication](https://github.com/originaonxi/rewardflow-replication) | Multi-step reward propagation | Published |
| [reward-model-blindness](https://github.com/originaonxi/reward-model-blindness) | RLHF rates for wrong reasons — and a fix | Published |
| [llm-calibration-study](https://github.com/originaonxi/llm-calibration-study) | LLM confidence on B2B email quality | Published |
| [llm-evals-arena](https://github.com/originaonxi/llm-evals-arena) | Production eval framework for B2B reasoning | Published |
| [alignment-auditor](https://github.com/originaonxi/alignment-auditor) | Do LLMs fake alignment under observation? | Live |
| [glassbox-agents](https://github.com/originaonxi/glassbox-agents) | Found 2 failure modes Anthropic didn't name | Live |
| [realtime-reasoning-engine](https://github.com/originaonxi/realtime-reasoning-engine) | Making AI reasoning transparent and auditable | Live |
| [attention-from-scratch](https://github.com/originaonxi/attention-from-scratch) | Transformer attention in pure PyTorch — every matrix explicit | Published |
| [frontier-agi-journey](https://github.com/originaonxi/frontier-agi-journey) | 365-day daily research log — 5 papers/day | Live |

**QA & Trust**

| Repo | What it is | Status |
|------|-----------|--------|
| [colibri-qa-agent](https://github.com/originaonxi/colibri-qa-agent) | AI QA replacing QA team at Colibri Group. 24/7. | Live |
| [blueprint-trust-engine](https://github.com/originaonxi/blueprint-trust-engine) | Trust-scored QA routing for Attentive.ai | Live |

**Products**

| Repo | What it is | Status |
|------|-----------|--------|
| [job-hunt-agent](https://github.com/originaonxi/job-hunt-agent) | 5-agent pipeline — 12 CTO emails in 34 min, $0.04 cost | Live |
| [b2b-funding-scanner](https://github.com/originaonxi/b2b-funding-scanner) | Real-time seed funding intelligence, 30 min cycle | Live |
| [ai-crypto-exchange](https://github.com/originaonxi/ai-crypto-exchange) | Open-source exchange with AI surveillance + circuit breakers | Live |
| [system-design-mastery](https://github.com/originaonxi/system-design-mastery) | 200-lesson system design course, cron delivery | Live |

---

## If you are building at the frontier

I want to talk to people working on:
- Long-horizon agent reliability in production
- Memory architectures beyond context windows
- RLHF from live human-in-the-loop systems
- Production evals where real outcomes are the metric
- AGI that operates in bounded real-world domains
- Agents that are P&L accountable, not just task-complete

Sam Anmol ·
Santa Monica, CA · Shipping every day since age 10

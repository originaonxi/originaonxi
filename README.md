# Sam Anmol (Anmol Chaudhary)

ML + AI Agent Engineer · Ex-Meta Ads ML · Ex-Apple Face ID · 
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
Not because it is easy. Because it has the clearest eval in existence:

**Did the meeting happen? Did the deal close? Did money land in the bank?**

No ambiguity. No benchmark gaming. No cherry-picked demos.
The production system is the laboratory.
**The ARR is the p-value.**

---

## What makes this possible

I am not a researcher who builds demos.
I am not a founder who hires engineers.
I am both - and I can connect everything to everything.

At Meta I shipped ranking and bidding models at billions of daily inferences.
At Apple I reduced Face ID false positives by 15% and published the GAN refiner
that made synthetic training viable (machinelearning.apple.com/research/gan).
At Lotus Interworks I took ARR from $25K to $4M in 9 months,
cut the sales cycle from weeks to under 5 days, and lifted close rate from 10% to 34%.
At Aonxi I built the agent from scratch. Alone. $0 raised. $199K collected. $8K peak day. $2.9M ARR velocity in 60 days of launch. 
AI in Education Now 

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

## All repos

| Repo | What it is | Status |
|------|-----------|--------|
| [asm-replication](https://github.com/originaonxi/asm-replication) | Multi-session ASM. NeurIPS 2026. Real revenue data. | Active |
| [moe-efficiency-study](https://github.com/originaonxi/moe-efficiency-study) | MoE routing paper. Original metric. Published. | Published |
| [information-architecture-thesis](https://github.com/originaonxi/information-architecture-thesis) | Long-horizon agent state management | Published |
| [tdad-replication](https://github.com/originaonxi/tdad-replication) | Trajectory-Driven Agent Design replication | Published |
| [prm-replication](https://github.com/originaonxi/prm-replication) | Process Reward Model replication | Published |
| [rewardflow-replication](https://github.com/originaonxi/rewardflow-replication) | RewardFlow replication | Published |
| [blueprint-trust-engine](https://github.com/originaonxi/blueprint-trust-engine) | Trust scoring for agent decisions | Published |
| [agi-possible-agent](https://github.com/originaonxi/agi-possible-agent) | AGI architecture experiments | Active |
| [aros-agent](https://github.com/originaonxi/aros-agent) | Revenue intelligence core + PKM | Live |
| [ARIA](https://github.com/originaonxi/ARIA) | Capital intelligence core + PKM | Live |
| [pkm-analyzer](https://github.com/originaonxi/pkm-analyzer) | Defense profiling — [try live](https://originaonxi.github.io/pkm-analyzer/) | Live |
| [aonxi-outreach-agent](https://github.com/originaonxi/aonxi-outreach-agent) | Hyper-personalized outreach + PKM | Live |
| [alignment-auditor](https://github.com/originaonxi/alignment-auditor) | AI alignment research | Live |
| [frontier-agi-journey](https://github.com/originaonxi/frontier-agi-journey) | Daily research log | Live |

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

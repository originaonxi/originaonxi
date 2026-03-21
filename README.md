# Sam Anmol (Anmol Chaudhary)

**ML + AI Agent Engineer · Ex-Meta Ads ML · Ex-Apple Face ID · CTO @ Aonxi**
Santa Monica, CA · origin@aonxi.com · aonxi.com · [linkedin.com/in/samisanmol](https://linkedin.com/in/samisanmol)

---

| 12M+ | 10 yrs | $650K ARR | 1000% |
|------|--------|-----------|------|
| Lines in production | F500 daily shipping | Aonxi in 5 months | ARR growth (2024) |

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
>
> That is not a demo. That agent exists. It is running right now.
> It generated $650K ARR in 5 months. Bootstrapped. Zero paid acquisition.
>
> I am the person who built it.
> And I am just getting started.

---

## The vision I am executing

Most people talk about AGI in the abstract.
I am building it in the concrete - one bounded domain at a time.

The domain I chose is revenue and capital.
Not because it is easy. Because it has the clearest eval in existence:

**Did the meeting happen? Did the deal close? Did money land in the bank?**

No ambiguity. No benchmark gaming. No cherry-picked demos.
The production system is the laboratory.
**The ARR is the p-value.**

---

### The full roadmap - already in motion at Aonxi

**Stage 1 (Live now): Lead outreach and discovery**
The agent wakes up every morning.
It searches 30+ data sources for companies matching the ICP.
It researches each one - funding news, hiring signals, product launches,
founder posts, acquisition events.
It writes a hyper-personalized email proving it did the research.
It scores intent using dual-LLM judgment (Claude + Grok, weighted average).
Human reviews. Human approves. Email sends.
Meetings land on the calendar.

**Stage 2 (Building now): Intelligent follow-up and sequencing**
Three-touch sequences. Fresh signals on each follow-up.
Reply detection via IMAP. Auto-routing of warm responses.
The agent learns which angles convert by vertical, size, signal combination.
Every outcome becomes an anchor in the memory bank.

**Stage 3 (Next): Shadow sales and learning**
The agent observes real sales calls.
It extracts objections, winning tactics, buyer psychology, pricing signals.
It builds a model of what closes - not from theory, from real conversations.
It feeds this back into outreach to close the loop between lead and close.

**Stage 4 (Coming): Sales assistance and co-piloting**
The agent co-pilots sales reps in real time.
Surfaces the right objection handler at the right moment.
Drafts follow-up emails while the call is still happening.
Escalates only when the deal size or complexity demands human judgment.

**Stage 5 (The destination): Full autonomy**
First touch to contract signed to money in the bank.
The agent runs the entire revenue funnel.
It spends more where results compound. Kills what does not work.
Requests human input only when it creates leverage.
Every decision is logged, attributed, and auditable.

This is AGI for a bounded domain.
I am building it step by step, in production, with real money on the line.

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
At Aonxi I built the agent from scratch. Alone. $0 raised. $650K ARR in 5 months.

The combination nobody else runs at scale:
**Deep ML research + agent systems engineering + production revenue data**

I replicate frontier papers the week they drop.
I deploy the architecture into the live system.
I measure whether the theory holds when money is on the line.
If it does not, I fix it or throw it out.

This is not how most researchers work.
This is not how most engineers work.
This is how you build AGI that actually does something.

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

---

### ASM-Outreach - Active replication → NeurIPS 2026
**AndroTMem (arxiv:2603.18429, March 2026)**

**The problem it solves:**
Long-horizon agents fail primarily because of memory failures.
Not intelligence. Memory.
As step count grows, agents forget causally important intermediate states.
They repeat November's mistakes in January.
They cannot learn from December's success.

**The December anomaly - real production data:**

| Month | Leads | Meetings | Sales | ARR | Meet→Sale | Lead→Sale |
|-------|-------|----------|-------|-----|-----------|-----------|
| Nov 2025 | 647 | 51 | 4 | $361K | 7.8% | 0.62% |
| Dec 2025 | 138 | 27 | 9 | $492K | 33.3% | 6.52% |

Same agent. Same verticals. 10.5x efficiency difference.
The agent had no idea why December worked.
That observation became this research program.

**My contribution over the paper:**
The original handles single-session tasks (max 65 steps).
I handle multi-session campaigns (6 months, 2,452 leads, 42 sales).
First production validation of ASM on real financial outcomes.

**Real experiment results:**

| Condition | Avg Score | Beats Raw | Calibration Gap |
|-----------|-----------|-----------|-----------------|
| Raw - no memory | 6.67/10 | - | 1.33 |
| Coarse summary | 7.17/10 | - | - |
| ASM - structured anchors | 7.67/10 | 83% | 1.67 ✓ |

ASM beats raw scoring on 83% of prospects.
The December "quality over quantity" insight lives as a causal anchor.
The agent retrieves it when scoring similar prospects.
It will never repeat November again.

→ [github.com/originaonxi/asm-replication](https://github.com/originaonxi/asm-replication)

---

### PRM Replication - Process Reward Models
**Why it matters for AGI:**
Outcome reward is not enough.
An agent that only learns from final results cannot improve
the quality of its reasoning process.
PRM rewards intermediate steps - it teaches the agent
to think well, not just to get lucky.
For the revenue agent: did the scoring decision at step 3
contribute to the meeting at step 47?
That attribution chain is what PRM formalizes.

→ [github.com/originaonxi/prm-replication](https://github.com/originaonxi/prm-replication)

---

### RewardFlow Replication - Multi-step reward propagation
**Why it matters for AGI:**
Single-step reward is local. RewardFlow propagates
reward signals across the full action chain -
crediting or penalizing decisions that caused
outcomes several steps later.
Revenue attribution IS RewardFlow in the wild.
Every email sent, every follow-up skipped, every
angle chosen - each one contributed to whether
the meeting happened. RewardFlow is how you learn
which contribution mattered most.

→ [github.com/originaonxi/rewardflow-replication](https://github.com/originaonxi/rewardflow-replication)

---

### TDAD Replication - Trajectory-Driven Agent Design
**Why it matters for AGI:**
Trajectory data is the ground truth of agent behavior.
Not what the agent said it would do - what it actually did,
step by step, under real conditions.
For the revenue agent: the full trajectory from
"Apollo returned this company" to "meeting booked"
is the dataset. TDAD is the framework for learning from it.

→ [github.com/originaonxi/tdad-replication](https://github.com/originaonxi/tdad-replication)

---

### Information Architecture Thesis - Long-horizon state management
**Why it matters for AGI:**
State is the unsolved problem of production agents.
What do you keep? What do you compress? What do you discard?
How do you structure it so retrieval is fast, relevant,
and causally grounded when the context window runs out?
This thesis formalizes those decisions for agents
operating over thousands of steps and months of campaigns.

→ [github.com/originaonxi/information-architecture-thesis](https://github.com/originaonxi/information-architecture-thesis)

---

### MoE Efficiency Study - Latest published paper
**Routing Strategy and Load Balancing in Small-Scale MoE Transformers**

Controlled comparison of top-k, expert choice, and noisy top-k routing.
Original expert specialization score metric.
Key finding: Top-2 routing + light auxiliary loss delivers
20% perplexity improvement and prevents collapse.
Directly applicable to multi-agent swarms where
routing decisions determine which persona model handles which prospect.

→ [github.com/originaonxi/moe-efficiency-study](https://github.com/originaonxi/moe-efficiency-study)

---

## The AGI thesis - what I actually believe

**The bottleneck is not intelligence. It is reliability.**

GPT-4 can reason. Claude can reason. Gemini can reason.
None of them can operate a live business autonomously
for 6 months without accumulating failures that compound.

The five components you need to build AGI that actually does something:

Memory that survives sessions (ASM)
Not context windows. Structured causal anchors.
What happened, what caused it, what it means for next time.
Reward that propagates through time (PRM + RewardFlow)
Not "did this email get a reply" but
"did this decision pattern produce meetings
across 6 months of campaigns."
Trajectories that stay coherent (TDAD)
An AGI that drifts after 100 steps is not AGI.
It is a very expensive random walk.
Human-in-the-loop as a learning signal (HAGI)
Not a safety patch. A continuous preference signal.
Every Y/N approval is a labeled training example.
That is RLHF running live in production, every day.
Production data as ground truth (Aonxi $650K ARR)
Benchmarks can be gamed.
Revenue cannot.
2,452 leads. 250 meetings. 42 sales. Real money.
That is the eval.


Put these five together and you get:
**An agent that improves itself continuously,
operates reliably over months,
attributes outcomes to decisions,
and gets better every single day
without human intervention.**

That is AGI for a bounded domain.
I chose revenue because the eval is unambiguous.
I am building it in production because that is the only
environment where the theory gets tested honestly.

I operate at the intersection where nobody else stands:
Visionary enough to see the destination.
Technical enough to build the path.
Obsessive enough to ship it daily.

The names people invoke when they talk about this level of ambition -
Elon, Demis, Sam, Andrej - they are all right about where this goes.
The difference is I can also write the code,
connect the agent to everything,
and put real money on the line to prove it works.

---

## What I do every day
Morning:    Read one new paper or arxiv preprint
            Run aonxi-outreach (20+ new emails sent)
            Note what the agent got wrong
Afternoon:  Review replies, close clients
            Run aonxi-sequence (follow-up sequences)
            Log outcomes as ASM anchors
Evening:    Build or improve one thing
            Push to GitHub
            Connect what I built to a paper I read
Weekly:     Write up what the data showed
            Update paper outline with new numbers
            Ask: what would falsify this hypothesis?
Always:     Every paper connects to a live experiment
            Every experiment produces real outcome data
            Every outcome improves the next decision

---

## Papers on my desk

| Paper | Why I am reading it |
|-------|---------------------|
| AndroTMem (2026) - arxiv:2603.18429 | Active replication → NeurIPS 2026 |
| Constitutional AI - Anthropic, 2022 | HAGI loop design, preference learning |
| LoRA - Microsoft, 2021 | Fine-tuning persona models on production data |
| ReAct - Google, 2022 | Reasoning + acting loops in live agent |
| Toolformer - Meta, 2023 | Tool use for 30+ source discovery waterfall |
| Sleeper Agents - Anthropic, 2024 | Alignment in long-running production agents |
| PRM - OpenAI | Process reward in multi-step scoring decisions |
| RewardFlow | Causal attribution across campaign trajectories |

---

## Production stack
Agent core:     Python · Anthropic API (Claude Haiku/Sonnet)
                Grok API · dual-LLM weighted scoring
Discovery:      Apollo · Exa · Hunter · 30+ source waterfall
Memory:         SQLite ASM anchor bank · structured causal retrieval
Delivery:       Gmail SMTP · SendGrid · IMAP reply detection
Orchestration:  Temporal.io · durable execution · kill switches
Infra:          Kubernetes · spot GPUs · Rust + Tokio core
Data:           Kafka/Redpanda · ClickHouse · 100M+ B2B records
Research:       PyTorch · vLLM · Qdrant · LoRA fine-tuning
Observability:  Custom revenue attribution dashboard · OpenTelemetry
HITL cockpit:   React · WebSockets · Y/N/feedback nodes

---

## Experience that proves I can ship this

**Aonxi - CTO** (Sep 2025 – Present · Santa Monica)
Built the autonomous revenue agent from scratch.
$650K ARR in 5 months. $0 raised. Zero paid acquisition.
120+ revenue-trained persona models as live autonomous workflows.
76 enterprise-grade real-time intent filters.
100M+ continuously enriched B2B records.
Native HITL nodes: veto, approve, override, feedback.
Every architecture decision tested on real production outcomes.

**Lotus Interworks - VP/Director Revenue Engineering** (2023–2025 · LA)
ARR: $25K → $4M in 9 months.
Close rate: 10% → 34%. Sales cycle: weeks → 5 days.
Pipeline throughput: 10x. Qualified pipeline exceeded $100M.
Built PilotOS (Results-as-a-Service) treating revenue
as a constrained learning control system.
Co-designed ECOSYSTEM framework with Dr. Gopinath (Stanford PhD)
and Ray Stata (Founder, Analog Devices).

**Meta - ML Engineer, Ads** (2017–2023 · 6 years · Menlo Park)
CTR/CVR prediction, ranking, and bidding at billions of daily inferences.
Data augmentation, synthetic data, knowledge distillation.
Early production PyTorch eager-mode adopter -
shipped one of the first ad-ranking models on dynamic graphs
when the industry was still on static TensorFlow.

**Apple - Research Scientist ML (Intern)** (2017 · Cupertino)
Reduced Face ID false positives by 15% on edge cases.
Built sim-to-real GAN refiner for synthetic training.
Published: machinelearning.apple.com/research/gan (arXiv 1612.07828).

**AutoScholar Pro - Founder** (Age 10–20 · India)
Self-taught on a second-hand PC. No internet.
QBASIC books from the library. 12-hour daily sprints.
Built an automated university and scholarship platform
serving 5,000 students, unlocking $2M+ in scholarships.
90% acceptance prediction accuracy. Exited for $100K.
First line of code written at age 10.
Have not stopped shipping since.

---

## Education

Northwestern University - Kellogg School of Management, MBA (Marketing)
Delhi University - B.Sc. Mathematics
Frontier AI Open School - Andrej Karpathy directed Deep Learning & LLM Systems

---

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
| aonxi-outreach-agent | Production autonomous revenue agent | Private |

---

## Numbers

| Metric | Number |
|--------|--------|
| ARR | $650,458 |
| Months to build it | 5 |
| Funding raised | $0 |
| Leads processed | 2,452 |
| Meetings booked | 250 |
| Sales closed | 42 |
| ASM beats raw scoring | 83% of prospects |
| Lines in production | 12M+ |
| Years shipping F500 | 10 |
| Age I wrote first line of code | 10 |
| Papers replicated | 5 + 1 original |
| NeurIPS 2026 submission | 1 in progress |

---

## If you are building at the frontier

I want to talk to people working on:
- Long-horizon agent reliability in production
- Memory architectures beyond context windows
- RLHF from live human-in-the-loop systems
- Production evals where real outcomes are the metric
- AGI that operates in bounded real-world domains
- Agents that are P&L accountable, not just task-complete

Frontier labs building AGI - I am your hire.
I can see where this goes and I can build the path to get there.
I have the production system, the research program,
the engineering depth, and the evidence.

origin@aonxi.com · aonxi.com
Santa Monica, CA · Shipping every day since age 10

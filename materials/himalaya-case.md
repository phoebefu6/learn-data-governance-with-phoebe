# Himalaya - the running case bible (data governance edition)

Every session governs the SAME company across all 8 sessions. Numbers below are canon - all
pages and presenter notes must stay consistent with this file. Update here first if anything
changes. (Company facts are shared with the strategic-thinking course; the data/privacy
situation below is specific to this course.)

## The company

**Himalaya** is a fictional B2B2C SaaS platform. Businesses subscribe to Himalaya; their end
consumers use it. Himalaya provides the digital layer (storefront, booking, engagement,
payments, analytics modules) that mid-size consumer businesses run their customer experience
on. "The platform behind the brands you buy from" - no single vertical.

- Founded 9 years ago, Series C, 300 employees
- **$40M ARR**, 1,200 business clients (the B), 8M end consumers (the C) monthly
- Headquartered in **Singapore**; clients and consumers across SG, EU, and SE Asia
- Runs on **AWS (Redshift warehouse)**; modules ship data to a shared analytics layer
- Pricing: platform subscription + per-transaction take rate

## The data situation (why the board just created a DPO role)

Himalaya has grown data-first and governance-last. The trigger events:

- A **near-miss breach**: a misconfigured analytics export exposed a table of end-consumer
  records to a client's staging bucket for 6 days before anyone noticed.
- Marketing blasts SMS + voice campaigns to the **8M consumer base** with no DNC register
  check and murky consent - a competitor was just fined for the same thing.
- **No data catalog**: nobody can answer "what personal data do we hold, where, and why."
  PII is scattered across 40+ Redshift schemas and 3 SaaS tools.
- Cross-border flows are undocumented: EU consumer data lands in a Singapore warehouse,
  copied to a US analytics vendor - no transfer safeguards on file.
- Retention is "keep everything." Ex-clients' consumer data still sits in the warehouse.
- The board appointed **You** as Himalaya's first **DPO** (Data Protection Officer). Mandate:
  protect the data subjects AND shield the company. PDPA-primary (Singapore home law),
  GDPR as the benchmark because of EU consumers.

## Cast (recurring voices in examples)

- **Mara** - CEO, appointed you, wants "compliant but don't slow us down"
- **Deven** - CPO, owns the product modules that collect the data
- **Ilsa** - CRO, owns the marketing campaigns (the DNC + consent risk)
- **Raj** - Head of Data/Platform, owns the Redshift warehouse and pipelines
- **Tom** - VP Customer Success, first to hear from angry consumers
- **You** - Himalaya's first DPO; each session hands you the pen

## Data landscape (canon - use consistently in diagrams and demos)

- **B-side data** (business clients): company contacts, billing, contract terms - mostly
  business, some personal (named contacts).
- **C-side data** (8M end consumers): name, email, phone, address, purchase history,
  in-app behavior, some **payment tokens** and, in the wellness-vertical clients, **health
  notes** (special/prescribed data).
- **Prescribed / sensitive** in play: NRIC-style national IDs (SG clients collect them),
  financial account info, health data, login credentials.
- Systems: Redshift warehouse (40+ schemas), the product modules, a CRM SaaS, a marketing
  automation SaaS (US-hosted), a support tool.

## Session-by-session state of play

| Session | Himalaya moment (what You, the DPO, do) |
|---|---|
| 1 | Day 1 as DPO. Map who does what with data, where you sit, and why PDPA makes your role mandatory. Draw the DAMA wheel over Himalaya. |
| 2 | Learn the two rulebooks you enforce: PDPA (home) + GDPR (EU consumers). Build the obligation-to-risk map for Himalaya. |
| 3 | You can't govern what you can't see. Build Himalaya's Record of Processing (RoPA) + classify its datasets (PII / sensitive / prescribed). |
| 4 | The marketing problem. Fix consent + purpose + the DNC register check before Ilsa's next 8M-consumer campaign. |
| 5 | The near-miss becomes real: a breach tabletop. Assess notifiability, draft the PDPC + individual notifications against the clock. |
| 6 | Clean up the lifecycle: retention schedule, disposal, cross-border transfer register (EU->SG->US), and how to answer access/correction requests. |
| 7 | Stand up the operating model: policies, decision rights, data owners/stewards/council, DPO office. Score Himalaya on a maturity model. |
| 8 | Capstone: assemble S1-7 into Himalaya's governance + privacy program. Run a DPIA on the AI copilot, write the DPO's first-90-days plan + board report. |

## Canon decisions (so later sessions don't contradict earlier ones)

- The wellness-vertical clients are the reason **health data (special/prescribed category)**
  is in scope - raises the stakes for consent, protection, and breach.
- The **marketing automation SaaS is US-hosted** - the concrete cross-border transfer case
  used in Sessions 4 and 6.
- Breach tabletop (Session 5) uses the near-miss export: **> 500 consumers affected + health
  notes involved** -> notifiable on BOTH the significant-scale and significant-harm limbs.
- Session 7 maturity score: Himalaya lands **low (early/"conceptual")** on most capabilities -
  the capstone plan in Session 8 is the roadmap to raise it.
- Session 8 board narrative: "Stop the bleeding (consent + DNC + breach playbook), see the
  data (catalog + RoPA), build the machine (operating model), then govern the AI bet (DPIA)."

## Honesty rails (must appear on the relevant pages)

- **PDPA Data Portability Obligation** is enacted (2020 amendment) but **not yet in force** -
  teach as "legislated, pending regulations," never as live.
- **DCAM** exact component names are member-gated (EDM Council). Teach the maturity/scoring
  *concept* honestly; do not invent the official 8 component names.
- Certification exams (IAPP CIPP/E, CIPM, CIPT; PDPC's own courses) stay official - this
  course teaches the body of knowledge, not the exam.

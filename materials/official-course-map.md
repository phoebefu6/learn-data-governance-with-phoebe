# Official course map - learn-data-governance-with-phoebe (Tech / DPO track)

How the 8 sessions cover the canon. ✓ = taught to working depth (the ~80% bar), ◐ = introduced
/ partial (deeper in the cited official source). Certification exams and member-gated content
stay official - this course teaches the **body of knowledge**, not the exam.

**Audience:** DA / DE / DS / AI practitioners on a data team, being equipped to run as a
**Data Protection Officer (DPO)** - protect data subjects and shield the company.
**Legal lens:** PDPA-primary (Singapore home law) with GDPR as the mirror/benchmark.
**Running case:** Himalaya (see `himalaya-case.md`).

Re-verify before delivery: PDPC and GDPR pages are stable, but check the PDPC site for any
change to the **Data Portability Obligation** commencement, and DCAM's current release, before
teaching live.

## Source universe

| Source | Role in course | Access reality |
|---|---|---|
| DAMA-DMBOK2 (2017) | Governance definition + the DAMA Wheel; spine for what "governance" spans | Book; wheel/areas public |
| Singapore PDPA + PDPC guidance | **Primary law**: 11 obligations, breach, DNC, DPO mandate | Public (pdpc.gov.sg) |
| Do Not Call (DNC) Registry | 3 registers, telemarketing checks | Public (pdpc.gov.sg) |
| GDPR (Arts. 5, 6, 12-22, 33, 37-39) | **Mirror**: principles, bases, rights, breach 72h, DPO role | Public (gdpr-info.eu) |
| IAPP CIPP/E, CIPM, CIPT | Maps the DPO body of knowledge; named, not reproduced | Certs official (iapp.org) |
| DCAM v3 (EDM Council) | Maturity-assessment model + scoring concept | Framework member-gated |
| Collibra / Alation (concepts) | Catalog, glossary, lineage, policy, stewardship, quality - tool-agnostic | Concepts public |

## Per-session coverage

### Session 1 - Foundations: data governance + the DPO  🟢
| Item | Cover | Note |
|---|---|---|
| DAMA Wheel - governance as the hub + the 10 spokes | ✓ | Named + diagrammed; each spoke deep in DMBOK2 |
| What data governance is (authority, decision rights, accountability) | ✓ | |
| DPO role - PDPA mandatory-for-all vs GDPR 3-case mandate | ✓ | PDPA Accountability Obligation; GDPR Art. 37(1) |
| DPO tasks + independent position | ✓ | GDPR Art. 38-39 as the task list |
| Personal data vs PII vs prescribed/sensitive | ✓ | |
| Full DMBOK2 knowledge areas in depth | ◐ | Introduced; book-level detail out of scope |

### Session 2 - The law you enforce  🟡
| Item | Cover | Note |
|---|---|---|
| PDPA 11 Data Protection Obligations | ✓ | Consent, Purpose, Notification, Access & Correction, Accuracy, Protection, Retention, Transfer, Breach, Accountability, Portability |
| PDPA consent model + deemed consent | ✓ | Deeper in S4 |
| DNC 3 registers | ◐ | Named here; worked in S4 |
| GDPR 7 principles (Art. 5) | ✓ | |
| GDPR 6 lawful bases (Art. 6) | ✓ | |
| GDPR 8 data subject rights | ✓ | Exercised in S6 |
| PDPA vs GDPR key differences | ✓ | Comparison table |
| Full statutory text / case law | ◐ | Pointers to PDPC + gdpr-info |

### Session 3 - Know your data: inventory, mapping, classification  🟡
| Item | Cover | Note |
|---|---|---|
| Record of Processing (RoPA) - build one | ✓ | Template provided |
| Data mapping / data flow | ✓ | |
| Data classification (PII / sensitive / prescribed) | ✓ | |
| Data catalog + business glossary (concept) | ✓ | Collibra/Alation, tool-agnostic |
| Data lineage (concept) | ✓ | Column/table-level impact analysis |
| Hands-on config of a specific catalog tool | ◐ | Vendor academies stay official |

### Session 4 - Consent, purpose & marketing (DNC)  🟠
| Item | Cover | Note |
|---|---|---|
| Consent Obligation + withdrawal | ✓ | |
| Purpose Limitation + Notification | ✓ | |
| Deemed consent (incl. by notification) | ✓ | |
| DNC - 3 registers + when to check | ✓ | Voice / Text / Fax registers |
| DNC exemptions (ongoing relationship, clear consent) | ✓ | |
| ePrivacy / EU marketing rules | ◐ | GDPR consent contrast only |

### Session 5 - Protection & breach response  🟠
| Item | Cover | Note |
|---|---|---|
| Protection Obligation - reasonable security arrangements | ✓ | |
| PDPA breach notification: 30-day assess / 3-day PDPC | ✓ | |
| Notifiable thresholds: significant harm OR >=500 individuals | ✓ | |
| GDPR breach: 72-hour authority notification | ✓ | Art. 33, as mirror |
| Breach tabletop / runbook | ✓ | On Himalaya near-miss |
| Deep security engineering (SOC, IR tooling) | ◐ | Governance angle only |

### Session 6 - Data lifecycle: accuracy, retention, transfer, rights  🟠
| Item | Cover | Note |
|---|---|---|
| Accuracy Obligation | ✓ | |
| Retention Limitation + disposal | ✓ | Retention schedule built |
| Transfer Limitation - comparable protection | ✓ | EU->SG->US case |
| GDPR transfer regime (adequacy / SCC / BCR) | ✓ | As mirror |
| Access & Correction Obligation | ✓ | DSAR handling |
| Data Portability | ◐ | **Enacted, not yet in force** - taught as pending |

### Session 7 - The operating model + maturity  🔴
| Item | Cover | Note |
|---|---|---|
| DAMA governance: policies, standards, decision rights | ✓ | |
| Roles: data owners, stewards, governance council, DPO office | ✓ | |
| Stewardship workflows | ✓ | |
| Data quality as a governed capability | ✓ | |
| DCAM maturity model + scoring concept | ✓ | Concept + scoring; exact v3 component names member-gated (◐) |
| Full DCAM assessment as an EDM member | ◐ | Requires member framework |

### Session 8 - Capstone: stand up the program  🔴
| Item | Cover | Note |
|---|---|---|
| DPIA (data protection impact assessment) | ✓ | On the AI copilot bet |
| Accountability - demonstrate compliance | ✓ | Policies/complaints/DPO contact |
| DPO first-90-days plan | ✓ | |
| Board-level reporting | ✓ | |
| Assemble S1-7 outputs into one program | ✓ | |

## Not covered by design (say so honestly on the pages)

- **Certification exam prep** - IAPP CIPP/E, CIPM, CIPT and PDPC's own courses are the official
  route; this course teaches the underlying body of knowledge, not exam questions.
- **Legal advice** - this is practitioner training, not a substitute for qualified counsel on
  specific matters.
- **Vendor tool configuration** - Collibra / Alation / Purview hands-on stays with their
  academies; we teach the tool-agnostic capabilities.
- **DCAM official component names + full assessment** - member-gated (EDM Council); we teach
  the maturity/scoring concept.
- **PDPA Data Portability Obligation** - legislated (2020) but not yet in force; taught as
  pending, not live.
- **Deep security engineering / incident-response tooling** - we cover the governance and
  notification duties, not the SOC build.

## Verified facts appendix (cite on pages)

- PDPA **11 obligations** (PDPC framing): Consent; Purpose Limitation; Notification; Access &
  Correction; Accuracy; Protection; Retention Limitation; Transfer Limitation; Data Breach
  Notification; Accountability (incl. **mandatory DPO** designation); Data Portability
  (enacted, pending). Source: pdpc.gov.sg.
- PDPA **breach notification**: assess within **30 days** of awareness; if notifiable, notify
  **PDPC within 3 calendar days**; notifiable if **significant harm likely OR >= 500
  individuals** affected. Source: pdpc.gov.sg/report-data-breach.
- PDPA **penalties**: up to **S$1M or 10% of annual SG turnover, whichever higher**.
- **DNC**: three registers - **No Voice Call, No Text Message, No Fax Message**; check the
  relevant register before sending marketing, unless clear consent / exemption applies.
- GDPR **7 principles** (Art. 5): lawfulness-fairness-transparency; purpose limitation; data
  minimisation; accuracy; storage limitation; integrity & confidentiality; accountability.
- GDPR **6 lawful bases** (Art. 6): consent; contract; legal obligation; vital interests;
  public task; legitimate interests.
- GDPR **8 rights**: informed; access; rectification; erasure; restriction; portability;
  object; automated-decision-making safeguards.
- GDPR **DPO mandatory** in 3 cases (Art. 37(1)): public authority; large-scale regular &
  systematic monitoring; large-scale special-category/criminal data. Tasks: Art. 39.
- GDPR **breach**: notify authority within **72 hours** (Art. 33).
- **IAPP**: CIPP/E (privacy law), CIPM (program management), CIPT (privacy by design);
  CIPP/E + CIPM is the recognised DPO training combination.
- **DAMA Wheel**: Data Governance at the hub; 10 spokes - Architecture; Modeling & Design;
  Storage & Operations; Security; Integration & Interoperability; Document & Content Mgmt;
  Reference & Master Data; Warehousing & BI; Metadata; Data Quality.
- **DCAM v3** (EDM Council): capability-assessment framework with a scoring model; exact
  component names are member-gated - teach the concept, not invented names.

## Sources

- PDPC PDPA obligations: https://www.pdpc.gov.sg/overview-of-pdpa/the-legislation/personal-data-protection-act/data-protection-obligations
- PDPC breach: https://www.pdpc.gov.sg/report-data-breach
- PDPC DNC: https://www.pdpc.gov.sg/overview-of-pdpa/do-not-call-registry/business-owner/do-not-call-registry-and-your-business
- GDPR Art. 5 / 6 / Ch.3 / 37 / 39: https://gdpr-info.eu/
- IAPP: https://iapp.org/certify/get-certified/
- DAMA-DMBOK: https://www.dama.org/cpages/body-of-knowledge
- DCAM: https://edmcouncil.org/frameworks/dcam/

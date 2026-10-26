# Project H — Pitch Pack

**Prepared:** 27 October 2026
**Stage:** pre-pilot. No product, no revenue, no clinical advisor, no company.
**Purpose:** four pitches, one evidence base, so no two conversations quote different numbers.

---

## README — which document goes to whom, and in what order

| # | Document | Reader | What they can say yes to | Send when |
|---|---|---|---|---|
| 00 | `00-EVIDENCE-BASE.md` | You (internal) | — | Never send. This is the source of truth |
| 01 | `01-CLINIC-LAB.md` | Lab owner, clinic manager, physio/rehab centre owner | A ₹15,000 paid pilot | **Week 1.** This is the only document that produces revenue |
| 02 | `02-GRANT.md` | SISFS/BIG panel, incubator | ₹20–50 lakh grant | Month 9–12, once a prototype or trial plan exists |
| 03 | `03-ADVISOR.md` | A doctor you want as clinical advisor | 2 hrs/month + 0.5% equity | Month 2–6, after one pilot or one strong conversation |
| 04 | `04-CUSTOMER-INVESTOR.md` | Lab-chain promoter, clinic owner, angel | ₹25 lakh for 10–12% | Month 12+, **only after** one paid pilot has renewed |

### The send order is not negotiable

```
01 (clinic) → produces revenue + evidence
     ↓
03 (advisor) → borrows credibility, unlocks more clinics
     ↓
02 (grant) → funds the product, not the sales
     ↓
04 (investor) → funds expansion, and only with traction
```

Sending 04 before 01 is the most common mistake a first-time founder makes. An investor who asks "who pays you today?" and hears "nobody yet" will not recover from that answer, no matter what slide 6 says.

### The one rule for all four documents

**No number appears in a pitch that is not either sourced or labelled as a target.** A lab owner who catches one inflated figure discards the whole document, and a grant panel checks every line of the budget. Every figure below carries a tag:

- **[F]** verified fact, source in `00-EVIDENCE-BASE.md`
- **[T]** target or planning assumption, not yet measured
- **[C]** the customer's own number, to be filled during the pilot

### What each document must never claim

| Claim | Status | Why |
|---|---|---|
| "60–70% of patients never come back" | **Not established** | Plausible, widely believed, unmeasured in Indian primary care. Use it as the pilot's hypothesis, not as a fact |
| "We improve blood pressure control" | **Not established** | Requires a controlled study. You are selling confirmation, not outcomes |
| "Clinically validated" | **Never, at this stage** | Nothing is validated. Say "protocol-based" |
| "AI-powered" | **Never, at this stage** | There is no model. Saying it invites technical diligence you will fail |
| "Backed by research" | **Careful** | You have a market analysis, which is real work, but it is not clinical evidence |

---

## 00 — EVIDENCE BASE (internal)

The twelve facts that carry the pitch, what each proves, and where it is used. Full citations resolve in §16.2 of `Project-H-Market-Intelligence-Report.md`.

### A. The clinical gap

| # | Fact | Source | What it proves | Used in |
|---|---|---|---|---|
| E1 | **1.4 billion** adults aged 30–79 have hypertension; **~600 million (44%) are unaware** | [F] MR S11 | The confirmation step addresses the largest undiagnosed population in chronic disease | 02, 04 |
| E2 | India: **210.2 million** adults with hypertension, **173.9 million uncontrolled** | [F] MR S12 | The problem is not marginal in the home market; it is the default condition of middle age | 02, 04 |
| E3 | Consumer hypertension notification has **41.2% sensitivity** in undiagnosed hypertensives (FDA-cleared, n=2,229) | [F] MR S13, S14 | A device "all clear" misses 6 in 10. The confirmatory step is not a nice-to-have; it is the only way the signal becomes usable | 01, 02, 04 |
| E4 | In **no country** does wearable data integration into clinical workflow exceed **6%** (2,222 physicians, 6 countries) | [F] MR S25 | The bottleneck is workflow, not sensor supply. Nobody owns the path from reading to decision | 01, 04 |
| E5 | Apple's hypertension feature was FDA-cleared in **September 2025** | [F] MR S13 | Detection is commoditising and will be free on every wrist within 3 years. Confirmation is not | 01, 02, 04 |

### B. The commercial gap

| # | Fact | Source | What it proves | Used in |
|---|---|---|---|---|
| E6 | India smartwatches: **28.9M units, −17.6%**, ASP **$26.5**; "advanced" segment **3.2%** | [F] MR S10 | Hardware is a low-margin, shrinking game here. Do not compete on the device | 04 |
| E7 | Oura: **89% gross margin on membership**, **85% 12-month retention**, 54.5% blended | [F] MR S7 | Recurring service economics beat device economics by a wide margin. A service business is the right shape | 04 |
| E8 | Garmin: **58.7% gross margin, 25.9% operating margin** at $7.25B revenue | [F] MR S6 | A focused, non-platform business can be highly profitable. You do not need to be Apple | 04 |
| E9 | US remote monitoring reimburses **~$102–160 per patient-month** (CPT 99453/99454/99457/99458) | [F] MR S26 | A funded pathway exists in a later market, which gives the business a second act without changing the product | 02, 04 |

### C. Why the timing works now

| # | Fact | Source | What it proves | Used in |
|---|---|---|---|---|
| E10 | Home BP devices are cheap and ubiquitous; WhatsApp is the default patient channel in India | [I] inference from E6 and Indian consumer behaviour | The delivery mechanism costs nothing. Five years ago this required an app and a smartphone cohort | 01, 04 |
| E11 | Diagnostic labs already run **home-collection networks** and already sell chronic-disease packages | [I] operational observation | The distribution and the commercial motive already exist. You are adding a step to a route that runs daily | 01 |
| E12 | Sleep-staging agreement with lab polysomnography is only **κ 0.41–0.53** | [F] MR S16 | Consumer data quality is genuinely contested. Quality scoring and provenance are a real product, not marketing | 02, 04 |

### D. What we do not know (state this before anyone asks)

| Gap | Status | How the pilot closes it |
|---|---|---|
| The actual follow-up rate after a high BP reading in an Indian clinic | **Unknown** | Measured in the first 6-week pilot, per site |
| Whether patients will complete a 7-day series | **Unknown** | Primary metric of the pilot |
| Whether doctors act on the summary | **Unknown** | Doctor-action rate, measured per cohort |
| What a clinic will pay | **Unmeasured** | The ₹15,000 pilot *is* the price test |
| Whether the model works outside one city | **Unknown** | Site 2 and 3, months 5–7 |
| Clinical outcomes | **Not addressed** | Requires a controlled study in year 2, with an advisor and ethics approval |

**This table is an asset.** Every credible operator you meet has the same gaps and hides them. Showing yours buys the right to be believed about everything else.

### E. The standard stage block (paste into any document)

```
STAGE: pre-pilot
Built:      market analysis (44 sources), legal scope, pilot design, pricing
Not built:  product, pilot, revenue, clinical advisory, company
Ask:        one paid pilot (₹15,000) — not investment
Timeline:   6 weeks from signature to first measured result
```

Never vary this. The moment one document says "early traction" and another says "pre-pilot," you are finished.

### F. The economics, consistently quoted

| Number | Value | Tag | Basis |
|---|---|---|---|
| Pilot price | ₹15,000 / 30 patients | [T] | Below approval threshold, above hobby pricing |
| Per-patient price at scale | ₹350–500 | [T] | Derived from pilot price at higher volume |
| Monthly retainer | ₹25,000–40,000 / 50–80 patients | [T] | Pilot price × 2, with a volume discount |
| Direct delivery cost | ₹80–120 / patient | [T] | Your time + comms, at a notional ₹300/hr |
| Gross margin at retainer | 70–80% | [T] | Assumes one part-time coordinator at 150 patients/month |
| Clinic's recovered revenue per completed patient | ₹500–2,500 / year | [T] | One follow-up consult plus one monitoring package; **must be validated per site** |

**The rule:** never quote a margin or a revenue figure you have not derived in front of the person asking. "It's about 75%" invites doubt; "₹400 a patient minus ₹95 of delivery cost" does not.

### G. The competitive frame, consistently quoted

| Who | What they do | Why they don't solve it |
|---|---|---|
| **The clinic's own staff** | Tell the patient to check at home | No owner, no list, no follow-up. This is the real competitor |
| **Consumer wearables** (Apple, Huawei, Samsung) | Detect and notify | 41.2% sensitivity; they hand the problem to the clinic, they don't solve it [E3] |
| **EMR / clinic software** | Records readings | Records; does not chase patients |
| **Remote monitoring platforms** | Device + dashboard, sold to hospitals | Built for US billing workflows; no India last-mile, no human follow-up |
| **Diagnostic labs** | Sell BP as part of a package | One-off measurement, no 7-day confirmation, no titration loop |
| **Us** | Own the 7 days between reading and decision | Only works if completion is measured and reported |

### H. Source register for this pack

All `[F]` items resolve to the companion report. Quick index:

| Tag | Fact | Report section |
|---|---|---|
| MR S11 | WHO hypertension prevalence | §16.2 A |
| MR S12 | WHO India country profile | §16.2 A |
| MR S13 | FDA K250507 clearance | §16.2 C |
| MR S14 | Apple hypertension validation | §16.2 C |
| MR S25 | AMA physician survey | §16.2 E |
| MR S26 | CMS RPM codes | §16.2 D |
| MR S10 | IDC India wearables 2025 | §16.2 A |
| MR S7 | Oura S-1 | §16.2 B |
| MR S6 | Garmin FY2025 | §16.2 B |
| MR S16 | Sleep-staging validation | §16.2 C |

---

*Audience documents: 01 clinic/lab · 02 grant · 03 advisor · 04 customer-investor.*

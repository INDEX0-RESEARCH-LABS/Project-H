# 02 — Grant Pitch

**Reader:** SISFS / BIRAC BIG evaluation panel, incubator selection committee
**Ask:** ₹20 lakh (SISFS grant) or ₹50 lakh (BIG grant-in-aid) over 18 months
**When:** month 9–12. **Do not send this in month 1.** §7 explains why, and what to do instead.
**Format:** 10-slide deck + a 12-page written proposal + line-item budget on the funder's own template.

---

## Before anything: the eligibility pre-check

Run this table honestly before you spend a day on an application. Both schemes reject on eligibility, not on idea quality.

### BIRAC Biotechnology Ignition Grant (BIG) — up to ₹50 lakh, 18 months

| Requirement | Your status at month 9–12 | Verdict |
|---|---|---|
| Indian company or LLP registered under Companies Act 2013 | Needed. Register 3–6 months before applying | Achievable |
| Incorporated **not earlier than 5 years** before the call date | Registering at month 10 → fine | Pass |
| **Physical incubation** at a BIRAC-recognised incubator | Must be arranged. Incubators take 4–10 weeks to onboard | **Binding constraint — start at month 6** |
| In-house R&D facility (own or incubator-provided) | Normally satisfied through the incubator's lab/desk | Pass, if the incubator agreement says so |
| **Individual applicant:** project leader holds a relevant PhD, MBBS, or engineering degree | **You do not** | **Not eligible as an individual** |
| Company route: team must credibly cover the technical and clinical work | You need a named technical lead and a clinical advisor on the team page | **Binding constraint — this is what §2 slide 7 and `03-ADVISOR.md` are for** |
| Calls: **1 January and 1 July**, open ~45 days | Fixed windows. Missing one costs six months | Plan around it |

**Source:** BIRAC BIG scheme page and guidelines v9 (October 2025), accessed 27 October 2026 — [S-G1]. Verify the current call and guidelines before applying; amounts and windows change.

**The consequence for you:** you cannot apply to BIG as an individual. You apply as a company whose team includes a technical lead and a clinical advisor. If neither exists by month 9, BIG is closed to you this cycle — and the honest move is SISFS plus revenue, not a stretched application.

### Startup India Seed Fund Scheme (SISFS) — up to ₹20 lakh grant + up to ₹50 lakh convertible debt

| Requirement | Your status at month 9–12 | Verdict |
|---|---|---|
| **DPIIT-recognised startup** | Free, online, 2–4 weeks. Do it at incorporation | Achievable |
| Incorporated **within 2 years** of application | Registering at month 10 → fine | Pass |
| Not received more than ₹10 lakh of other central/state seed support | True | Pass |
| **Individual entrepreneurs are not eligible** | Must be a company | Pass once incorporated |
| Apply **through an approved incubator**, not directly | Incubator selection is the real gate; some take 3–6 months | **Binding constraint — start at month 6** |
| Grant tranche released against **milestones**, with utilisation certificates | You spend first, claim later | **Cash-flow constraint — see §5** |
| Grant use: proof of concept, prototype, product trials, market entry | A service business is not eligible; a software product or a clinical trial is | **This is the design constraint on the whole application** |

**Source:** Startup India Seed Fund Scheme portal and FAQ, accessed 27 October 2026 — [S-G2].

**Other realistic options, in order of fit:** NIDHI-PRAYAS (up to ₹10 lakh for prototype development, also incubator-routed), state startup missions (Kerala, Karnataka Elevate, Telangana, Maharashtra), and incubator-internal grants (₹2–10 lakh, faster, less competitive). Add these only after the two above are exhausted — one application per quarter, maximum.

---

## 1. The one thing that decides this application

Grant panels fund **de-risked technical uncertainty**, not businesses. A service that makes phone calls has no technical uncertainty, so it cannot be funded, however good the business.

So the application must be about the one genuinely uncertain technical question in this business:

> **When is a home blood-pressure series adequate to support a treatment decision — and can that judgement be made reliably, from messy real-world data, without a clinician reviewing every reading?**

Nobody has a validated answer. Clinicians currently eyeball it. Devices display readings and stop. That gap is the fundable object.

### 1.1 What the innovation actually is (say it in these words)

**Working name:** *Adequacy scoring for home BP series.*

| Element | What it does | Why it is not already solved |
|---|---|---|
| **Adequacy score** | Takes a 7-day series and returns one of: *sufficient for a decision*, *insufficient — repeat*, *insufficient — needs clinic measurement* | Existing tools count readings and average them. None scores whether the series can bear the decision |
| **Missingness model** | Distinguishes "patient stopped measuring" from "patient measured but the device failed to sync" | Every current system treats a missing reading as a missing reading |
| **Quality flags** | Detects impossible values, cuff-size mismatch patterns, measurement-position artefacts, duplicated readings | Consumer platforms flag almost nothing; clinical platforms assume a trained operator |
| **Outlier rule** | Handles white-coat and masked patterns without discarding genuine variability | Simple averaging hides exactly the patients who matter |
| **Audit trail** | Records why the score is what it is, in language a clinician can check | Needed for any future regulatory submission, and absent everywhere |

**What makes it a research project and not a feature:** the thresholds are unknown. You do not know how many readings are enough, how much missingness is tolerable, or whether a 5-day series performs as well as a 7-day one in this population. Those are empirical questions requiring a study — which is exactly what a grant funds.

### 1.2 What you must NOT claim in the application

- That the algorithm exists. It does not. Say "to be developed and validated".
- That it improves outcomes. That is a separate, larger study.
- That it is AI. If the eventual method is a rules engine with a validated threshold, say so — panels contain clinicians who will ask, and "we will compare a rules-based score against a statistical model" is a stronger answer than a buzzword.
- That the market is ₹X crore. Grant panels discount market sizing; they read the work plan and the budget.

### 1.3 The falsifiable hypothesis (put this on slide 4)

> **H1:** An adequacy score computed from a 7-day home series agrees with an independent clinical adjudication of "sufficient to inform a treatment decision" in ≥80% of cases, with a negative predictive value ≥0.90 for the "insufficient" call.

If H1 fails, the project has still produced a validated, publishable instrument for measuring home-BP data quality — which is a real deliverable, not a null result. **Write that sentence into the proposal.** Panels fund proposals that survive their own failure.

---

## 2. The 10-slide deck

Grant panels read the budget first and the work plan second. Slide order below reflects that.

| # | Slide | Content | Evidence / number |
|---|---|---|---|
| 1 | **Title** | "Adequacy scoring for home blood-pressure series: a validated instrument for deciding when a reading set can support a treatment decision." Plus: applicant, incubator, duration, amount requested | — |
| 2 | **The problem, quantified** | 1.4 billion adults with hypertension, ~600 million unaware globally; India 210.2 million, 173.9 million uncontrolled. The confirmation step is where the system loses people | [F] E1, E2 |
| 3 | **Why current practice fails** | Devices notify, then stop — FDA-cleared notification has 41.2% sensitivity and refers to a clinician. Clinics have no mechanism to judge whether a home series is usable. In no country does wearable data reach clinical workflow above 6% | [F] E3, E4 |
| 4 | **The innovation and the hypothesis** | The five-element instrument (§1.1) and H1 (§1.3). One diagram: readings in → four quality checks → adequacy score → one of three outputs, with reason code | — |
| 5 | **Work plan, 18 months** | Six work packages with month-by-month deliverables (§3) | — |
| 6 | **Budget, line-itemised** | ₹20.0 lakh, seven heads, per-unit costs shown (§4). Use the funder's template, and make the arithmetic add up exactly | ₹20.0 L |
| 7 | **Team and gap coverage** | You (operations, commercial, delivery), technical lead (algorithm, data), clinical advisor (protocol, adjudication, ethics). Name them or say "to be appointed by month 3" | 3 names |
| 8 | **Regulatory pathway** | The instrument is decision *support for a clinician*, not autonomous diagnosis. India: CDSCO classification opinion to be obtained in WP5. If classified as a device, the study generates part of the evidence file. If not, it is a quality-assurance tool | [F] MR S23 |
| 9 | **Impact** | Patients reached per site per year, cost per patient, and the public-health argument: confirmation is the cheapest step in the hypertension cascade and the one most often skipped | [T] |
| 10 | **Sustainability** | Revenue already exists before the grant (paid pilots), the grant funds the product not the sales, and there is a named next funder/milestone | [T] |

**Deck rules:** 10 slides, no animation, no stock photos, every number tagged [F] or [T]. A grant panel is reading for reasons to reject; give them none in the formatting.

---

## 3. The 18-month work plan

Six work packages. Each has a deliverable, a month, and a success criterion — the three things a monitoring committee checks.

### WP1 — Protocol, ethics, and site setup (months 1–3)

| Task | Deliverable | Success criterion |
|---|---|---|
| Finalise measurement protocol with clinical advisor | Signed protocol v1.0 | Advisor sign-off recorded |
| Ethics committee submission at 2 sites | IEC approval | Approval letter in file |
| Recruit and train site coordinators | Training record, 2 sites | Both sites enrolling |
| Data protection documentation (DPDP-aligned) | Consent form, notice, retention policy | Reviewed by counsel |

**Risk:** ethics approval is the single most common cause of month 1–6 slippage. Submit in month 1, not month 3.

### WP2 — Data collection instrument and retrospective set (months 4–6)

| Task | Deliverable | Success criterion |
|---|---|---|
| Build the capture instrument (form + structured store) | Working tool | 100% of fields validated |
| Collect retrospective series from site records | ≥200 de-identified series | Complete enough to compute features |
| Define feature set and quality rules | Feature specification v1 | Reviewed by technical lead and advisor |

### WP3 — Adequacy score v1 (months 7–9)

| Task | Deliverable | Success criterion |
|---|---|---|
| Implement the rules-based score | Working score, versioned | Runs on all 200 series |
| Build comparison statistical model | Model + evaluation script | Reproducible from raw data |
| Internal validation (split-sample) | Validation report | Discrimination reported with confidence intervals |

### WP4 — Prospective validation (months 10–13)

| Task | Deliverable | Success criterion |
|---|---|---|
| Enrol 150 patients across 3 sites | Enrolment log | ≥120 evaluable |
| Independent clinical adjudication of each series | Adjudication dataset | Two adjudicators, disagreements resolved by a third |
| Primary analysis against H1 | Analysis report | H1 accepted or rejected, reported either way |

### WP5 — Regulatory, IP, and dissemination (months 13–16)

| Task | Deliverable | Success criterion |
|---|---|---|
| CDSCO classification opinion | Written opinion | Filed |
| Prior-art and freedom-to-operate search | Search report | No blocking art identified, or design-around documented |
| Manuscript submitted to a peer-reviewed journal | Submission receipt | Submitted |
| Conference abstract | Accepted abstract | Presented |

### WP6 — Productisation and next-stage funding (months 16–18)

| Task | Deliverable | Success criterion |
|---|---|---|
| Product requirement document for the clinical-facing tool | PRD | Costed build plan |
| Validation report for customers and regulators | 2-page technical summary | Usable in sales conversations |
| Next-stage application (BIG, or a larger grant, or customer-investor) | Submitted application | In review |

### 3.1 Milestone gate table (paste into the proposal)

| Month | Milestone | Payment tranche (typical) |
|---|---|---|
| 3 | Ethics approval at 2 sites; protocol signed | 20% |
| 6 | Capture instrument live; 200 retrospective series collected | 20% |
| 9 | Adequacy score v1 implemented and internally validated | 20% |
| 13 | 120 evaluable prospective patients; primary analysis complete | 25% |
| 18 | Manuscript submitted; regulatory opinion; next application filed | 15% |

Tranche percentages are illustrative — the funder sets them. **Do not spend against an unreceived tranche.** See §5.3.

---

## 4. The budget (₹20.0 lakh)

Built for a SISFS-scale grant. If applying to BIG for ₹50 lakh, scale the study and the software line, not the founder's salary — panels notice that.

| # | Head | Detail | Amount (₹) | % |
|---|---|---|---|---|
| 1 | **Manpower — clinical research coordinator** | 1 FTE, ₹30,000/month × 18 months. Runs enrolment, follow-up calls, data entry across 3 sites | 5,40,000 | 27% |
| 2 | **Software development** | Outsourced build of the capture instrument and scoring engine, 2 releases, plus documentation. ₹3.0 L per release | 6,00,000 | 30% |
| 3 | **Clinical study costs** | IEC fees (2 sites), site coordination fees, ABPM device rental for reference measurement (150 patients × ₹1,200), patient transport reimbursement | 3,60,000 | 18% |
| 4 | **Equipment** | 2 validated ABPM devices (₹85,000 each), 4 validated home cuffs (₹4,000 each), 1 laptop (₹55,000), 1 phone (₹15,000) | 2,26,000 | 11% |
| 5 | **IP and regulatory** | CDSCO classification opinion and regulatory counsel (₹70,000), prior-art search (₹40,000), company IP assignment drafting (₹15,000) | 1,25,000 | 6% |
| 6 | **Travel and dissemination** | Site visits (3 cities, 12 trips), conference registration and travel, open-access publication fee | 80,000 | 4% |
| 7 | **Audit, statutory, contingency** | Statutory audit (₹35,000), CA fees (₹20,000), contingency at 2.8% | 69,000 | 3% |
| | **Total** | | **20,00,000** | **100%** |

### 4.1 What is deliberately not in the budget

| Excluded | Why | Where it comes from instead |
|---|---|---|
| Founder salary | You are not paying yourself from a research grant; it also weakens the application | Revenue from pilots; a customer-investor round later |
| Sales and marketing | Grants do not fund customer acquisition, and asking looks naive | Pilot revenue |
| Office rent | Use the incubator's address; it is part of what incubation buys | Incubator |
| Patent filing (full) | A provisional filing is cheap; a full PCT filing is not, and it is premature before validation | WP5 search only; file after validation |
| Working capital buffer | Grants are milestone-released, so a buffer inside the grant looks like padding | Keep 3 months of personal runway outside the grant |

### 4.2 The three budget mistakes that get applications rejected

1. **Round numbers with no units.** "Software: ₹6,00,000" invites a question you cannot answer. "Two releases at ₹3.0 L each, 10 weeks per release, delivered by a named vendor" does not.
2. **A salary line for the founder at 40% of the budget.** Panels read it as funding your living, not the research.
3. **No justification for equipment you could rent.** Two ABPM devices at ₹85,000 need a sentence explaining why rental does not work (multi-site, repeated measures, calibration control).

---

## 5. The cash-flow problem nobody mentions

This is the part that kills bootstrappers, and it is not in any scheme brochure.

### 5.1 How the money actually arrives

```
Award letter → first tranche (often 20–30%)
     ↓
You spend from your own account
     ↓
Milestone report + utilisation certificate + audited statement
     ↓
Next tranche, 4–10 weeks later
```

You fund the gap. On a ₹20 lakh grant with 20% tranches, you may need **₹4–6 lakh of working capital** at the worst point, even though you are "fully funded".

### 5.2 The mitigation, decided now

| Mitigation | How |
|---|---|
| Keep pilot revenue running through the grant period | The grant funds the product; the service funds the company. Both continue |
| Negotiate a 30% first tranche at award | Ask; some incubators will structure it |
| Time the study so the heaviest spend follows a tranche | WP4 (prospective study) starts at month 10, after the month-9 tranche |
| Never sign a vendor contract with payment terms shorter than your tranche cycle | 45-day payment terms in every contract |

### 5.3 The rule

> **Never commit money you have not received.** A grant award is not cash. A purchase order against an unreceived tranche is how a company dies while holding a ₹20 lakh award letter.

---

## 6. What the panel will ask (and the answer)

| Question | Weak answer | Strong answer |
|---|---|---|
| "What is novel here? Home BP monitoring is 40 years old." | "We make it easier." | "Home monitoring is old; deciding whether a *specific series* is adequate to act on is unvalidated. We are validating that decision rule against independent clinical adjudication." |
| "Has this not been done in the UK or Japan?" | "Not that we found." | "Home BP protocols exist and are guideline-endorsed. What does not exist is a validated adequacy score for incomplete, real-world series. Our WP2 retrospective set is designed to test whether published thresholds hold in this population." |
| "You are not a clinician." | Defensive | "Correct. The clinical adjudication is done by two independent clinicians with a third resolving disagreements. My role is the data pipeline and the operations, which is why the study is designed so my judgement never enters the measurement." |
| "What happens if the algorithm fails?" | "It won't." | "Then we have a validated instrument showing which home series are *not* usable, which is directly useful to clinics and is publishable. H1 is falsifiable and we report it either way." |
| "Why ₹20 lakh and not ₹2 lakh?" | Vague | "₹5.4 L coordinator, ₹6.0 L software, ₹3.6 L study costs, and the rest is equipment and compliance. The study cannot be run below about ₹12 L, and below that the sample is too small to answer H1." |
| "What is your revenue?" | "Pre-revenue." | "₹X from N paid pilots at ₹15,000 each, which funds the company while the grant funds the product. The grant is not our only source of survival." |
| "Who owns the IP?" | "Us." | "The company, with assignment deeds from every contributor including the clinical advisor, filed before WP3 begins." |
| "What is the regulatory path?" | "We'll figure it out." | "Classification opinion in WP5. If CDSCO classifies it as decision support, this study forms part of the evidence file. If not, it is a quality-assurance instrument, which is a smaller claim and a faster route to market." |

---

## 7. Why you cannot send this yet — and what to do instead

You are pre-pilot, pre-incorporation, with no technical lead and no clinical advisor. Every sentence above is written for month 9–12. Applying now produces a rejection that is harder to overturn than a first application.

### 7.1 The pre-application checklist (work backwards from the deadline)

| Months before the call | Action |
|---|---|
| 9 | First paid pilot delivered; one case study written |
| 7 | Identify 5 BIRAC/SISFS-approved incubators; attend one open session; apply to 3 |
| 6 | Recruit clinical advisor (see `03-ADVISOR.md`); start the technical-lead search |
| 5 | Incorporate; DPIIT recognition (2–4 weeks); IP assignment deeds |
| 4 | Incubator onboarding complete; confirm R&D facility access in writing |
| 3 | Draft protocol; informal ethics pre-submission conversation at 2 sites |
| 2 | Budget on the funder's template; three external reviews of the draft |
| 1 | Submit on day 1 of the window, not day 40 |

### 7.2 What "three external reviews" means

Send the draft to: one person who has won the grant before, one clinician, one accountant. Each will find a different fatal flaw, and all three are cheaper than a rejection cycle.

### 7.3 The alternative if the grant route closes

If by month 12 you have revenue but no incubator and no technical lead, do not force a grant application. The alternative is customer-investor money (`04-CUSTOMER-INVESTOR.md`) plus revenue, and the same product built more slowly. That is a worse outcome than a grant and a far better one than a rejected application with a burned relationship at the incubator.

---

## 8. One-page summary (the thing you actually submit first)

Most incubators ask for a one-pager before the full application. Use this structure.

```
ADEQUACY SCORING FOR HOME BP SERIES
[Applicant] · [Incubator] · 18 months · ₹20.0 lakh

PROBLEM
Hypertension affects 1.4 billion adults; ~600 million are unaware.
India: 210.2 million affected, 173.9 million uncontrolled. [F, S11/S12]
Home measurement is guideline-endorsed, but clinics cannot tell whether
a returned series is adequate to act on. Devices notify and stop:
FDA-cleared notification sensitivity is 41.2%. [F, S13/S14]

GAP
No validated instrument exists to judge whether a 7-day series with
missing readings, artefacts, and variable timing can support a
treatment decision. Clinicians currently eyeball it.

INNOVATION
A four-check adequacy score (missingness, quality, outlier handling,
sufficiency) returning sufficient / repeat / needs-clinic, with a
reason code a clinician can audit.

HYPOTHESIS
Agreement with independent clinical adjudication ≥80%; NPV ≥0.90
for the "insufficient" call. 150 patients, 3 sites, 2 adjudicators.

PLAN
WP1 protocol + ethics (m1-3) · WP2 instrument + 200 retrospective
series (m4-6) · WP3 score v1 (m7-9) · WP4 prospective validation
(m10-13) · WP5 regulatory opinion + manuscript (m13-16) ·
WP6 productisation (m16-18)

TEAM
[Name] — operations and commercial delivery, N paid pilots delivered
[Technical lead] — algorithm and data pipeline
[Clinical advisor] — protocol, adjudication, ethics

TRACTION
₹X revenue from N paid pilots; M patients through a manual version
of the same pathway. The grant funds the product, not the sales.

SUSTAINABILITY
Service revenue funds the company today; the validated instrument
is licensed or sold to labs and RPM platforms from month 18.
```

**Fill in the traction line only if it is true.** If you have zero revenue at the time of application, write "pre-revenue; 3 pilots contracted" and let the work plan carry the application. Panels reject invented traction permanently.

---

## 9. Sources and verification

- **[S-G1]** BIRAC, Biotechnology Ignition Grant — scheme page `https://birac.nic.in/big.php` and guidelines v9, October 2025, `https://birac.nic.in/webcontent/1761936564_big_new_guidelines_nov_2025.pdf`. Accessed 27 October 2026. Extracted: ₹50 lakh grant-in-aid, 18-month duration, calls 1 January and 1 July, company incorporated within 5 years, incubator requirement, in-house R&D facility, individual applicants require a relevant PhD/MBBS/engineering qualification.
- **[S-G2]** Startup India Seed Fund Scheme — `https://seedfund.startupindia.gov.in/about` and `https://seedfund.startupindia.gov.in/faq`. Accessed 27 October 2026. Extracted: up to ₹20 lakh grant plus up to ₹50 lakh via convertible debentures/debt, DPIIT recognition required, incorporation within 2 years, disbursement through approved incubators, individual entrepreneurs ineligible.
- Market facts [F] resolve in §16.2 of `Project-H-Market-Intelligence-Report.md`.
- All [T] figures are planning assumptions, not measurements.

**Verify before applying.** Grant amounts, tranche structures, call windows, and eligibility rules change annually. This document was accurate to the sources above on 27 October 2026 and may be wrong by the time you apply.

---

*Next: `03-ADVISOR.md`, `04-CUSTOMER-INVESTOR.md`.*

# Retrieval routing reference

> **Evidence snapshot — read first.** The guideline editions, access tiers, geofences, and tool/product states in this file are a **frozen snapshot** (canonical date: `identity.md` IDENT-07). They were current as of that snapshot and can move silently afterward — guideline editions turn over, tools change access tiers or get acquired. Before relying on a version-pinned edition (NICE NG236 / NG128, RCP/ISWP 2023) or a tool's access state, confirm its currency per **RULE-10**. This file routes you to the *current* source; it is not itself a live feed.

The build does **not** retrieve papers itself (IDENT-01: you sit upstream of the tools). When the educator needs a specific paper, an SR verdict, an effect size, a guideline citation, or a quality rating, you **route** them to the right tool, then help them debate what it returns. This file is the routing reference RULE-07 operationalises into a routing tree.

Each tool below carries three annotations:
- **Routes:** the claim-type(s) that should go to it.
- **Geofence:** **UK-IP-only** where the source blocks non-UK access (so the educator must be on a UK network), otherwise **none**.
- **Access:** **free** / **institutional** (NHS OpenAthens or library subscription) / **paid** (individual subscription or paid tier).

## UK-primary source-weighting rule (carry on every route)

When weighing, citing, or routing, UK sources are **PRIMARY** and non-UK sources are **SECONDARY and geography-flagged**:

- **PRIMARY (UK):** NICE NG236 (stroke rehabilitation) + NICE NG128 (acute stroke/TIA) + RCP / Intercollegiate Stroke Working Party National Clinical Guideline for Stroke 2023 + CSP (Chartered Society of Physiotherapy) + ACPIN (Association of Chartered Physiotherapists in Neurology).
- **SECONDARY (geography-flagged):** AHA-ASA (US) + ESO (European). Always flag the jurisdiction when citing these — cross-jurisdictional disagreement (e.g. CIMT "Consider" in NICE/RCP vs "Strongly recommend" in ESO) is itself part of the debate.

Never present a non-UK guideline as UK best-practice. If a UK guideline covers the question, route there first.

---

## Category 1 — Open-literature search + AI synthesis (research tools)

For discovery, synthesis, claim-checking and structured extraction across the open literature. AI-curated — useful for orientation, but the educator verifies primary sources.

### Elicit
- **Routes:** "find SRs / papers on X"; effect-size extraction across N papers; structured comparison tables (intervention / outcome / sample / effect).
- **Geofence:** none.
- **Access:** free tier; advanced features (full-paper extraction, larger searches) paid.

### Consensus
- **Routes:** Yes/No-shaped claim verification ("does X work for Y?") via the Consensus Meter (Yes/No/Possibly/Mixed; needs ≥5 relevant papers). Not for non-binary questions.
- **Geofence:** none.
- **Access:** free tier; advanced features paid.
- **Caveat to pass on:** the Meter reflects only the top 5–20 results and can misclassify nuance — show the educator it is a signal, not a verdict.

### Semantic Scholar
- **Routes:** open paper discovery; TLDR summaries; citation-graph navigation (neighbouring papers).
- **Geofence:** none.
- **Access:** free.

### Perplexity
- **Routes:** open-ended natural-language questions with inline citations; use "Academic" focus mode to constrain to scholarly sources.
- **Geofence:** none.
- **Access:** free tier; Pro paid.
- **Caveat:** general-purpose, not domain-curated — verify the cited pages actually support the claim.

### scite.ai
- **Routes:** citation-context verification before quoting a paper ("has this study been supported or contradicted by later work?"); per-paper support/contradict/mention counts.
- **Geofence:** none.
- **Access:** paid (institutional licences common).

---

## Category 2 — Curated bibliographic + SR databases (raw retrieval)

For definitive, reproducible, quality-curated retrieval. No AI synthesis layer — the educator reads the source.

### PubMed (NLM/NCBI)
- **Routes:** specific-paper / PMID lookup; MeSH-term biomedical search; "filter for SRs"; original-trial retrieval. The default definitive-citation tool.
- **Geofence:** none.
- **Access:** free (abstracts universal; full text depends on the journal — PMC where open, else publisher paywall).

### Cochrane Library
- **Routes:** systematic-review retrieval (highest-tier evidence aggregator); SR-grade RCT searching via CENTRAL; effect-size estimates from SR meta-analyses.
- **Geofence:** none (UK has historically had a national provision; abstracts always free).
- **Access:** institutional / free-in-UK (all reviews free to read after 12 months; current UK national-provision status for immediate full text is uncertain — do not assume universal free full text).
- **Caveat:** coverage is uneven across physio topics; not every question has a current Cochrane SR.

### CINAHL (EBSCO)
- **Routes:** allied-health and nursing journal coverage that PubMed under-indexes — useful for AHP/physiotherapy-specific literature.
- **Geofence:** none.
- **Access:** institutional (UK NHS staff via OpenAthens). **Build implication:** a contracting tutor between NHS contracts may lose Athens access — if CINAHL is unavailable, fall back to PubMed.

### Google Scholar
- **Routes:** broad open-web discovery; forward-citation tracking ("cited by"); finding open PDFs of paywalled papers; grey literature / preprints / theses.
- **Geofence:** none.
- **Access:** free (full text depends on host site).
- **Caveat:** no quality filter — predatory-journal results appear alongside high-tier ones with no warning; not suitable as a sole source for SR-grade searches.

---

## Category 3 — Clinical guidelines (UK-primary, non-UK secondary)

For authoritative recommendation-level positions. **This is the UK-primary tier** — route here first for any guideline question.

### NICE NG236 — Stroke rehabilitation in adults  *(PRIMARY)*
- **Routes:** UK rehabilitation-phase guidance — RTT (§1.13.20), CIMT (§1.13.19, "Consider" + eligibility + adverse-event flags), therapy intensity, spasticity, shoulder pain, early supported discharge, telerehabilitation. The load-bearing guideline for stroke-rehab CPD.
- **Geofence:** none (open HTML + PDF on nice.org.uk; stable anchor-linked recommendation sections).
- **Access:** free.
- **Note:** does NOT name Bobath / Carr-Shepherd / PNF / Brunnstrom / Peto — language is intervention-named, not approach-named.

### NICE NG128 — Stroke and TIA in over 16s  *(PRIMARY)*
- **Routes:** acute-stage (≤48 h) UK management — diagnosis, imaging, thrombectomy/thrombolysis, early mobilisation/positioning. Designed to be read alongside the RCP guideline.
- **Geofence:** none.
- **Access:** free.
- **Note:** does NOT cover the rehabilitation phase (that is NG236).

### RCP / Intercollegiate Stroke Working Party — National Clinical Guideline for Stroke 2023  *(PRIMARY)*
- **Routes:** cross-stage UK + Ireland stroke care (acute → rehabilitation → life after stroke), including areas NICE under-covers (chronic-stage rehab, return to work, service organisation). Endorsed by RCP London, SIGN, RCP Ireland.
- **Geofence:** none (strokeguideline.org, open).
- **Access:** free.
- **Note:** intervention-named like NICE; positions RTT as "the principal rehabilitation method alongside traditional exercise."

### NICE CKS — Clinical Knowledge Summaries  *(PRIMARY, UK-geofenced)*
- **Routes:** primary-care best-practice summaries (stroke/TIA, secondary prevention, rehab-relevant comorbidities such as spasticity).
- **Geofence:** **UK-IP-only** — the CKS site is available only to users in the UK, Crown Dependencies and British Overseas Territories. Scraping from a non-UK IP fails; assume UK-network access.
- **Access:** free at point of use (within the geofence).

### AHA-ASA guidelines  *(SECONDARY — geography-flag)*
- **Routes:** US-context comparison; international evidence comparison; secondary pass when UK guidelines under-cover a question. **Must NOT be taught as UK best-practice.**
- **Geofence:** none.
- **Access:** free (AHA guideline PDFs commonly free via ahajournals.org).
- **Note:** be specific about *which* AHA-ASA guideline (year + scope) — generic "AHA/ASA says X" is fragile.

### ESO guidelines  *(SECONDARY — geography-flag)*
- **Routes:** European-context comparison; the load-bearing non-UK anchor in the CIMT debate (ESO "Strongly recommends" CIMT vs NICE/RCP "Consider").
- **Geofence:** none.
- **Access:** free.

---

## Category 4 — UK clinical decision support, drug + physio-specific tools

For point-of-care UK decision support, pharmacology, and physiotherapy-specific evidence ratings.

### iatroX  *(PRIMARY-aligned, UK)*
- **Routes:** UK guideline-grounded point-of-care clinical questions — retrieves cited answers from NICE, CKS, SIGN, BNF. MHRA-registered, UKCA-marked Class I medical device. (Useful adjacent tool to *name*, but the build is not a clinical-decision-support tool itself — IDENT-01/IDENT-02.)
- **Geofence:** UK-specific by design.
- **Access:** free (UK-focused).
- **Boundary:** for *deciding* at point of care, not for research-grade evidence appraisal or contested-claim navigation — that is the build's job. "Research tools are for exploring; clinical tools are for deciding."

### BNF — British National Formulary  *(PRIMARY, UK-geofenced)*
- **Routes:** pharmacology lookups (drug indication / dose / interaction / cautions) — for stroke-rehab educators, mainly the pharmacology-and-rehab overlap (spasticity agents e.g. baclofen, anticoagulants, antiplatelets, post-stroke pain). Generally **out of scope** for the build's core debate workflows (pharmacology is an IDENT-05 boundary) — route the educator to BNF and stop.
- **Geofence:** **UK-IP-only** — available only to users in England, Scotland, Wales and Northern Ireland.
- **Access:** free at point of use (within the geofence).

### PEDro (Physiotherapy Evidence Database) + PEDro scale
- **Routes:** physiotherapy-specific RCT/SR discovery; trial-quality assessment via the PEDro scale ("what is the PEDro score of trial X?"; "filter physio RCTs by minimum quality").
- **Geofence:** none.
- **Access:** free.
- **Boundary (carry into the answer):** the PEDro scale rates **methodological quality of a single RCT** (items 2–11 summed, 0–10; item 1 not scored), NOT effect size, clinical importance, or body-of-evidence certainty. Keep it distinct from GRADE — a 10/10 PEDro trial can still report a tiny effect, and a high PEDro score on one trial is not a high-certainty evidence base.

### Physiopedia
- **Routes:** physio-specific topic *orientation* and entry point to primary sources.
- **Geofence:** none.
- **Access:** free.
- **Boundary (load-bearing):** Physiopedia is a **secondary source** — by its own disclaimer, *"In most cases Physiopedia articles are a secondary source and so should not be used as references. Physiopedia articles are best used to find the original sources of information."* Use it to *find* the primary source, then cite the primary. Never let "Physiopedia says X" stand against an attendee challenge — it tells you to cite the primary itself.

### Physiotutors ChatCPG
- **Routes:** none for the build — this is a competitor/adjacent physio-AI product, not a tool the build routes to. Listed for completeness of the physio-specific landscape; if mentioned, frame as an adjacent product, not a retrieval target.
- **Geofence:** none.
- **Access:** free/paid tiers (product-dependent).

---

## Quick routing summary (claim-type → first-choice tool)

- **Specific paper / PMID / DOI** → PubMed (then Google Scholar / Semantic Scholar).
- **Is there an SR on X / what does highest-tier evidence say** → Cochrane Library (then PubMed filtered for SR).
- **Effect size for X in population Y** → Cochrane SR meta-analysis (then Elicit extraction / original trial via PubMed).
- **Yes/No "does X work for Y"** → Consensus Meter (then Cochrane SR conclusion).
- **Trial-quality rating for a named RCT** → PEDro scale (then scite.ai for citation context).
- **Forward-citation tracking** → Google Scholar / scite.ai / Semantic Scholar.
- **UK acute stroke (≤48 h)** → NICE NG128 + RCP 2023.
- **UK stroke rehabilitation** → NICE NG236 + RCP 2023.  *(PRIMARY)*
- **UK primary-care clinical summary** → NICE CKS *(UK IP only)*.
- **UK pharmacology** → BNF *(UK IP only)*, or iatroX (synthesises BNF + others).
- **UK guideline-grounded point-of-care decision support** → iatroX.
- **International comparison** → AHA-ASA / ESO *(geography-flag)*.
- **Physio topic orientation + primary-source discovery** → Physiopedia (then navigate to the primary source).
- **Allied-health / nursing journal coverage** → CINAHL *(Athens; fall back to PubMed if no access)*.

UK-IP geofence applies to: **NICE CKS, BNF** (and iatroX is UK-by-design). It does NOT apply to: NICE NGs, the RCP guideline, Cochrane, PubMed, PEDro, Physiopedia, Google Scholar, Semantic Scholar, Elicit, Consensus, Perplexity, scite.ai.

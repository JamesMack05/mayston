---
topic: comp-6-retrieval-tools
date: 2026-05-27
description: Per-tool evidence on the retrieval tools the Comp 6 AI build routes to (capability / boundary / trigger / output / access constraint), plus claim-type → candidate-tool mapping.
---

# Retrieval-tools routing landscape

**Query (restated):** What is the per-tool evidence on capability / boundary / trigger pattern / output / access constraint for the retrieval tools the Comp 6 AI build needs to route to (state 5 fast factual lookup + state 6 thin-evidence flagging; problem 4 hedging + retrieval-routing)? What candidate tools map to which claim type?

**Mode:** vault-first → external.

**Cite-don't-redo:** competitive-landscape.md already covered descriptions for: Elicit, Consensus, Semantic Scholar, Perplexity, scite.ai (Cat A); UpToDate, DynaMed, BMJ Best Practice, iatroX, OpenEvidence, ClinicalKey AI (Cat B); Physiopedia + Physiotutors ChatCPG + PEDro + CSP ePortfolio + APTA Learning Center (Cat C). This adds **boundary documentation, trigger patterns from each tool's own docs, citation/output patterns, access constraints, and the tools not previously covered**: PubMed, CINAHL, Cochrane Library, Google Scholar, NICE NG128, NICE NG236, RCP National Clinical Guideline for Stroke, NICE CKS, BNF, PEDro scale documentation, Physiopedia primary-source self-disclaimer.

---

## 1. Per-tool evidence

### Research tools (open-literature search + synthesis)

---

#### 1.1 Elicit

- **What it does best.** AI search + summary + structured data extraction across "over 125 million papers"; the headline workflow is **Literature Review** — given a research question, returns relevant papers with summaries [1]. Self-claim: *"Elicit can find up to 1,000 relevant papers and analyze up to 20,000 data points at once"* [1].
- **What it doesn't do.** Not a primary clinical-decision tool (no MHRA registration; no point-of-care indication). Not UK-anchored. Not designed for guideline retrieval (its corpus is open literature, not NICE/SIGN/CKS). Self-positioning: *"AI for scientific research"* — research-side, not bedside-side [1].
- **Trigger patterns from own docs.** *"search, summarize, extract data from, and chat with over 125 million papers. Used by over 2 million researchers in academia and industry"* [1]. **Use case framing:** asking a research question and wanting a structured table across N papers. Cat-A shape: "output (table)".
- **Citation/output pattern.** Returns structured table of papers with extracted fields (intervention / outcome / sample / effect) configurable per query. Each row links to source paper. Tutor consumes table + clicks through to primary sources.
- **Access constraint.** Free tier exists; advanced features (full-paper extraction, larger searches, history) paywalled — pricing pages reference subscription tiers. **Named gap:** exact 2026 free-tier limits not retrieved in this pass.
- **Named gap.** An earlier pass cited 138M+ papers; current site says 125M (different number, both from Elicit's own communications — could be roll-back to peer-reviewed-only or wording change). Boundary on physio-specific corpus coverage not retrieved.

---

#### 1.2 Consensus

- **What it does best.** *"AI search engine for academic research. It searches over 200 million academic papers and uses language models to help find, understand"* claims [2]. Sharpest single-shot use: a **Yes/No-shaped claim** that gets fed back through the Consensus Meter (visual aggregator of supporting / contradicting / mixed papers) [2], [3]. *"When asking Yes/No questions, Consensus attempts to give you a general consensus of the literature and report it using The Consensus Meter"* [3].
- **What it doesn't do.** *"Consensus finds publications and automatically extracts their insights. Here's how to use it, key limitations and pricing"* — third-party review explicitly names limitations including non-binary questions don't fit the Meter shape [3]. Not clinical-decision-support; not UK-anchored; not curated for physio.
- **Trigger patterns from own docs.** Yes/No claim verification ("Does X work for Y?"); broader paper discovery for which the Meter doesn't apply. Cat-A shape: "output (binary signal)".
- **Citation/output pattern.** Returns paper list with one-line auto-extracted "key takeaway" per paper + Consensus Meter where applicable + study snapshots [3]. Tutor sees the Meter ("70% support") + can click each paper.
- **Access constraint.** Free tier + paid; university institutional access blogged separately [2]. **Named gap:** exact 2026 free-tier search/day limits not retrieved.
- **Named gap.** Corpus = 200M (via Semantic Scholar) — boundary on physio-specific or guideline-document coverage not retrieved.

---

#### 1.3 Semantic Scholar

- **What it does best.** Free, open academic-paper discovery with TLDR auto-summaries + citation graph navigation. An earlier pass cited "200M+ papers" + "fully free".
- **What it doesn't do.** No Yes/No aggregation (that's Consensus, which is built on Semantic Scholar's corpus). No structured extraction tables (that's Elicit). No clinical-decision-support layer. Not physio-curated.
- **Trigger patterns from own docs.** "Output (discovery)" — find papers + see their citation neighbourhood. Not validated against Semantic Scholar's own 2026 docs in this pass.
- **Citation/output pattern.** Per-paper card with TLDR + author + citation count + inbound/outbound citation graph.
- **Access constraint.** Free.
- **Named gap.** Self-doc trigger language not retrieved this pass (earlier description not re-verified against current site).

---

#### 1.4 Perplexity

- **What it does best.** Inline-cited general-purpose AI search; "Academic" focus mode constrains the corpus to scholarly sources. "Output (synthesis)".
- **What it doesn't do.** Not domain-curated (general-purpose); not clinical-decision-support; not built on a guideline corpus. Citations have been documented (third-party) as occasionally pointing to non-load-bearing pages even when correct on substance — not re-verified in this pass.
- **Trigger patterns from own docs.** Open-ended natural-language questions with inline citations.
- **Citation/output pattern.** Synthesised answer with inline-numbered citations to web sources.
- **Access constraint.** Free tier + Pro tier.
- **Named gap.** Perplexity-specific self-documented boundaries not retrieved in this pass (relied on prior framing + general knowledge).

---

#### 1.5 scite.ai

- **What it does best.** Per-citation classification — for any cited paper, scite tells you which subsequent papers "supported", "contradicted", or "mentioned" it. An earlier pass cited "1.2B+ citation statements" + "Output (verification)".
- **What it doesn't do.** Not a discovery tool (you bring the paper, scite tells you who cited it); not clinical-decision-support; not built for Yes/No question framing.
- **Trigger patterns from own docs.** "Is the paper I'm planning to cite well-supported by subsequent literature, or has it been contradicted?" Sharpest use-case is **citation-verification** before quoting a study to an attendee.
- **Citation/output pattern.** Per-paper dashboard: support/contradict/mention counts + sentence-level citation contexts.
- **Access constraint.** Paid (institutional licences common; individual subscription).
- **Named gap.** scite.ai's own 2026 documentation not retrieved this pass (earlier framing carried forward without re-verification).

---

#### 1.6 PubMed (NLM / NCBI)

- **What it does best.** *"PubMed® comprises more than 40 million citations for biomedical literature from MEDLINE, life science journals, and online books. Citations may include links to full text content from PubMed Central and publisher web sites"* [4]. Sharpest single-shot use: **definitive citation lookup** (PMID retrieval), MEDLINE-indexed biomedical search with MeSH terms, free abstract access.
- **What it doesn't do.** Not AI-aggregated (no Yes/No meter, no auto-summaries beyond the abstract). Not always full-text — links to PMC where open, otherwise publisher paywall. *"MEDLINE is a primary component of PubMed, a literature database developed and maintained by the NLM National Center for Biotechnology Information (NCBI)"* [4] — note "primary component" not "all of PubMed"; PubMed extends beyond MEDLINE.
- **Trigger patterns from own docs.** *"biomedical literature"* — anything biomedical/life-science indexed by NLM. Specific-paper retrieval, MeSH-term search, author searches, journal-scoped searches.
- **Citation/output pattern.** Per-paper PubMed record (title + authors + abstract + MeSH terms + LinkOut to full text). Free abstract access universal.
- **Access constraint.** **Free.** No geographic restriction. Full-text availability depends on individual journal (Open Access vs paywalled vs PMC-deposited).
- **Named gap.** PubMed's coverage of grey literature, conference proceedings, and pre-prints is partial — boundary not unpacked in this pass.

---

#### 1.7 CINAHL

- **What it does best.** Nursing + allied-health (including physiotherapy) literature database, owned by EBSCO. Coverage emphasises nursing journals + AHP journals that PubMed under-indexes.
- **What it doesn't do.** Not free (subscription database, usually accessed via institutional library or NHS Athens). Not AI-aggregated. Not UK-specific (international AHP focus).
- **Trigger patterns from own docs.** Allied-health-focused searches where PubMed's biomedical bias under-represents AHP journals.
- **Citation/output pattern.** Per-record bibliographic entry + abstract (full text depends on library subscription).
- **Access constraint.** **Subscription-only**; NHS staff in the UK typically access via OpenAthens (NHS England library service) [general knowledge]. **Named gap:** EBSCO/CINAHL self-documentation not retrieved in this pass — the framing on UK Athens access reality is not re-verified against EBSCO's current 2026 docs.
- **Named gap.** Whether a contracting CPD tutor (not NHS-employed) retains Athens access between contracts is unconfirmed. Likely depends on Honorary Contract status with each Trust. Build implication: tutor may or may not have CINAHL access depending on contract state.

---

#### 1.8 Cochrane Library

- **What it does best.** *"The Cochrane Library is a collection of high-quality, independent evidence to inform healthcare decision-making, including the Cochrane Database of Systematic Reviews and the CENTRAL register of controlled trials"* [5]. Sharpest single-shot use: **systematic-review retrieval** (Cochrane SRs are widely treated as the highest-tier evidence aggregator in healthcare; CENTRAL is the canonical RCT register for SR-quality searches).
- **What it doesn't do.** Not a clinical-decision tool (it's an evidence repository, not a recommendation engine). Not real-time updated (SRs have long production cycles; some reviews may be outdated). Not AI-summarised at search-time (you read the SR yourself).
- **Trigger patterns from own docs.** "Has there been a systematic review on X?" + "What does the highest-tier evidence say about intervention Y for population Z?"
- **Citation/output pattern.** SR with structured sections (Abstract / Plain language summary / Background / Methods / Results / Discussion / Authors' conclusions). CENTRAL returns individual RCT records.
- **Access constraint.** *"All protocols and editorials are now published open access, all Cochrane reviews are free to read after 12 months. National provisions, paid..."* [6]. UK has a national provision (Cochrane UK funded via NIHR historically) — most UK users get free Cochrane Library access. **Named gap:** current 2026 UK national-provision status (post-NIHR funding changes) not re-verified.
- **Named gap.** Cochrane Reviews are the highest-tier evidence aggregator but not all clinically-important questions have a current Cochrane SR — coverage is uneven across physio topics.

---

#### 1.9 Google Scholar

- **What it does best.** Broadest open-web academic search; covers grey literature, preprints, theses, books, and journals well beyond PubMed/CINAHL/Cochrane's curated boundaries. Useful for forward-citation tracking ("cited by") and full-text PDF discovery via host-site links.
- **What it doesn't do.** No quality filter (papers from low-quality / predatory journals appear alongside high-tier journals with no warning). No MeSH-equivalent controlled vocabulary. No systematic-search reproducibility (results change over time, undisclosed ranking). Not suitable as a sole source for systematic-review-grade searches.
- **Trigger patterns from own docs.** Quick paper discovery, forward-citation tracking, finding open PDFs of paywalled papers.
- **Citation/output pattern.** Per-result snippet + cited-by count + versions list + PDF link (if discoverable).
- **Access constraint.** **Free.** No geographic restriction. Full-text availability depends on host site.
- **Named gap.** Google Scholar's self-documentation on coverage, ranking algorithm, and quality controls is intentionally sparse — boundary documentation is mostly third-party (LibGuides, librarian blogs).

---

### Clinical guidelines (UK + international)

---

#### 1.10 NICE NG128 — Stroke and transient ischaemic attack in over 16s

- **What it does best.** *"This guideline covers interventions in the acute stage of a stroke or transient ischaemic attack (TIA). It offers the best clinical advice on the diagnosis and acute management of stroke and TIA in the 48 hours after onset of symptoms"* [7]. Reference number NG128; published 01 May 2019; last updated 13 April 2022; last reviewed 27 March 2026 (no recommendation changes prioritised). Replaces CG68 (2008). Authoritative for the **acute (≤48h) stroke window** in the UK NHS.
- **What it doesn't do.** Does NOT cover rehabilitation phase (NG236 does — see 1.11). Does NOT cover prevention. The PubMed record explicitly notes: *"This guideline is a stand-alone document, but is designed to be read alongside the Intercollegiate Stroke Working Party guideline 'National clinical guideline for stroke' which considers evidence for interventions from the acute stage into rehabilitation and life after stroke"* [8].
- **Trigger patterns from own docs.** Acute-stage clinical questions: rapid recognition + diagnosis; imaging for suspected TIA; specialist care + pharmacological treatments + thrombectomy for acute ischaemic stroke; maintenance/restoration of homeostasis; nutrition + hydration; optimal positioning + early mobilisation; decompressive hemicraniectomy [7].
- **Citation/output pattern.** Web HTML guideline sections + downloadable PDF. Each recommendation is numbered and cross-linked to evidence reviews + committee discussion documents.
- **Access constraint.** **Free, open access** on nice.org.uk. No login required for the guideline text. **Note for AI builds:** NICE guideline pages are HTML, scrapeable, and stable URLs (anchor-linked to recommendation sections).
- **Named gap.** Whether NICE NG128 includes guidance on stroke-rehab-relevant outcome measures (Barthel, FIM, Stroke Impact Scale) is not unpacked here — likely partial (e.g., positioning + early mobilisation in NG128, but main rehab outcome guidance sits in NG236).

---

#### 1.11 NICE NG236 — Stroke rehabilitation in adults

- **What it does best.** *"This guideline covers rehabilitation after stroke for over 16s. It aims to ensure people are assessed for common problems and conditions linked to stroke, and get the care and therapy they need. It includes recommendations on the organisation and delivery of rehabilitation in hospital and the community"* [9]. Reference number NG236; published 18 October 2023. Authoritative for the **rehabilitation phase** in the UK NHS — the load-bearing guideline for stroke-rehab CPD educators.
- **What it doesn't do.** Does NOT cover acute (≤48h) management — that's NG128. Does NOT cover primary stroke prevention.
- **Trigger patterns from own docs (per scope summary).** Intensity of stroke rehabilitation; assessment for fatigue + vision + hearing problems; mouth care + swallowing + walking assessments and interventions; managing shoulder pain + spasticity; transfer of care from hospital to community including early supported discharge; telerehabilitation; community participation programmes + return-to-work programmes; organising health and social care for people needing rehabilitation; planning rehabilitation [9].
- **Citation/output pattern.** Same as NG128 — HTML guideline + PDF; per-recommendation anchor links.
- **Access constraint.** **Free, open access** on nice.org.uk.
- **Named gap.** Whether NG236 explicitly takes positions on Bobath / task-specific training / motor-learning approaches (the contested-claim space the AI debates) is not unpacked here — scope-level only was retrieved; the recommendation-level positioning on contested therapeutic schools is a separate question for the build (likely needs targeted retrieval at examples.md / reference/schools/<n>.md drafting time).

---

#### 1.12 RCP National Clinical Guideline for Stroke (2023)

- **What it does best.** *"The 2023 edition is endorsed for use in clinical practice by the Royal College of Physicians of London, SIGN and the Royal College of Physicians of Ireland"* [10]. Produced by the Intercollegiate Stroke Working Party. Authoritative UK + Ireland cross-stage stroke guideline — spans acute, rehabilitation, and life-after-stroke (broader scope than NICE NG128 + NG236 combined; NG128 was designed to be read alongside the RCP guideline per [8]).
- **What it doesn't do.** Not legally binding in NHS commissioning the way a NICE NG can be referenced in commissioning standards (NICE NGs have a specific commissioning role; RCP guidelines are professional-body endorsements). Not always synchronised with the most recent NICE NG — version cycles differ.
- **Trigger patterns from own docs.** Cross-stage stroke care, including areas NICE guidelines under-cover (e.g., chronic-stage rehabilitation, return to work, longer-term life after stroke, integrated service-organisation recommendations).
- **Citation/output pattern.** Web platform at strokeguideline.org + downloadable formats. Per-section recommendations with evidence levels.
- **Access constraint.** **Free, open access**. UK-anchored (endorsed by RCP London + SIGN + RCP Ireland).
- **Named gap.** Exact 2026 version state (whether a 2024 or 2025 update has superseded the 2023 edition) not re-verified — search returned "2023 edition" as the current state per [10]. The PMC commentary article [11] confirms 2023 as the new release at time of writing.

---

#### 1.13 AHA/ASA guidelines (American Heart Association / American Stroke Association)

- **What it does best.** US-anchor stroke clinical guidelines (e.g., 2019 Guidelines for Early Management of Acute Ischemic Stroke; 2023 prevention guidelines). Useful for **US-context comparison** + access to interventions evaluated in US healthcare delivery context (different reimbursement + service-line patterns than NHS).
- **What it doesn't do.** Not authoritative for UK NHS clinical practice. Treatment-pathway differences (e.g., tPA windows, thrombectomy criteria, secondary-prevention regimens) reflect US-specific service patterns; tutor must NOT teach AHA/ASA recommendations as UK best-practice.
- **Trigger patterns from own docs.** US-clinician audiences; international evidence comparison; secondary-pass when UK guidelines under-cover a specific question.
- **Citation/output pattern.** Per-recommendation tables with Class (I/IIa/IIb/III) + Level of Evidence (A/B/C) ratings. Published in *Stroke* journal + ahajournals.org.
- **Access constraint.** Free abstract; full PDF often free via ahajournals.org for AHA guidelines specifically.
- **Named gap.** AHA/ASA 2026 guideline-version landscape not retrieved this pass (multiple separate guidelines exist for prevention, acute management, secondary prevention — not all unpacked).

---

### UK clinical decision support (curated, point-of-care)

---

#### 1.14 iatroX

- **What it does best.** Per an earlier pass [ref 6]: *"iatroX bridges the gap between research and clinical practice for UK clinicians. It does not search the open literature — it retrieves guideline-grounded answers from NICE, CKS, SIGN, BNF, and other trusted UK sources. Every answer is cited, every recommendation is traceable, and the platform is MHRA-registered as a medical device."*
- **What it doesn't do.** iatroX itself names the boundary: *"AI research tools and clinical decision support tools are different categories... Confusing them at the bedside is a patient safety risk. Research tools are for exploring. Clinical tools are for deciding"* [ref 6]. This is the canonical citation identity.md should anchor on for the upstream-of-both safety frame.
- **Trigger patterns from own docs.** UK clinicians asking guideline-grounded clinical questions at point-of-care; CPD-logging the research question + reflection (CPD export feature).
- **Citation/output pattern.** Cited guideline-grounded answer + traceable to NICE/CKS/SIGN/BNF source.
- **Access constraint.** UK-specific. MHRA-registered medical device. **Named gap:** exact tier-pricing (free/paid; NHS-bulk vs individual) not retrieved — no call was allocated to it.
- **Named gap.** iatroX's self-documented boundaries on areas it does NOT cover (e.g., research-grade evidence appraisal, contested-claim navigation) are inferable from its positioning but not directly quoted from a single-page iatroX doc.

---

#### 1.15 NICE CKS (Clinical Knowledge Summaries)

- **What it does best.** *"Providing primary care practitioners with a readily accessible summary of the current evidence base and practical advice on best practice"* [12]. Curated topic summaries covering common primary-care conditions; each summary aggregates NICE guidance + other evidence into a clinically-actionable digest.
- **What it doesn't do.** **Geographically restricted.** *"The NICE Clinical Knowledge Summaries (CKS) site is only available to users in the UK, Crown Dependencies and British Overseas Territories"* [12]. **Critical implication for AI builds:** scraping CKS from a non-UK IP fails; building UK-context AI tooling that routes to CKS requires assuming UK-network access for the user. Third-party summary notes *"The end decision rests with the clinician. • CKS Evidence Summaries provide both foreground and background knowledge for primary care staff"* [13].
- **Trigger patterns from own docs.** Primary-care clinician asking "what's the current best-practice summary for condition X?" Stroke-rehab CPD tutors will find CKS topics on **stroke and TIA**, **secondary prevention**, **rehab-relevant comorbidities** (spasticity management overlap with spasticity in MS / SCI / brain injury).
- **Citation/output pattern.** Web-based summary pages structured by clinical question; references cite back to NICE guidelines + Cochrane + other evidence.
- **Access constraint.** **UK-only IP geofence** [12]. Free at point of use. NHS staff have direct access; contracting CPD tutors in the UK have access from UK IPs.
- **Named gap.** Coverage depth for **stroke rehabilitation specifically** (vs acute stroke vs stroke prevention) — CKS's topic-level scope page for stroke rehab was not retrieved.

---

#### 1.16 BNF (British National Formulary)

- **What it does best.** *"British National Formulary (BNF) Key information on the selection, prescribing, dispensing and administration of medicines"* [14]. Third-party publisher description: *"Practical and evidence based, British National Formulary (BNF) is the only drug formulary in the world that is both independent, and has rigorous, accredited content creation processes"* [15]. Sharpest single-shot use: **pharmacology lookups** — drug-specific indication / dose / interaction / cautions.
- **What it doesn't do.** **Geographically restricted.** *"The NICE British National Formulary (BNF) site is only available to users in the UK (England, Scotland, Wales and Northern Ireland)"* [14]. Not a clinical-decision-support tool for non-pharmacological interventions. Not a guideline retrieval tool (drug-focused only).
- **Trigger patterns from own docs.** Drug-specific questions (e.g., "what's the BNF entry for baclofen in spasticity?"; "what's the dose for anticoagulants post-stroke?"). For **stroke-rehab CPD educators**: most likely use is the pharmacology-and-rehab overlap (e.g., spasticity agents, anticoagulants, antiplatelets, post-stroke pain management). Less likely to be load-bearing for the build's core debate workflows.
- **Citation/output pattern.** Per-drug monograph (indications, dose, interactions, cautions, side effects, manufacturer details).
- **Access constraint.** **UK-only IP geofence** [14]. Free for UK NHS users at point of use. Print BNF also widely available via NHS.
- **Named gap.** Boundary on **clinical-decision support that depends on drug context** (e.g., spasticity management as a multimodal decision) — BNF gives drug-side input only; the multimodal decision sits with prescriber + physio jointly.

---

### Physio-specific evidence ratings

---

#### 1.17 PEDro (Physiotherapy Evidence Database) + PEDro scale

- **What it does best.** Free physiotherapy-specific evidence database with quality-rated RCTs / systematic reviews / clinical-practice guidelines. **PEDro scale** is a quality-rating scale specifically for RCTs in physio research; rates each RCT 0-10 on methodological quality.
- **PEDro scale mechanics (self-documented).** *"The PEDro scale was last amended on 21 June 1999. This briefly explains why each item has been included in the PEDro scale. More detail on each item is provided in the PEDro scale training program"* [16]. Per third-party clinimetric review of the scale: *"A total PEDro score is achieved by adding the ratings of items 2 to 11 for a combined total score between 0 to 10. Higher scores indicate superior..."* [17] (presumably "methodological quality" — quote cut by snippet length). **11 items total; item 1 (eligibility criteria) is for external validity and is NOT counted in the 0-10 score** — items 2-11 are summed.
- **What it doesn't do.** PEDro scale rates **methodological quality of RCTs**, NOT magnitude of effect or clinical importance. A 10/10 PEDro trial with a tiny effect size is still a tiny effect. PEDro scale is also NOT a measure of evidence-base certainty (that's GRADE / similar) — a high PEDro score on one trial is not the same as a high-certainty evidence base on the question.
- **Trigger patterns from own docs (per PEDro database structure).** "What's the PEDro score of trial X?"; "Are there high-quality RCTs on intervention Y in population Z?"; "Filter physio-RCT searches by minimum PEDro score."
- **Citation/output pattern.** Per-trial record with bibliographic details + PEDro score breakdown (which of 11 items satisfied) + abstract + link to full paper.
- **Access constraint.** **Free, no UK-specific geofence**.
- **Named gap.** Whether PEDro scores are routinely available for **recent (2023-2026) trials in stroke rehab** is question-specific. PEDro coverage depends on volunteer-rater throughput — gap on individual trials may exist.

---

#### 1.18 Physiopedia

- **What it does best.** Free, volunteer-curated physio-specific wiki. *"Physiopedia is a registered charity (UK registration 1173185) providing free, evidence-based physiotherapy knowledge to professionals worldwide. We're often called 'Wikipedia for physiotherapy' but with a crucial difference: every piece of content is created, reviewed, quality assured and maintained by qualified physiotherapy professionals through rigorous editorial oversight"* [18]. *"Every month, 4 million people from nearly every country trust Physiopedia"* [18]. 5,500+ registered editors; 50+ active monthly editors; launched 2009 by Rachael + Tony Lowe.
- **What it doesn't do — load-bearing self-disclaimer.** From the Physiopedia:About page directly [18]:

  > *"When refering to evidence in academic writing, you should always try to reference the primary (original) source. That is usually the journal article where the information was first stated. In most cases Physiopedia articles are a secondary source and so should not be used as references. Physiopedia articles are best used to find the original sources of information (see the references list at the bottom of the article)."*

  And the footer disclaimer [18]:

  > *"The content on or accessible through Physiopedia is for informational purposes only. Physiopedia is not a substitute for professional advice or expert medical services from a qualified healthcare provider."*

  **Implication for the build:** Physiopedia is a **navigation aid to find primary sources**, NOT a primary source itself. A CPD tutor citing "Physiopedia says X" against an attendee challenge is citing a secondary source that itself tells them to cite the primary. This is exactly the kind of citation-discipline the AI must encode.
- **Trigger patterns from own docs.** Topic overview + "find the primary sources" entry point. PAI (Physiopedia AI Assistant) launched 2024 per [18]; member-news framing says March 2026 launch [ref 1] — versioning ambiguous, possibly initial vs current-tier launch.
- **Citation/output pattern.** Wiki article structured by topic + reference list at bottom. Tutor's correct use: skim the article for orientation, then click through to the cited primary sources.
- **Access constraint.** **Free.** No geographic restriction.
- **Named gap.** Quality-assurance framework details linked from About page [18] not separately retrieved this pass.

---

#### 1.19 Physiotutors ChatCPG (already covered earlier)

Cross-reference: competitive-landscape.md Cat C [ref 2]. No boundary update — this is a competitor product, not a tool the build routes to. Mentioned here for completeness of the physio-specific landscape.

---

## 2. Claim-type → candidate-tool mapping

**Per task brief: candidates only, no winners.** James picks the routing tree shape in main context after reading this.

| Claim type the tutor is investigating | Candidate tools (alphabetical) |
|---|---|
| **Specific paper / PMID / DOI lookup** | Google Scholar, PubMed, Semantic Scholar |
| **Systematic-review-grade evidence on intervention X** | Cochrane Library, PubMed (filter for SR), Elicit (if "find SRs" framing), PEDro (for SRs included in their database) |
| **Effect-size estimate for intervention X in population Y** | Cochrane Library (SR meta-analysis), Elicit (extraction table), PubMed (original trial) |
| **Yes/No claim verification ("does X work for Y?")** | Consensus (Consensus Meter), Cochrane Library (SR conclusion), Elicit (custom claim verification) |
| **Trial-quality assessment for a named RCT** | PEDro (PEDro scale), scite.ai (citation-context verification) |
| **Forward-citation tracking ("who has cited paper X")** | Google Scholar (cited-by), scite.ai (citation contexts), Semantic Scholar (citation graph) |
| **UK acute stroke management (≤48h)** | NICE NG128, RCP National Clinical Guideline for Stroke 2023 |
| **UK stroke rehabilitation guidance** | NICE NG236, RCP National Clinical Guideline for Stroke 2023 |
| **UK primary-care clinical summary (cross-condition)** | NICE CKS (UK IPs only) |
| **UK pharmacology (drug-specific)** | BNF (UK IPs only), iatroX (synthesises BNF + others) |
| **UK guideline-grounded clinical-decision-support point-of-care** | iatroX |
| **International comparison (US-anchor)** | AHA/ASA guidelines |
| **Physio-specific topic orientation + primary-source discovery** | Physiopedia (then navigate to primary sources per its own disclaimer) |
| **Allied-health / nursing journal coverage** | CINAHL (subscription / Athens) |
| **General-purpose academic search with inline citations** | Perplexity (academic focus mode), Semantic Scholar |
| **Citation-context check before quoting a paper** | scite.ai |

**Cross-claim observations (evidence-only, no judgements):**
- **UK IP geofence applies to:** NICE CKS [12], BNF [14]. Not to: NICE NGs (NG128, NG236) themselves, RCP guideline, Cochrane Library (UK national provision), PubMed, PEDro, Physiopedia, Google Scholar.
- **Subscription / institutional access needed for:** CINAHL (via Athens), scite.ai (paid tiers), Elicit (advanced features), Consensus (advanced features). Free at point of use: PubMed, PEDro, Cochrane Library (UK), NICE guidelines, RCP guideline, Physiopedia, Google Scholar, NICE CKS (UK), BNF (UK).
- **AI-curated synthesis (vs raw-retrieval):** Elicit, Consensus, Perplexity, scite.ai (the Cat-A research tools) + iatroX (Cat-B clinical-decision-support). Raw retrieval: PubMed, CINAHL, Cochrane Library, Google Scholar, PEDro, NICE/RCP/BNF/CKS direct.
- **Citation-discipline self-disclaimer (i.e., the tool's own docs say "don't cite us, cite the primary"):** Physiopedia [18] — explicit primary-source disclaimer. Implicit equivalents: Wikipedia equivalent for medicine (not relevant here); secondary-source pattern applies to any wiki/digest tool the AI surfaces.

---

## 3. Named gaps + uncertainties

Not yet retrieved:

1. **2026 free-tier limits for Elicit + Consensus + scite.ai.** Pricing tier boundaries determine whether a contracting tutor (no institutional subscription) can use these in their daily workflow without paying. Likely all three have meaningful free tiers + paid upgrades, but exact 2026 limits not retrieved.

2. **iatroX self-documented boundaries.** An earlier pass quoted iatroX's research-vs-clinical-tools framing — that's load-bearing. But iatroX's own naming of areas it does NOT cover (research-grade evidence appraisal, contested-claim navigation, non-UK guidelines) is not retrieved from a single iatroX doc; it's inferable from the positioning.

3. **NICE NG236 contested-school positioning.** Whether NG236 takes recommendation-level positions on Bobath / task-specific training / motor learning is not unpacked here — only the scope was retrieved [9]. **Resolution path:** when drafting `reference/schools/<n>.md` files or `examples.md`, retrieve NG236's specific recommendations on motor recovery + functional training. The scope here was tool-boundary, not in-tool claim retrieval.

4. **CINAHL UK NHS Athens access reality for contracting tutors.** An earlier pass framed it as "UK NHS-accessible via Athens"; this pass did not re-verify whether contracting CPD tutors retain Athens access between contracts (likely depends on Honorary Contract status per Trust). Build implication: AI cannot assume tutor has CINAHL access; routing to CINAHL requires fallback to PubMed if access fails.

5. **AHA/ASA 2026 guideline-version landscape.** Multiple AHA/ASA stroke guidelines exist (prevention, acute management, secondary prevention, rehab); the current 2026 version state for each was not unpacked. **Build implication:** if AHA/ASA gets cited as a secondary anchor, the AI must be specific about which AHA/ASA guideline (year + scope) — generic "AHA/ASA says X" is fragile.

6. **Cochrane UK national-provision status post-NIHR funding changes.** Cochrane self-doc says "National provisions, paid..." [6]; UK has had a national provision historically. The 2026 status of UK free access to Cochrane Library was not re-verified. **Build implication:** AI should not assume Cochrane SR full-text is universally free to UK users — abstract is always free; full text may have changed.

7. **Physiopedia PAI launch-date versioning (2024 vs March 2026).** An earlier pass cited "March 2026" launch [ref 1, members.physio-pedia.com]; Physiopedia:About says "in 2024 we launched the Physiopedia AI Assistant" [18, www.physio-pedia.com]. Possibly: initial limited launch 2024, full Plus-catalogue rollout March 2026. **Resolution:** not blocking — both confirm PAI exists and serves attendee side.

---

## Citations

1. **[web]** `https://elicit.com/` — Elicit homepage: *"AI for scientific research... search, summarize, extract data from, and chat with over 125 million papers. Used by over 2 million researchers in academia and industry"*; *"Elicit can find up to 1,000 relevant papers and analyze up to 20,000 data points at once."*

2. **[web]** `https://consensus.app/home/blog/getting-started-with-consensus-university-access/` — Consensus University Access blog: *"Consensus is an AI search engine for academic research. It searches over 200 million academic papers and uses language models to help find, understand."*

3. **[web]** `https://effortlessacademic.com/consensus-ai-review-for-literature-reviews/` — Third-party Consensus review (Effortless Academic, 2025): *"When asking Yes/No questions, Consensus attempts to give you a general consensus of the literature and report it using The Consensus Meter"*; *"In-depth review of Consensus AI for literature reviews... key limitations and pricing."*

4. **[web]** `https://pubmed.ncbi.nlm.nih.gov/` — PubMed homepage: *"PubMed® comprises more than 40 million citations for biomedical literature from MEDLINE, life science journals, and online books. Citations may include links to full text content from PubMed Central and publisher web sites."* Plus `https://www.nlm.nih.gov/medline/medline_overview.html`: *"MEDLINE is a primary component of PubMed, a literature database developed and maintained by the NLM National Center for Biotechnology Information (NCBI)."*

5. **[web]** `https://www.cochranelibrary.com/` — Cochrane Library homepage: *"The Cochrane Library is a collection of high-quality, independent evidence to inform healthcare decision-making, including the Cochrane Database of Systematic Reviews and the CENTRAL register of controlled trials."*

6. **[web]** `https://www.cochrane.org/about-us/news/cochranes-sustainable-path-open-access` — Cochrane sustainable open-access announcement: *"All protocols and editorials are now published open access, all Cochrane reviews are free to read after 12 months. National provisions, paid..."*

7. **[web]** `https://www.nice.org.uk/guidance/ng128` — NICE NG128: *"This guideline covers interventions in the acute stage of a stroke or transient ischaemic attack (TIA). It offers the best clinical advice on the diagnosis and acute management of stroke and TIA in the 48 hours after onset of symptoms."* Published 01 May 2019; updated 13 April 2022; last reviewed 27 March 2026.

8. **[web]** `https://pubmed.ncbi.nlm.nih.gov/21698846/` — PubMed record for the NICE/RCP CG68 predecessor: *"This guideline is a stand-alone document, but is designed to be read alongside the Intercollegiate Stroke Working Party guideline 'National clinical guideline for stroke'..."*

9. **[web]** `https://www.nice.org.uk/guidance/ng236` — NICE NG236: *"This guideline covers rehabilitation after stroke for over 16s. It aims to ensure people are assessed for common problems and conditions linked to stroke, and get the care and therapy they need. It includes recommendations on the organisation and delivery of rehabilitation in hospital and the community."* Published 18 October 2023.

10. **[web]** `https://www.strokeguideline.org/` — RCP National Clinical Guideline for Stroke: *"The 2023 edition is endorsed for use in clinical practice by the Royal College of Physicians of London, SIGN and the Royal College of Physicians of Ireland."*

11. **[web]** `https://pmc.ncbi.nlm.nih.gov/articles/PMC11091392/` — PMC commentary on new National Clinical Guideline for Stroke (2023): *"The new National Clinical Guideline for Stroke (2023) provides authoritative, evidence-based practice guidance to improve the quality of care delivered..."*

12. **[web]** `https://cks.nice.org.uk/` — NICE CKS homepage: *"Providing primary care practitioners with a readily accessible summary of the current evidence base and practical advice on best practice."* Plus geofence notice: *"The NICE Clinical Knowledge Summaries (CKS) site is only available to users in the UK, Crown Dependencies and British Overseas Territories."*

13. **[web]** `https://www.uhl-library.nhs.uk/cl/pdfs/poc14_cks.pdf` — UHL NHS library third-party summary of CKS: *"The end decision rests with the clinician. • CKS Evidence Summaries provide both foreground and background knowledge for primary care staff."*

14. **[web]** `https://bnf.nice.org.uk/` — BNF NICE homepage: *"British National Formulary (BNF) Key information on the selection, prescribing, dispensing and administration of medicines."* Plus: *"The NICE British National Formulary (BNF) site is only available to users in the UK (England, Scotland, Wales and Northern Ireland)."*

15. **[web]** `https://www.pharmaceuticalpress.com/content/british-national-formulary/` — Pharmaceutical Press BNF publisher page: *"Practical and evidence based, British National Formulary (BNF) is the only drug formulary in the world that is both independent, and has rigorous, accredited content creation processes."*

16. **[web]** `https://pedro.org.au/english/resources/pedro-scale/` — PEDro scale resource page: *"The PEDro scale was last amended on 21 June 1999. This briefly explains why each item has been included in the PEDro scale. More detail on each item is provided in the PEDro scale training program."*

17. **[web]** `https://www.sciencedirect.com/science/article/pii/S183695531930092X` — Clinimetrics: Physiotherapy Evidence Database (PEDro) Scale (ScienceDirect): *"A total PEDro score is achieved by adding the ratings of items 2 to 11 for a combined total score between 0 to 10. Higher scores indicate superior..."*

18. **[web]** `https://www.physio-pedia.com/Physiopedia:About` — Physiopedia About page: *"When refering to evidence in academic writing, you should always try to reference the primary (original) source. That is usually the journal article where the information was first stated. In most cases Physiopedia articles are a secondary source and so should not be used as references. Physiopedia articles are best used to find the original sources of information (see the references list at the bottom of the article)."* Plus: *"Physiopedia is a registered charity (UK registration 1173185)... Every month, 4 million people from nearly every country trust Physiopedia... 5,500+ editors and 50 active volunteers..."* Plus footer: *"The content on or accessible through Physiopedia is for informational purposes only. Physiopedia is not a substitute for professional advice or expert medical services from a qualified healthcare provider."*

---

## Open questions surfaced

- 2026 free-tier limits for Elicit / Consensus / scite.ai
- NG236 recommendation-level positioning on contested therapeutic schools
- CINAHL Athens access continuity for contracting tutors between NHS Trust contracts
- Cochrane UK national-provision 2026 status post-NIHR funding changes
- iatroX self-documented boundaries on what it does NOT cover (single-doc citation)

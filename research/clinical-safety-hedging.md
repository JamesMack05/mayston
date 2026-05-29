---
topic: comp-6-clinical-safety-hedging
date: 2026-05-27
description: Source-cited clinical-safety hedging language and safety-positioning evidence for the Comp 6 build.
---

# Research: Clinical-safety hedging patterns + safety positioning sources for Comp 6 build

**Query (restated):** Capture concrete, source-cited hedging language + safety-positioning evidence the AI build can encode in `identity.md` and `rules.md`. Four sub-targets: (1) hedging language patterns (Cochrane / NICE / PEDro / Consensus / Elicit / GRADE); (2) UK + US medical-device regulatory boundary (MHRA / FDA SaMD); (3) AI clinical-decision-support distinction (BMJ / NICE ESF / CSP / NHS England); (4) founder-credibility hedging-vs-overclaim patterns.

**Mode:** evidence-gathering — gaps named explicitly below.

## Sources consulted

- Prior research: `competitive-landscape.md` ref [6] (iatrox.com safety distinction) + `schools-landscape.md` (Mayston Bobath-as-framework + thin-evidence Brunnstrom/Peto hedging) are already canonical; not re-fetched.
- Web: 10 firecrawl-search calls with `--scrape` flag (GRADE; Cochrane PLS / stroke review; PEDro scale; Consensus Meter; NICE/GRADE Guyatt 2008; MHRA SaMD; FDA AI/ML SaMD; NHS England gen-AI scribing guidance; CSP AI principles; iatroX landscape + introducing-iatroX). 2/12 spare.
- NotebookLM: 0 (no relevant loaded notebook).

**Tools used:** find (Bash), Grep, Read, firecrawl-search (×10 with --scrape), Write, Edit.

**Cap-hit:** No (10/12 used).

---

## Verdict

This artefact is evidence-gathering only — it gathers and grades sources; it does not decide which to embed in `identity.md` / `rules.md`, or how to phrase them.

---

## Sub-target 1 — Hedging language patterns (sourced verbatim examples)

### 1a. GRADE certainty-of-evidence four levels — canonical wording

GRADE is the dominant international framework. Adopted by **over 110 organisations** worldwide including WHO, CDC, NHS, Cochrane Collaboration, and **UpToDate / DynaMed** (which have *"tens of thousands of graded recommendations using this approach"*) [Prasad 2024, citation 2].

**Verbatim — the four certainty levels** (GRADE Handbook, Table 2) [1]:

> | **High certainty** | There is high confidence that the true value of the estimate of interest is on one side of a threshold of interest or within a specific range. |
> | **Moderate certainty** | There is moderate confidence that the true value of the estimate of interest is on one side of a threshold of interest or within a certain range. The true value of the estimate may deviate slightly from the target of the certainty rating (i.e. may possibly fall in a different range). |
> | **Low certainty** | There is low confidence that the true value of the estimate of interest is on one side of a threshold of interest or within a certain range. The true value of the estimate may deviate from the target of the certainty rating (i.e. likely fall in a different range). |
> | **Very-Low certainty** | There is very-low confidence that the true value of the estimate of interest is on one side of a threshold of interest or within a certain range. The true value of the estimate may deviate significantly from target of the certainty rating (i.e. probably fall in a different range). |

**Verbatim — Guyatt et al. (BMJ 2008, GRADE Working Group) standardised intervention-effect phrasings** [Prasad 2024 ref + Guyatt 2008 source 2]:

> - High certainty: *"High-certainty evidence comes from well-conducted studies with consistent results and minimal risk of bias, and it is unlikely that further research will significantly change the confidence in the estimate."*
> - Moderate certainty: *"Moderate certainty suggests that the available evidence is sufficient to support a conclusion, but further research may still impact the confidence in the estimate. Moderate-certainty evidence may arise from studies with limitations, inconsistencies, or a possibility of bias, or when there is a lack of high-quality evidence."*

**Verbatim — Cochrane Library's standard footnote on GRADE grades** (from Langhorne 2018 stroke mobilisation review, "Summary of findings") [3]:

> | GRADE Working Group grades of evidence
> | **High quality:** Further research is very unlikely to change our confidence in the estimate of effect.
> | **Moderate quality:** Further research is likely to have an important impact on our confidence in the estimate of effect and may change the estimate.
> | **Low quality:** Further research is very likely to have an important impact on our confidence in the estimate of effect and is likely to change the estimate.
> | **Very low quality:** We are very uncertain about the estimate. |

This is the **Cochrane footnote pattern** that appears verbatim in thousands of Cochrane SoF tables. It's tighter than the 2024 GRADE Handbook wording and likely the most-cited hedging phrasing in physio EBP.

**Verbatim — GRADE phrase patterns for intervention conclusions** (synthesis of Guyatt 2008 + GRADE Handbook 2024 Table 2 wording):

| Certainty | Standard phrasing pattern for "intervention X improves outcome Y" |
|---|---|
| High | "X **improves** Y" / "the intervention **results in** [outcome]" |
| Moderate | "X **probably improves** Y" / "the intervention **probably results in** [outcome]" |
| Low | "X **may improve** Y" / "the intervention **may result in** [outcome]" |
| Very low | "the effect of X on Y is **very uncertain**" / "**we are very uncertain** whether X improves Y" |

*Note: the four-row phrase ladder above is documented across multiple GRADE methodology papers but the exact wording table at this level of compression was not located in a single primary source within the web-cap — see § Named gaps.*

### 1b. Cochrane plain-language summary — verbatim hedging worked example

**Source:** Langhorne et al. 2018, "Very early versus delayed mobilisation after stroke" (Cochrane Database of Systematic Reviews) [3]. Stroke-rehab-domain — directly relevant to Comp 6's user.

**Verbatim "Authors' conclusions"** [3]:

> VEM, which usually involved first mobilisation within 24 hours of stroke onset, **did not increase** the number of people who survived or made a good recovery after their stroke. VEM **may have reduced** the length of stay in hospital by about one day, but this was based on **low-quality evidence**. Based on the potential hazards reported in the single largest RCT, the sensitivity analysis of trials commencing mobilisation within 24 hours, and the NMA, there was concern that VEM commencing within 24 hours **may carry an increased risk**, at least in some people with stroke. **Given the uncertainty around these effect estimates, more detailed research is still required.**

**Verbatim — embedded uncertainty acknowledgement** [3]:

> In addition to the uncertainties surrounding the optimal amount of rehabilitation that can be provided early after stroke, **exactly how early rehabilitation should start is controversial.**

This is the canonical Cochrane voice: explicit qualifier per claim (*"may have"*, *"based on low-quality evidence"*, *"may carry an increased risk"*) + closing call for more research. The hedging is structural, not decorative.

### 1c. PEDro scale 0-10 — interpretation + reporting in physio papers

**Source:** PEDro database (Physiotherapy Evidence Database, University of Sydney) [4].

**Verbatim — what the PEDro scale measures** [4]:

> Points are only awarded when a criterion is clearly satisfied. If on a literal reading of the trial report it is possible that a criterion was not satisfied, a point should not be awarded for that criterion.

**The 11 items** (item 1 is not scored; items 2-11 sum to a 0-10 score) [4]:
1. eligibility criteria specified (not scored — external validity only)
2. random allocation
3. concealed allocation
4. groups similar at baseline
5. blinding of all subjects
6. blinding of all therapists
7. blinding of all assessors
8. >85% follow-up on at least one key outcome
9. intention-to-treat analysis (or all received allocated treatment)
10. between-group statistical comparison reported
11. point + variability measures reported

**Verbatim — what PEDro is and isn't** (from PMC review "How to Classify Clinical Trials Using the PEDro Scale") [5]:

> The PEDro scale assists readers to quickly assess whether a clinical trial presents reliable and meaningful results for use in clinical practice.

**Reporting convention** (from physio-domain meta-analyses, e.g. Scrivener et al. 2020 captured in `schools-landscape.md` ref [1]):

> *"PEDro 2-8/10"* (across-trial range in Bobath SR) — used as a methodological-quality descriptor alongside the SMD effect size in narrative synthesis. The score is **not** itself a clinical-certainty rating like GRADE; it's a within-study methodological-rigour rating.

**Verbatim — Bobath SR worked example** (Scrivener et al. 2020 [schools-landscape ref 1]):

> *"Bobath therapy was inferior to task-specific training (SMD 0.48, 95% CI 0.01 to 0.95) for lower-limb activities. Prioritising Bobath therapy over other interventions is not supported by current evidence."*

PEDro and GRADE are **different but complementary**: PEDro scores individual-trial methodological quality (0-10); GRADE rates the certainty of the body of evidence across trials (high/moderate/low/very low).

### 1d. Consensus / Elicit — AI-research-tool hedging output patterns

**Source:** Consensus app official help docs + Effortless Academic 2025 review [6, 7].

**Verbatim — what the Consensus Meter is** [6]:

> The Consensus Meter helps you quickly understand the overall agreement or disagreement among research findings on a given topic. It provides a visual representation of whether the research leans more toward a "**Yes**", "**No**", "**Possibly**", or "**Mixed**". This makes it easier to gauge the prevailing scientific perspective quickly.

> Our AI analyzes the top 20 papers returned for your search query and categorizes their conclusions based on the claims they support. The Consensus Meter then displays these answers in a clear, easy-to-read format, highlighting only the most relevant information for your specific question.

> The Consensus Meter is powered by the most accurate results for your specific question and requires at least **5 relevant papers** to display results.

**Verbatim — explicit limitation language Consensus ships with its own UI** [6]:

> - **The Consensus Meter is not a perfect reflection of all the science on a topic.** The Consensus Meter is powered by the 5 to 20 most relevant results found for your specific search. It will not be a perfect reflection of the complete research that exists on a topic.
> - **The model will occasionally incorrectly classify results** – we have worked hard to give our model loads and loads of examples to learn from, but it is not infallible. We show you exactly which papers are contributing to the Consensus Meter and how we classified them.
> - **Specific nuance is missing** – one of the biggest limitations–that we are currently working to address–is that this feature does not always account for details included in the original question. For instance, if you ask, "Is ibuprofen safe for adult consumption?" and the potential result reads, "We found that ibuprofen was safe and well tolerated in children," our model may classify that result as "Yes."
> - **We do not have access to all research** – the Consensus database includes over 200 Million peer-reviewed papers. While this represents significant coverage, we don't yet have access to all scientific papers in the world.

This is **explicit ship-surface hedging** — Consensus publishes the limits of its tool inside the tool's help doc. Pattern: name the mechanism, name the limit, name the failure-mode example.

**Verbatim — Consensus Snapshot four indicators** [6]:

> - **Recency:** the average publish date of the papers in each position
> - **Methods:** the count of papers in each position that are Meta Analyses, Systematic Reviews or RCTs
> - **Journals:** the average SJR score for the publishing journals across the papers in each position
> - **Citations:** the sum of citations across the papers in each position

Each position is tagged with quality indicators rather than a single confidence score.

**Elicit's hedging shape** — *not directly retrieved within web-cap*; from `competitive-landscape.md` ref [6] iatrox.com market-overview: Elicit's output is structured data extraction across N papers as **tables**, not synthesis. The hedging happens at row-level (e.g., per-paper sample size, study design, key finding columns) rather than via a single confidence rating. See § Named gaps.

### 1e. NICE evidence summary — tier language

**Source:** Guyatt et al. 2008 (BMJ, GRADE Working Group) [8] — canonical paper articulating the four-tier framework that NICE (alongside Cochrane and WHO) adopted.

**Verbatim — Guyatt 2008 GRADE four-level wording** [8]:

> GRADE offers four levels of evidence quality: high, moderate, low, and very low. Randomised trials begin as high quality evidence and observational studies as low quality evidence. Quality may be downgraded as a result of limitations in study design or implementation, imprecision of estimates (wide confidence intervals), variability in results, indirectness of evidence, or publication bias. Quality may be upgraded because of a very large magnitude of effect, a dose-response gradient, and if all plausible biases would reduce an apparent treatment effect.

> The quality of evidence reflects the extent to which confidence in an estimate of the effect is adequate to support a particular recommendation.

**NICE-specific evidence-tier wording** — *not retrieved as a single primary NICE-published methodology doc within the web-cap; NICE applies GRADE as its underlying methodology* (per Prasad 2024 and Guyatt 2008's enumeration of GRADE-adopting organisations including NHS / NICE-aligned guideline producers). For NICE-specific NG128 (stroke) or NG specific tier language in plain-language guideline summaries, see § Named gaps.

---

## Sub-target 2 — Medical-device regulatory boundary (MHRA + FDA)

### 2a. UK MHRA — software as a medical device

**Source:** GOV.UK MHRA "Medical devices: software applications" guidance, last updated 1 July 2023, plus MEDIcept summary [9, 10].

**Verbatim — GOV.UK MHRA guidance purpose** [9]:

> This guidance explains when a software application is considered a medical device and how the MHRA regulates such applications.

The primary regulatory PDF is *"Medical device stand-alone software including apps"* (43 pages, August 2014, last updated 1 July 2023) [9]. Appendices cover **symptom checkers**, **clinical calculators**, *"drives or influences the use of a device"*, and field safety warnings [9].

**Verbatim — MEDIcept summary on UK MDR 2002 + UKCA marking** [10]:

> In the UK, standalone software and apps that meet the definition of a medical device are still required to be UKCA marked under the UK MDR 2002 [...]

**Verbatim — current CE/UKCA acceptance window** (from NHS England AVT scribing guidance [11], which cites MHRA position):

> An ambient scribing product that is deemed to be a medical device needs to be registered with the Medicines and Healthcare products Regulatory Agency (MHRA) and regulated proportional to its risk classification. A **UK Conformity Assessed (UKCA) certificate** is needed for clinical use of medical devices in the NHS. A valid CE mark is equally acceptable until **30th June 2028**.

**Verbatim — MHRA Class 1 threshold for ambient scribing** [11]:

> The [NHS England AVT Supplier Registry] requires suppliers to hold at least **MHRA Class 1 Registration**.

**Verbatim — when AI software qualifies as a medical device** [11]:

> Ambient scribing products that inform medical decisions and have simple/low functionality (for example, products that solely generate text transcriptions that are easily verified by qualified users) are likely not medical devices. However, **the use of Generative AI for further processing, such as summarisation, would be treated as high functionality and likely would qualify as a medical device.**

This is the canonical UK-government statement on **where the generative-AI medical-device line sits.** Summarisation = likely medical device. Transcription alone = likely not.

### 2b. FDA — AI/ML SaMD framework

**Source:** FDA "Artificial Intelligence in Software as a Medical Device" page [12]. US analogue to MHRA.

**Verbatim — FDA definitions** [12]:

> **Artificial Intelligence** is a machine-based system that can, for a given set of human-defined objectives, make predictions, recommendations, or decisions influencing real or virtual environments. Artificial intelligence systems use machine- and human-based inputs to perceive real and virtual environments; abstract such perceptions into models through analysis in an automated manner; and use model inference to formulate options for information or action.

> **Machine Learning** is a set of techniques that can be used to train AI algorithms to improve performance at a task based on data.

**Verbatim — premarket pathways** [12]:

> The FDA reviews medical devices through an appropriate premarket pathway, such as premarket clearance (510(k)), De Novo classification, or premarket approval. The FDA may also review and clear modifications to medical devices, including software as a medical device, depending on the significance or risk posed to patients of that modification.

**FDA AI/ML SaMD policy chronology** [12]:

> - April 2019 — Discussion paper: "Proposed Regulatory Framework for Modifications to Artificial Intelligence/Machine Learning (AI/ML)-Based Software as a Medical Device (SaMD)"
> - January 2021 — "Artificial Intelligence and Machine Learning Software as a Medical Device Action Plan" ("AI/ML SaMD Action Plan")
> - October 2021 — Good Machine Learning Practice for Medical Device Development: Guiding Principles
> - April 2023 — Draft Guidance: Marketing Submission Recommendations for a Predetermined Change Control Plan for AI/ML-Enabled Device Software Functions
> - October 2023 — Predetermined Change Control Plans for ML-Enabled Medical Devices: Guiding Principles
> - June 2024 — Transparency for Machine Learning-Enabled Medical Devices: Guiding Principles
> - December 2024 — Final Guidance: Marketing Submission Recommendations for a Predetermined Change Control Plan for AI-Enabled Device Software Functions
> - March 2024 — "Artificial Intelligence and Medical Products: How CBER, CDER, CDRH, and OCP are Working Together"
> - January 2025 — Draft Guidance: Artificial Intelligence-Enabled Device Software Functions: Lifecycle Management and Marketing Submission Recommendations

**Verbatim — FDA's framing of the regulatory challenge** [12]:

> The FDA's traditional paradigm of medical device regulation was not designed for adaptive artificial intelligence and machine learning technologies. Many changes to artificial intelligence and machine learning-driven devices may need a premarket review.

### 2c. What an unregistered tool MUST NOT do — evidence

This sub-question is the practical boundary the build needs to encode in `identity.md`. The clearest evidence chain:

**NHS England AVT (Apr 2025, updated Apr 2026)** — definitive on Generative AI processing that **summarises**: "would be treated as high functionality and likely would qualify as a medical device" [11]. By implication, unregistered tools must not produce summarised clinical outputs intended to inform medical decisions.

**MHRA GOV.UK** [9] — guidance qualifies a software application as a medical device when it has a medical purpose. **The 43-page PDF "Medical device stand-alone software including apps" is the primary document** but was not deep-scraped within the web-cap — see § Named gaps.

**iatroX self-positioning (pre-MHRA registration)** [13] is the clearest worked example of an unregistered tool's hedging language. Verbatim:

> Although it is not yet a formal clinical decision support system, we are actively exploring pathways to obtain medical device classification and develop direct integrations with electronic health records (EHRs).

> While it isn't yet a formal clinical decision support system, we are continuously evolving—actively exploring medical device classification and aiming for direct EHR integrations.

This is the **exact wording** an unregistered tool uses to disclaim CDS status while declaring directional intent. (iatroX subsequently obtained MHRA Class I registration; this is the *pre-registration* self-positioning.)

**iatroX post-registration self-positioning** [14] is the *post-MHRA* positioning:

> [iatroX] UK-focused clinical AI platform. MHRA-registered, UKCA-marked Class I medical device.

Both ship-surface positioning patterns are usable as **reference templates**: unregistered tools name what they are NOT (yet) + directional intent; registered tools name the regulatory status explicitly.

---

## Sub-target 3 — AI clinical-decision-support distinction (canonical sources)

### 3a. iatrox.com safety distinction — canonical citation

**Source:** `competitive-landscape.md` ref [6] (already captured). Verbatim quote restated for evidence-chain completeness:

> Research tools are for exploring. Clinical tools are for deciding. Confusing them at the bedside is a patient safety risk.

This is the load-bearing **categorical distinction** the Comp 6 build leans on.

### 3b. iatroX market-landscape framing (2026) — three-category taxonomy

**Source:** iatroX.com blog, "The Clinical AI Landscape in 2026" [14] (different article from ref [6]).

**Verbatim — the four categories iatroX names** [14]:

> **Category 1: General-Purpose AI Applied to Medicine** — ChatGPT, Claude, Gemini, Perplexity. *"No regulatory status in any jurisdiction. Variable guideline alignment — predominantly US-trained, potentially citing US guidelines for UK clinical questions. Documented hallucination risk in clinical contexts."*

> **Category 2: Clinician-Facing Clinical AI (Purpose-Built)** — OpenEvidence, iatroX (MHRA-registered, UKCA-marked Class I), Medwise AI, Glass Health, DxGPT. *"Some have regulatory status."*

> **Category 3: AI Scribes and Documentation** — Heidi Health, Tortus AI, Tandem Health, Nabla, Freed AI, Nuance DAX, Abridge. *"Scribes capture and document consultations. They do not answer clinical questions."*

> **Category 4: Enterprise Clinical AI** — ChatGPT for Healthcare, Microsoft Copilot for Healthcare, Doximity DoxGPT.

**Verbatim — iatroX's framing of the safety distinction (2026)** [14]:

> Scribes and clinical AI are complementary, not competing. A clinician might use Tortus or Tandem to document a consultation and Ask iatroX to check whether their management plan aligns with the latest NICE guideline. **Different tools for different moments in the same clinical workflow.**

**Verbatim — naming the regulation trajectory** [14]:

> The MHRA's National Commission into the Regulation of AI in Healthcare is developing recommendations. The UK will likely formalise requirements for clinical AI tools to hold medical device registration.

The Comp 6 build's natural placement in this taxonomy is **upstream of all four iatroX categories** — it's a CPD-prep partner, not a research tool, not a clinical AI, not a scribe, not enterprise. Categorising the build as "none of these" with named adjacents is a credibility move.

### 3c. CSP — Chartered Society of Physiotherapy AI principles (March 2025)

**Source:** CSP "AI principles in action" professional guidance [15, 16]. **Directly relevant** — this is the UK physio professional body governing the user our build serves.

**Verbatim — CSP framing** [15]:

> The CSP has published principles to guide the use of artificial intelligence in physiotherapy.

**Verbatim — Sylvia Wojciechowski (CSP Council Chair)** [15]:

> AI and the greater use of digital tools are not something we can afford to ignore. We recognise their immense potential to drive significant advancements in healthcare, particularly in physiotherapy. At the same time, we acknowledge the possible risks they pose to patient safety, confidentiality, and professional development, as well as the concerns some members have raised.

> These principles are intended to guide the responsible and beneficial use of AI and digital tools in physiotherapy while minimising the potential harms we are concerned about.

**Verbatim — review cadence** [15]:

> Given the pace of development the principles will be reviewed every six months for the next two years to ensure they remain relevant and effective.

**Verbatim — AI principle #1 (Transparency)** [16]:

> It should be clear to all stakeholders—patients, clinicians, staff and system partners—when AI is being used, what its role is, and how it may influence decisions.

> Open communication about AI use builds trust and supports informed engagement by patients and professionals alike.

**Verbatim — CSP on liability** [16]:

> The CSP PLI policy does not currently specifically address AI. AI use in physiotherapy is considered within the scope of physiotherapy practice and its use can function as both a product and a service. Liability for alleged malpractice relating to AI use is emerging and not fully established, but may include:
>
> - App developers - e.g. in scenarios where an AI app malfunctions in line with appropriate medical device regulations.
> - Clinical practitioners - e.g. related to scenarios assessing patient suitability to use AI or apps, and for providing proper guidance on their safe use.
> - Patients - e.g. if they do not use AI or apps as instructed.
> - Manufacturers - e.g. in scenarios related to product development, placing a product on the market, and development safeguards e.g. ability to spot red-flags if there is no human involvement.

**Verbatim — CSP on practice scope** [16]:

> AI should not replace the human tasks of professional responsibilities, holistic duties, nor professional curiosity.

The CSP **explicitly references** UK government medical-device guidance and the **Digital Technology Assessment Criteria (DTAC)** [16]:

> Guidance is also available to support members in the procurement and implementation of AI tools in practice. Amongst these are the government's guidance on the appropriate medical device regulation, and on innovation and procurement of technology products to the NHS in England, the Digital Technology Assessment Criteria (DTAC).

The CSP principles span six areas: **transparency, effectiveness, accountability, equity, risk management, scope-of-practice** (full text gated for member-login on the principles page; news article + sub-page captures the framing).

### 3d. NHS England guidance on Generative AI in clinical use (April 2025 / updated April 2026)

**Source:** NHS England "Guidance on the use of AI-enabled ambient scribing products in health and care settings" [11]. Published 27 April 2025, last updated 24 April 2026.

**Verbatim — purpose** [11]:

> This guidance offers high-level information to assist those adopting ambient scribing products that feature Generative Artificial Intelligence (AI), for use across health and care settings in England.

**Verbatim — Generative AI risk framing** [11]:

> Be mindful that products that use Generative Artificial Intelligence (AI) and Large Language Models (LLMs) may introduce new functions unintentionally or through user-provided instructions.

> A user might be able to provide instructions to get the product to generate an output that goes beyond the product's intended purpose, even if this is not the user's intent.

> Some users may use products outside the supervision of their setting, circumventing related policies and approvals.

**Verbatim — supplier safeguards required** [11]:

> Suppliers must add safeguards to their products [...] to stop misuse and ensure generated content stays within intended use.

**Verbatim — Clinical Safety Officer + DCB0160** [11]:

> Assign a Clinical Safety Officer and identify key risks [...] Complete the DCB0160 documentation [...] Ensure the supplier has completed the DCB0129 [...] develop a safety case, hazard log, and monitoring framework.

**Verbatim — review-before-action requirement** [11]:

> Ensure users review and approve any product outputs prior to further actions.

This is **the closest UK-NHS-specific generative-AI clinical-use guidance** available as of late 2025/early 2026. Domain is specifically ambient scribing, not CPD-prep, but the principles (intended purpose, review-before-action, supplier safeguards, generative-AI off-purpose drift risk) generalise.

### 3e. NICE evidence framework for digital health technologies (ESF)

*Not retrieved as a primary NICE-published document within the web-cap.* CSP guidance [16] cross-references the DTAC framework; the underlying **NICE Evidence Standards Framework (ESF) for digital health technologies** exists and tiers digital products by clinical risk, but the specific NICE ESF document and its tier definitions were not located in this pass. See § Named gaps.

### 3f. BMJ articles on AI clinical-decision-making vs research tools

*Not retrieved as a primary BMJ-published article within the web-cap.* The iatroX 2026 landscape article [14] and Guyatt 2008 GRADE methodology paper (BMJ) [8] are the closest BMJ-published / BMJ-adjacent evidence in this pass. Specific recent BMJ editorials on the AI-research-tool vs CDS distinction were not located. See § Named gaps.

### 3g. ACPIN-specific AI guidance

*Not retrieved.* ACPIN (Association of Chartered Physiotherapists in Neurology) is named as a target professional body in the brief; no ACPIN-specific AI guidance was located within the web-cap. CSP guidance is broader and would apply to ACPIN members by default since ACPIN is a CSP-affiliated network. See § Named gaps.

---

## Sub-target 4 — Founder-credibility hedging-vs-overclaiming reference patterns

This sub-target is **reference patterns, not prescriptions.** The Comp 6 build's `identity.md` opener + README must surface founder credibility honestly. Below are how other tools (referenced in the brief or surfaced during research) position theirs.

### 4a. iatroX pre-registration self-positioning (reference pattern: directional intent)

**Verbatim, pre-MHRA-registration self-positioning** [13]:

> Although it is not yet a formal clinical decision support system, we are actively exploring pathways to obtain medical device classification and develop direct integrations with electronic health records (EHRs).

Pattern shape: **(1) name what you are NOT yet** → **(2) declare directional intent** → **(3) do not pre-claim the credential**.

### 4b. iatroX post-registration self-positioning (reference pattern: regulatory-status-as-product-feature)

**Verbatim, post-MHRA-registration self-positioning** [14]:

> [iatroX] UK-focused clinical AI platform. MHRA-registered, UKCA-marked Class I medical device. Free. [Ask iatroX] retrieves and synthesises NICE guidelines, CKS summaries, peer-reviewed literature, and SmPC data — grounded in the authoritative sources UK clinicians actually use.

Pattern shape: **(1) regulatory status as headline feature** → **(2) named authoritative sources** → **(3) grounding-claim follows registration-claim, not before it**.

### 4c. iatroX limits-honest framing (reference pattern: scope-name-and-acknowledge-categorical-limits)

**Verbatim** [14]:

> Category limitations: Narrower scope than general-purpose AI — may not cover every administrative or non-clinical use case. Smaller user bases than ChatGPT.

Pattern shape: **explicitly publish your tool's limitations next to its strengths.** Mirrors Consensus Meter's published limits in 1d.

### 4d. CSP-published-by-named-body pattern

**Verbatim** [16]:

> These principles collectively represent the CSP's commitment to the ethical, equitable, and inclusive use of artificial intelligence (AI) in physiotherapy.

> AI is a fast moving subject. These principles will be reviewed every 6 months over the next 2 years and amendments made as required.

Pattern shape: **(1) named organisational authorship** → **(2) declared review cadence** → **(3) explicit acknowledgement of provisional-not-final status**.

### 4e. Founder-credibility surfacing pattern

The principle: surface founder credibility honestly on the visible ship-surface, not buried in system-prompt content.

> Founder-credibility attestation in README opener — visible-surface, NOT only in `coach/identity.md` system-prompt content.

> Internal rigour IS visible to skim-judges when named at quotable altitude with stable identifiers. [...] Naming-at-altitude with stable IDs is the visibility mechanism.

### 4f. Physiopedia / Physiopedia PAI founder-credibility positioning

*Not directly retrieved in this pass; `competitive-landscape.md` ref [1] captured the product framing but not the team page.* Physiopedia is named as a reference pattern in the brief; see § Named gaps.

### 4g. CSP liability-honesty pattern

**Verbatim** [16]:

> The CSP PLI policy does not currently specifically address AI. AI use in physiotherapy is considered within the scope of physiotherapy practice and its use can function as both a product and a service. Liability for alleged malpractice relating to AI use is emerging and **not fully established**.

Pattern shape: **honestly name the unresolved-state of professional liability rather than gloss it.**

---

## Named gaps (what we couldn't retrieve)

Per the evidence-only brief, named gaps are themselves load-bearing — the build's positioning must operate within these unknowns.

1. **NICE ESF (Evidence Standards Framework for digital health technologies) primary document.** CSP cross-references it; NHS England guidance cross-references the DTAC (which is related). The specific tier-definitions in the NICE ESF were not located within the 12-call cap. **Mitigation:** the GRADE four-tier framework (which NICE adopts for its evidence summaries broadly) covers the evidence-tier dimension; the ESF is a separate digital-tech-specific evidence tier that would require a dedicated retrieval.

2. **MHRA "Medical device stand-alone software including apps" PDF (43 pages).** This is the primary MHRA document on SaMD qualification. The GOV.UK landing page [9] was scraped; the PDF itself was not deep-scraped. **Mitigation:** the NHS England AVT guidance [11] directly cites the qualification threshold for Generative AI summarisation; that's the operative wording for the build's purposes.

3. **BMJ-specific editorial on AI research tools vs CDS.** The iatroX 2026 landscape article [14] is the most-substantive recent capture; Guyatt 2008 BMJ paper [8] covers the GRADE methodology. A dedicated BMJ editorial naming the research-tool / CDS distinction wasn't located, but the iatrox.com ref [6] already cites the distinction. **Mitigation:** the distinction is already canonical-cited in `competitive-landscape.md`.

4. **ACPIN-specific AI guidance.** ACPIN is named as a target body; no ACPIN-specific AI principles document was located. **Mitigation:** CSP principles apply to ACPIN members by affiliation; ACPIN functions as a contractor accreditation body, not a guidance authority for this build.

5. **Physiopedia team page (founder-credibility reference).** Brief named this; not retrieved in this pass. **Mitigation:** prior research captured Physiopedia PAI's product framing; the team-page reference pattern is liftable from iatroX patterns (4a, 4b) without Physiopedia-specific retrieval.

6. **Elicit's output hedging structure (table-level rather than meter-level).** Documented at the descriptive level from `competitive-landscape.md` but the specific table columns + hedging-cell language not deep-fetched. **Mitigation:** Consensus Meter (1d) and GRADE (1a) are richer reference patterns; Elicit's structured-extraction pattern is documented enough at descriptive altitude.

7. **The "verbatim four-row phrase ladder" for GRADE intervention wording** (improves / probably improves / may improve / very uncertain) was assembled from multiple GRADE sources rather than retrieved from a single canonical phrase-table document. The ladder is documented across the methodology literature but a single primary-source table at this level of compression was not located. **Mitigation:** the four-tier definitions (1a) plus Cochrane's "Authors' conclusions" worked example (1b) plus GRADE Handbook Table 2 give the same content in narrative form.

8. **Specific NICE NG128 (stroke rehabilitation) plain-language summary hedging.** Stroke-rehab is the Comp 6 domain; NG128 is the canonical NICE guideline. Its specific evidence-tier wording in plain language wasn't deep-fetched. **Mitigation:** Cochrane Langhorne 2018 [3] is stroke-rehab-domain and gives the verbatim hedging pattern; NICE NG128 specifically can be retrieved if `rules.md` ends up citing NG128 directly.

---

## Citations

1. **[web]** `https://book.gradepro.org/guideline/overview-of-the-grade-approach` — Neumann, Brennan, Meerpohl et al. "Overview of the GRADE approach" (GRADE Handbook, last updated 12 May 2026). Four certainty levels (high/moderate/low/very-low) with Table 2 verbatim definitions; five down-rating domains + three up-rating domains; SoF tables and EP framework; strength-of-recommendation distinction.

2. **[web]** `https://www.sciencedirect.com/science/article/pii/S2213398423002713` — Prasad M. "Introduction to the GRADE tool for rating certainty in evidence and recommendations" (Clinical Epidemiology and Global Health, Vol 25, Jan–Feb 2024). Open access. Names GRADE adoption by 110+ organisations including WHO, CDC, NHS, Cochrane, and UpToDate / DynaMed. Verbatim wording for high / moderate certainty levels.

3. **[web]** `https://www.cochranelibrary.com/cdsr/doi/10.1002/14651858.CD006187.pub3/` — Langhorne P et al. "Very early versus delayed mobilisation after stroke" (Cochrane Database of Systematic Reviews, 2018). Stroke-rehab-domain. Verbatim Authors' conclusions with hedging language; GRADE Working Group grades-of-evidence footnote with "We are very uncertain about the estimate" wording.

4. **[web]** `https://pedro.org.au/english/resources/pedro-scale/` — PEDro scale official page (Physiotherapy Evidence Database, University of Sydney, last amended 21 June 1999; database last updated 4 May 2026; 68,406 records). 11 items, 0-10 scoring (item 1 not scored). "Points are only awarded when a criterion is clearly satisfied" verbatim rule.

5. **[web]** `https://pmc.ncbi.nlm.nih.gov/articles/PMC7008740/` — Cashin & McAuley. "How to Classify Clinical Trials Using the PEDro Scale" (J Lasers Med Sci, 2020). "The PEDro scale assists readers to quickly assess whether a clinical trial presents reliable and meaningful results for use in clinical practice" verbatim.

6. **[web]** `https://help.consensus.app/en/articles/10069920-the-consensus-meter` — Allison Elechko (Consensus official help docs, last updated April 21, 2026). Verbatim Yes/No/Possibly/Mixed Consensus Meter definition; 5-20 paper analysis range; four quality indicators (Recency / Methods / Journals / Citations); ship-surface limits section verbatim.

7. **[web]** `https://effortlessacademic.com/consensus-ai-review-for-literature-reviews/` — Shabanov I. "Consensus AI: 2025 Review for Researchers" (Effortless Academic, last updated March 17, 2026). Independent review describing the four-bar output (Yes / No / Possibly / Mixed) and the prompt-shape requirements.

8. **[web]** `https://pmc.ncbi.nlm.nih.gov/articles/PMC2364804/` — Guyatt G, Oxman A, Kunz R, Vist G, Falck-Ytter Y, Schünemann H (GRADE Working Group). "What is 'quality of evidence' and why is it important to clinicians?" (BMJ 2008;336:995-998, doi:10.1136/bmj.39490.551019.BE). Canonical GRADE-in-BMJ paper. Verbatim four-level definition; quality-of-evidence-vs-strength-of-recommendation distinction; up/down-rating criteria.

9. **[web]** `https://www.gov.uk/government/publications/medical-devices-software-applications-apps` — MHRA "Medical devices: software applications" guidance (Medicines and Healthcare products Regulatory Agency, published 8 August 2014, last updated 1 July 2023). Primary PDF: "Medical device stand-alone software including apps" (43 pages). Appendices: symptom checkers / clinical calculators / "drives or influences the use of a device" / Field Safety Warnings.

10. **[web]** `https://www.medicept.com/mhra-standalone-software-and-apps/` — MEDIcept summary on MHRA standalone software requirements. UK MDR 2002 + UKCA marking requirement verbatim.

11. **[web]** `https://www.england.nhs.uk/long-read/guidance-on-the-use-of-ai-enabled-ambient-scribing-products-in-health-and-care-settings/` — NHS England "Guidance on the use of AI-enabled ambient scribing products in health and care settings" (published 27 April 2025, last updated 24 April 2026). Verbatim Generative AI risk framing; DCB0160/DCB0129 requirements; MHRA Class 1 registration minimum; verbatim qualification threshold for Generative AI summarisation as medical device.

12. **[web]** `https://www.fda.gov/medical-devices/software-medical-device-samd/artificial-intelligence-software-medical-device` — FDA "Artificial Intelligence in Software as a Medical Device" page. Verbatim AI / ML definitions; premarket pathways (510(k) / De Novo / PMA); AI/ML SaMD policy chronology Jan 2021 Action Plan → Jan 2025 Draft Guidance.

13. **[web]** `https://www.iatrox.com/blog/introducing-iatroX` — iatroX "introducing iatroX" blog post. Pre-MHRA-registration self-positioning: *"While it isn't yet a formal clinical decision support system, we are continuously evolving—actively exploring medical device classification..."*

14. **[web]** `https://www.iatrox.com/blog/clinical-ai-landscape-2026-chatgpt-openevidence-iatrox-medwise` — iatroX "The Clinical AI Landscape in 2026" (2026). Four-category clinical-AI taxonomy (General-Purpose / Clinician-Facing / AI Scribes / Enterprise); MHRA-registered Class I positioning verbatim; "Different tools for different moments in the same clinical workflow" framing.

15. **[web]** `https://www.csp.org.uk/news/2025-03-31-new-ai-physio-principles-provide-guideline-future` — CSP news "New AI in physio principles provide a 'guideline for the future'" (31 March 2025). Verbatim Sylvia Wojciechowski (CSP Council Chair) framing; 6-monthly review cadence over 2 years.

16. **[web]** `https://www.csp.org.uk/professional-clinical/professional-guidance/ai-use-physiotherapy` — CSP "Artificial Intelligence (AI) principles in action" professional guidance page. Verbatim Transparency principle; verbatim PLI / liability four-category framing; verbatim scope-of-practice statement; cross-reference to government medical-device regulation guidance + DTAC.

**Prior-research references (cited but not re-retrieved):**

- **iatrox.com 2026 (different article)** — research-tools-vs-clinical-tools safety distinction. `competitive-landscape.md § P1` ref [6]: *"Research tools are for exploring. Clinical tools are for deciding. Confusing them at the bedside is a patient safety risk."*
- **Scrivener et al. 2020** (Bobath SR) + **Pollock et al. 2014** (Bobath SR) — both captured in `schools-landscape.md` ref [1] + `competitive-landscape.md § P2 Friction B`. Worked examples of physio-SR hedging in stroke-rehab domain.
- **Mayston 2008** (Bobath as framework-not-treatment) — captured in `schools-landscape.md` ref [2]. Worked example of within-school nuanced hedging.

---

## Open questions surfaced

- **Q7 — NICE Evidence Standards Framework (ESF) primary document and tier definitions for digital health technologies.** CSP and NHS England cross-reference DTAC and the ESF, but the ESF primary document with its tier-definitions for AI clinical-AI-adjacent products was not located within the 12-call web-cap. Resolution: targeted single-query if `identity.md` or `rules.md` decides to position the build against an ESF tier.

- **Q8 — MHRA "Medical device stand-alone software including apps" PDF (43 pages, 1 July 2023).** GOV.UK landing page scraped; primary PDF not deep-retrieved. Resolution: dedicated firecrawl-scrape of the PDF URL if `identity.md` ends up making a specific MHRA-qualification claim.

- **Q9 — ACPIN-specific AI guidance.** No ACPIN-specific document located. Resolution: targeted search or accept CSP-by-affiliation as the operative authority.

- **Q10 — NICE NG128 (stroke rehabilitation) plain-language summary hedging.** Domain-specific NICE wording for the stroke-rehab context not deep-retrieved. Resolution: targeted single-query if `rules.md` ends up citing NG128 specifically.

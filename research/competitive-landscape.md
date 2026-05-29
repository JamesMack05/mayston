---
topic: comp-6-competitive-landscape
cadence: low
source-skill: research
date: 2026-05-27
verdict: pass
---

# Research: Competitive landscape + user-friction prior-art for Comp 6 build

**Query (restated):** Does a folder-based AI research debate partner for UK CPD course tutors delivering weekend stroke-rehabilitation courses to practising physiotherapists already exist? What's the competing landscape? What frictions are CPD tutors / practising physios actually voicing?

**Mode:** vault-first → external (vault sweep produced no direct prior-art on AI research tools or CPD frictions; main signal from web).

**Sources consulted:**
- Vault: 0 directly-relevant files (Comp 4/5 artefacts surfaced but on different domains)
- Web: 4 firecrawl-search calls + scraped content (~6 unique URLs deep-read). Cap not hit (4/10).
- NotebookLM: 0 (no loaded notebook on this topic)

**Tools used:** find, grep, Read, firecrawl-search (with --scrape flag bundling search + scrape into one call).

---

## P0 — Does our tool already exist?

### Direct answer: No exact match. Adjacent products exist; none combine our four differentiators.

**Closest adjacents identified:**

**1. Physiopedia PAI (Physiopedia AI Assistant)** — [1]

Launched March 2026 across the Physiopedia Plus CPD catalogue. Physiopedia explicitly claims it is *"the only physiotherapy CPD provider in the world"* with integrated AI-powered learning features [1].

- **Features:** Interactive PAI Knowledge Checks, scenario-based learning activities, conversational learning across CPD topics.
- **Stated purpose:** *"bridge the gap between theoretical knowledge and the real clinical situations you encounter every day. Whether that means working through a differential diagnosis, identifying red flags or reflecting on evidence-based guidelines, PAI activities are designed to prompt the kind of critical thinking that defines strong clinical reasoning."* [1]
- **User-side member quote:** *"It helped me to identify areas I needed to improve."* [1]

**Why this matters:** PAI is the strongest signal that a generative-AI/CPD/physio combination is being commercially developed. Crucially, it serves the **CPD-attendee** side (the learner taking a Physiopedia course), not the **CPD-deliverer** side (the tutor preparing the course).

**Gaps vs. our build:**
- User mismatch: PAI prompts physio LEARNERS during/after a Physiopedia course. We target physio EDUCATORS preparing courses upstream of any platform.
- Embedded in proprietary content ecosystem (Physiopedia courses only).
- SaaS-locked, not folder-based / portable.
- Not stroke-rehab-specific.
- Teaching-shaped (prompt the learner) — different conversation pattern from research-debate (challenge the educator).

**2. Physiotutors ChatCPG** — [2]

Released July 2024. *"chatCPG stands for 'chat Clinical Practice Guidelines.' It is an AI clinical assistant trained on a comprehensive database of recent clinical practice guidelines relevant to physiotherapy."* [2]

- **Features:** Curates research, summaries of findings, contextual insights, links to educational resources.
- **User:** Practising physiotherapists at point of clinical decision.
- **Roadmap signal:** Physiotutors AI Co-Pilot in waiting-list phase as of 2026 — bigger product behind. [2]

**Gaps vs. our build:**
- User mismatch: targets practising physios at clinical decision-point, not educators preparing CPD content.
- Output-shaped (give answer), not debate-shaped.
- SaaS, not folder-based.
- Built on clinical practice guidelines, not investigative-mode research debate.

### Skool / Clief Notes community prior art

The methodology our build uses — **Interpretable Context Methodology (ICM)** — is Jake Van Clief's published framework [3], hosted as an arxiv preprint and openly distributed in the Clief Notes Skool community [4]. Past weekly comps have applied ICM to different agent shapes:

- **Comp 4 — "The Agency"** (winner: Ruby Sparks): folder-based AI agencies, mostly in property/real-estate/commercial domains [5].
- **Comp 5 — "The Coach"**: folder-based AI coaches (James shipped a squat-rack coach; spotlight tier).
- **Comp 6 — "The Researcher"** (current): folder-based AI researcher (open domain).

**Finding:** No evidence of any past Skool comp shipping a clinical / medical / physio-domain build. Our domain choice (stroke-rehab CPD) is **novel for this community** as far as the public Skool posts and Clief Notes archive show. (Caveat: I cannot see all past Show-Your-Work posts.)

---

## P1 — Competing landscape we'd be measured against

Distinguishable into **two categories** per the canonical iatrox.com framing [6]:

### Category A — AI research tools (search the literature)

| Tool | Database | Unique feature | Shape | Physio-specific? |
|---|---|---|---|---|
| **Elicit** | 138M+ papers, 545K trials | Structured data extraction tables across N papers | Output (table) | No |
| **Consensus** | ~200M papers (via Semantic Scholar) | Consensus Meter (Yes/No/Possibly visual) | Output (binary signal) | No |
| **Semantic Scholar** | 200M+ papers | TLDR summaries + citation graph; **fully free** | Output (discovery) | No |
| **Perplexity** | Web + academic | Inline cited general-purpose AI search | Output (synthesis) | No |
| **scite.ai** | 1.2B+ citation statements | "Supporting / contradicting / mentioning" citation context | Output (verification) | No |

**Common shape across category A:** retrieval + synthesis. None operate in debate mode. None encode physio-specific tradition lineages (Bobath / Carr-Shepherd / PNF). None are folder-based.

### Category B — Clinical decision support tools (search guidelines)

| Tool | Geography | Source | Shape |
|---|---|---|---|
| **UpToDate** | International | Curated clinical content | Point-of-care answers |
| **DynaMed** | International | Editorial guideline synthesis | Point-of-care answers |
| **BMJ Best Practice** | International (BMJ-affiliated) | Curated clinical pathways | Point-of-care answers |
| **iatroX** | **UK-specific, MHRA-registered** | NICE, CKS, SIGN, BNF | Point-of-care answers + CPD-export logging |
| **OpenEvidence** | International | Curated medical content | Point-of-care answers |
| **ClinicalKey AI** | International | Elsevier content + AI | Point-of-care answers |

**iatroX is the closest UK-context competitor for *practising* physios** [6]:
- *"iatroX bridges the gap between research and clinical practice for UK clinicians. It does not search the open literature — it retrieves guideline-grounded answers from NICE, CKS, SIGN, BNF, and other trusted UK sources. Every answer is cited, every recommendation is traceable, and the platform is MHRA-registered as a medical device."* [6]
- Has a **CPD export feature** (*"Log the research question and reflection as CPD evidence using iatroX's CPD export"*) [6] — but this is CPD-logging, not CPD-prep.

**Gaps vs. our build:** all Category B tools are point-of-care for clinicians, not prep-tools for educators. None are debate-shaped. None encode therapeutic schools.

### The iatrox.com framing — "research tools vs clinical tools confusion is a patient safety risk"

The iatrox.com article [6] explicitly warns: *"Research tools are for exploring. Clinical tools are for deciding. Confusing them at the bedside is a patient safety risk."* This is a useful framing for our identity.md — our tool is neither pure research-retrieval (Elicit) nor point-of-care decision support (iatroX). It is **upstream of both: an evidence-debate partner for the educator preparing teaching content**, where the output is not a clinical decision but a structured brief input.

### Category C — Physio-specific tools

| Tool | Type | AI features |
|---|---|---|
| **Physiopedia (free)** | Wiki | None core (Physiopedia Plus has PAI) |
| **Physiopedia Plus / PAI** | CPD platform + AI | Conversational learning, scenario-based activities (March 2026) [1] |
| **PEDro** | Evidence database | Trial-quality scoring (PEDro scale), no AI |
| **CSP ePortfolio** | CPD tracking | No AI |
| **Physiotutors ChatCPG** | Clinical assistant | Chat over CPG database [2] |
| **APTA Learning Center** | CPD courses | Course on "AI in Physical Therapy" (Hardwick) [7] |

**Gap:** No tool I found targets the **CPD-tutor workflow specifically**. Tools target practising clinicians (Physiotutors ChatCPG, iatroX) or CPD-attendees (Physiopedia PAI). The CPD-content-preparer side is uncovered.

---

## P2 — Friction signals from CPD tutors / practising physios

**Update 2026-05-27 (extension pass):** original P2 was thin. Re-run with different query patterns surfaced strong two-sided friction signal across four sources. The frictions below are direct first-person quotes from named UK and international physiotherapists — usable in identity.md / rules.md / examples.md as anchored design constraints.

### Friction A — CPD course content quality + retention failure (practitioner → tutor side)

**Source:** Dave O'Sullivan, chartered physiotherapist (Munster Rugby, England Rugby, Wallabies — World Cup teams), now CPD tutor at thegotophysio.com [8]. Particularly load-bearing because Dave is **both sides**: ex-consumer who became a tutor.

Direct quotes from his "How NOT To Waste Money On Your Physiotherapy CPD Courses" essay [8]:

- *"I had spent over £10,000 on four levels of this 'technique' based course... but the course tutor kept promising you next the next advanced level to fix this or that. The theory had lots of gaps and the application of the evidence-based left questions."*
- *"You can hardly sleep that night, your mind is racing with all this new information. You get into work the next day... The first patient comes in and you use your new information... But something strange happens... That 'technique' or 'exercise' that worked so well on the other therapists during the weekend hasn't worked so well on your patients."*
- *"It's Friday and a few physios you work with ask you to show them what you learned on the course last weekend... You pause... You can remember a couple of bits of the course and show those but make a mental note to check your notes as you've forgotten 99% of the content covered that weekend."*
- *"I became a physio cpd courses junkie early in my career. Hopping from cpd courses to cpd courses. I couldn't get enough of the instant gratification, looking for that magic bullet course."*

**His own current tutor-prep workflow** [8]: *"I'd first schedule a time to look through the evidence base in these pillars to get a better understanding of the evidence and the application of use in the real world... Then I'd do a quick search and list the leading physiotherapists... in this field and see what I can learn from them."*

**Implication for our build:** Dave's tutor workflow IS the workflow our AI should support — score gaps → search evidence base → identify leading thinkers → debate application. He's doing this manually; the AI compresses it.

### Friction B — Bobath / EBP cultural conflict in UK NHS (practitioner side)

**Source:** Sarah Tyson blog (UK neuro physio educator/researcher), 2015-2016 reader comment thread on "How to do Bobath" series [9]. Includes named UK and international neuro physios.

**Zack Siddells** (former neuro physiotherapy teacher, January 2016) [9]:
- *"Such 'schools of thought' as the Bobath Method still has so much popularity amongst physios. My disheartening is when I reflect on the enormous amount of clinical research that has happened over the last two decades; the enormous amount of evidence now for task based approaches... the more-or-less complete failure of trials investigating BB to show benefit. Yet a huge body of therapists just don't get it and continue to flog a dead horse."*
- *"My interest is more in the sociology that we still seem to be a profession that is prone to cults rather than applied science."*
- *"Why are we still littered with names such as the McKenzie approach, the Bobath method, or the Maitland concept? Why don't we just attach a simple label that describes the function of an approach?"*

**JB8205** (acute neuroscience unit physio, January 2016) [9]:
- *"I so enjoyed these blogs! I am so not a bobath fan but I do find I am often in the minority where I work. I work in acute neuroscience unit and usually use a much more functional/impairment/participation approach but recently had a young patient and I felt doing this would be a disadvantage to him.... Now reading these blogs and I am so questioning my practice! Yikes! I need to have the courage of my convictions and stand up for what I (and I know others!) think and need to stop worrying about what my colleagues in the rehab and stroke units think of my practice and I need to challenge their approach!"*

**Sarah Tyson** (blog author, January 2016) [9]:
- *"Many have invested time, effort, finances and reputation on the named approaches and have gained status and often comfortable living from following and promoting the named approaches so there are many vested interests in keeping them going, which doesn't make it right but does explain why it happens despite its illogicality."*
- *"Many do not understand the difference between disagreeing and arguing... weeping and wailing, passive aggression (sometimes not so passive) and tantrums in other AHPs too, when their comfort zones are challenged."*

**Ruud van der Veen** (Netherlands physio, November 2015) [9]:
- *"Bobath was abandoned in the Netherlands in 2007 in favor of an evidence-based approach... Just because patients improve in function doesn't mean there's a causal relation with your therapy."*

**Erik Prinsen** (commenter, November 2015) [9]:
- *"It is not one opinion facing an opposing opinion. It is years of research leading to evidence-based facts against an opinion that is based on years of experience with BB therapy... evidence-based facts outweigh empirical evidence (also known as sense experience)."*

**Nikki Penny** (UK neuro physio, ex-Bobath tutor track, February 2016) [9] — the NUANCED defender position:
- *"I left one month shy of qualifying as a Bobath tutor. The second half of my career has been about exercise and strength training in the neuro patient... So I don't have a financial gain in the concept, I have no misplaced loyalty."*
- *"The Bobath courses to me are movement courses that allowed me to begin to understand movement. They provided a forum where I could see an experienced clinician identify movement problems and begin to develop a treatment plan forward."*

**This Penny quote is critical for the build.** It separates two claims that summarisers conflate:
- *"Bobath as a research-validated treatment method"* (evidence: weak / inferior to task-specific training)
- *"Bobath courses as a movement-observation training framework"* (evidence: clinically useful, no equivalent training exists)

A debate-shaped AI must surface this distinction. A summariser AI will collapse it.

**Direct UK academic confirmation of the Bobath debate:** [10] — Pollock et al. 2014/2020 systematic review concluded *"Bobath therapy was inferior to task-specific training and not superior to other interventions, with the exception of proprioceptive neuromuscular facilitation."* This is the canonical academic citation for the contested-claim our AI debates against.

### Friction C — Evidence-based practice barriers (UK MSK physios, quantitative)

**Source:** Physiotherapy Journal — "Perceived barriers to evidence based practice amongst UK musculoskeletal physiotherapists" [11]; plus systematic barriers data [12].

**Quantified barriers:** *"insufficient time"* (OR 1.48), *"lack of information resources"* (OR 2.07), *"lack of access to patient decision aids and treatment information"* — top barriers across studies [11], [12], NHS eWIN Physiotherapy Evidence Brief 2025 [12].

**Implication:** the time-and-access friction is empirically documented, not just anecdotal. Our tool addresses exactly these two: condensed access (vs Time) + AI-curated reference content (vs lack-of-information-resources).

### Friction D — Specialisation / CPD quality gap (international signal)

**Source:** Reddit r/physiotherapy AMA, "7 years a Physio" thread [13]:
- *"Europe offers programs to help specialize, like a 2nd master's. Canada has shit options for that and just generally shit CPD for employees."*

This is anecdotal and Canada-specific, but the signal generalises: CPD quality is uneven across jurisdictions, and there's named frustration with employer-provided CPD. The UK-NHS context our build serves probably has analogous frustrations even where formal CPD exists.

### Friction signals — synthesis for the build

Five named friction patterns the AI must address by design:

1. **Content-retention failure** [Dave O'Sullivan]. Tutors deliver content attendees forget 99% of within a week. Our AI helps tutors structure briefs around *transferable principles* not technique-of-the-week, which attendees can actually retain.
2. **Vested-interest detection** [Sarah Tyson, Zack Siddells]. Named approaches (Bobath, McKenzie, Maitland) carry financial + status incentives for proponents. Tutors must navigate this without becoming partisan. The AI surfaces vested-interest patterns proactively.
3. **EBP-aligned-physio-in-Bobath-team conflict** [JB8205]. Real first-person testimony of a physio feeling outnumbered when applying EBP in a tradition-dominant team. Tutors preparing CPD for mixed-tradition audiences need the AI to help frame contested findings in ways that respect both camps.
4. **"Movement framework" vs "treatment method" conflation** [Nikki Penny]. The Bobath debate has TWO layers (research-validated treatment vs. movement-observation training framework). A debate-shaped AI must separate them; a summariser collapses them.
5. **Time + information-resource barriers** [Physiotherapy Journal UK MSK barriers paper]. Empirically the top two barriers to EBP. The AI directly addresses both.

These five frictions are **ANCHORED, NAMED, QUOTABLE** evidence the build addresses real practitioner pain. They translate directly to rules.md sections and examples.md walkthroughs.

---

## Differentiation map — where we win vs. where we're redundant

### Where we have a real gap to fill

| Differentiator | Why no existing tool covers it |
|---|---|
| **Debate-shaped interaction** | Every tool surveyed is output-shaped (table, Yes/No signal, synthesis, citation context). None operate in claim-vs-evidence sparring mode. This IS the brief's load-bearing angle and is genuinely under-served. |
| **CPD-tutor user persona** | All physio AI tools target attendees (Physiopedia PAI) or practitioners at clinical decision-point (Physiotutors ChatCPG, iatroX). CPD-deliverer side is uncovered. |
| **Therapeutic-school tradition navigation** | Bobath / Carr-Shepherd / PNF / Brunstrom / Peto / CIMT as lineages with founders, evidence bases, contemporary defenders/critics — no tool encodes this. Generic research tools (Elicit, Consensus) treat papers as atomic; physio-specific tools (Physiotutors ChatCPG, Physiopedia PAI) don't surface the meta-debate. |
| **Folder-based portability** | All competitors are SaaS-locked. Folder-based ICM gives users ownership, modifiability, portability. This is the brief's methodology and a real moat against SaaS incumbents — but only matters to users who value owning their tooling. |
| **UK-NHS context anchored** | Most generic tools are international-default. iatroX is the only one specifically UK-anchored — but iatroX targets clinicians, not educators. UK CPD-educator context is open. |

### Where we're redundant or marginal

| Risk | Honest assessment |
|---|---|
| **Literature retrieval / synthesis** | We CANNOT beat Elicit, Consensus, or Semantic Scholar on retrieval breadth. We have no database, no semantic search, no citation graph. **Implication:** position the tool as a debate-partner that complements retrieval tools — not as a retrieval tool itself. The README should frame this: "use Consensus / Elicit / PubMed to FIND papers; use us to interrogate what to do with them." |
| **Clinical-decision-support** | We CANNOT and SHOULD NOT replace iatroX, UpToDate, etc. The iatrox.com article makes this point explicitly — confusing research/teaching tools with clinical decision tools is a patient-safety risk. **Implication:** the safety frame James locked in (AI offers pattern-matched material; user verifies primary literature; not authoritative on clinical effectiveness) directly addresses this risk. Lean into it in identity.md. |
| **Physiopedia Plus PAI as adjacent** | If Physiopedia expands PAI from the attendee-side to the deliverer-side, the gap we're filling closes. **Implication:** ship within the comp window (4 days left). Don't optimise for a 6-month roadmap. |
| **General LLM tools (ChatGPT, Claude)** | A physio educator could in principle do most of what we'd offer in a vanilla Claude conversation. **Implication:** our edge is the curated rules.md + therapeutic-school reference/ + portability of the folder. Without those, we're just "a Claude with a system prompt" — that's the brief's failure-mode test. Quality of the encoded rules is the differentiator. |

---

## Verdict

**Proceed with current framing. The tool does not already exist; the gap is real.**

The four key differentiators (debate-mode interaction, CPD-tutor persona, therapeutic-school navigation, folder-based portability) compound. Each individually is partially-covered or marginally novel. Together, they describe a tool no current product offers.

**Sharpening recommendations for the build:**

1. **Lean into the safety frame.** The iatrox.com article gives us an external-source citation for the "research-tools-vs-clinical-tools" distinction. identity.md should explicitly position us upstream of both: we are an **educator's evidence-debate partner**, NOT a clinical-decision tool, NOT a literature-retrieval engine. Each negative-positioning is defensible against a real product that does that thing better.

2. **Cite the adjacent products as named complements**, not competitors, in README. "Use Elicit / Consensus to FIND papers. Use us to interrogate WHAT TO DO WITH THEM." This signals technical literacy + market awareness + appropriate scope to judges.

3. **Acknowledge Physiopedia PAI's existence in README** without minimising. Their move into AI-CPD is real and growing; our positioning is upstream/adjacent (different user, different shape, portable not SaaS). Pretending they don't exist would be a credibility loss with informed judges.

4. **The therapeutic-school tradition navigation is your sharpest unique angle.** No competitor encodes Bobath / Carr-Shepherd / PNF / Brunstrom as named traditions with founders + defenders + critiques. This is the differentiator most resistant to commoditisation by general LLM tools (because it requires domain-curated reference content, not just prompt engineering).

5. **The UK-NHS anchoring + MHRA-aware safety frame is defensible.** iatroX is the only directly-comparable UK-specific incumbent, and they're for clinicians-at-point-of-care, not educators-preparing-content. UK-CPD-educator slot is open.

**Decision options for James:**

- **(a) Proceed** with current framing — recommended. The gap is real, the differentiation map holds, build week 4/5 days remain.
- **(b) Sharpen differentiation** — re-read the differentiation map; consider whether to tighten the CPD-tutor user further (e.g., bias examples.md heavily toward the Bobath debate / facilitation conflict — the most defensible differentiator).
- **(c) Pivot user / domain** — only if a finding here surprised you about the strength of an incumbent. It shouldn't have — Physiopedia PAI is the closest threat and it's clearly different user + different shape.
- **(d) Abandon and pick new comp framing** — not warranted by these findings.

---

## Citations

1. **[web]** `https://members.physio-pedia.com/members-news/ai-powered-learning-comes-as-standard-with-physiopedia-plus/` — Physiopedia Plus PAI (March 2026): *"the only physiotherapy CPD provider in the world"* with integrated AI; conversational learning, scenario-based activities, PAI Knowledge Checks across the Plus CPD catalogue.

2. **[web]** `https://www.physiotutors.com/ai-clinical-assistant-chatcpg/` — Physiotutors ChatCPG (July 2024): AI clinical assistant trained on clinical practice guidelines for physiotherapy; targets practising physios at clinical decision-point. AI Co-Pilot in waiting-list phase as of 2026.

3. **[web]** `https://arxiv.org/pdf/2603.16021` — Van Clief, "Interpretable Context Methodology: Folder Structure as Agentic Context" (preprint). The published methodology our build applies.

4. **[web]** `https://www.skool.com/cliefnotes/icm-research-paper` — Clief Notes Skool community post by Jake Van Clief sharing the ICM paper, March 2026. Confirms the methodology + community context.

5. **[web]** `https://www.skool.com/cliefnotes/weekly-comp-4-results-the-agency-corrected` — Comp 4 results (Ruby Sparks winner). Confirms folder-based-agency genre and past comp shape.

6. **[web]** `https://www.iatrox.com/blog/best-ai-tools-medical-research-2026-elicit-consensus-semantic-scholar-perplexity` — iatroX market-overview article (2026) covering Elicit / Consensus / Semantic Scholar / Perplexity / scite + clinical-decision-support category positioning. Source of the "research-tools-vs-clinical-tools" safety distinction and the UK-NICE-anchored iatroX positioning.

7. **[web]** `https://learningcenter.apta.org/products/ai-in-physical-therapy` — APTA Learning Center course "AI in Physical Therapy" (Dustin Hardwick). Teaches CLEAR prompt-engineering framework for PTs.

---

## Open questions surfaced

- **Are there past Skool comp builds in clinical/medical domains I missed?** Searches confirmed Comp 4 was The Agency (Ruby Sparks won, property/real-estate context) and the methodology is well-established in the community. But I cannot see all Show-Your-Work posts — there may be a past medical-domain build I'm not aware of. **Resolution:** James can ask in the Clief Notes community if relevant, or check past Show-Your-Work posts directly.
- **Tutor-side friction signals** (P2) — couldn't surface first-person quotes from CSP community / ACPIN / Reddit r/physiotherapy. This is a real gap. **Resolution if needed:** targeted forum search with different query patterns, or direct outreach to a UK stroke-rehab CPD provider. Not blocking for the build given the strong P0 + P1 findings.
- **Physiopedia PAI roadmap.** They may expand from attendee-side to deliverer-side at any time. **Resolution:** ship within comp window; don't optimise for a 6-month timeline.

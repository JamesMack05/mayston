---
topic: comp-6-schools-landscape
date: 2026-05-27
description: Research audit of named stroke-rehab therapeutic schools — founders, evidence stance, defenders, critics, and UK NHS uptake.
---

# Research: Therapeutic schools landscape for stroke rehabilitation

**Query (restated):** For each named stroke-rehab therapeutic school the build encodes (Bobath / Carr-Shepherd / PNF / Brunnstrom / Peto / CIMT), capture founder + origin + core claim + current evidence stance + contemporary defenders + contemporary critics + vested-interest signals + UK-NHS uptake. Output target: build `reference/schools/<n>.md` files dense enough to defend against judging criterion #2 (domain specificity) + #3 (source weighing / uncertainty flagging).

## Sources consulted

- Prior research: 2 files (competitive-landscape.md Friction B already captured rich Bobath debate quotes from Tyson/Siddells/JB8205/Penny/Prinsen/van der Veen + Pollock 2014 reference; user-profile-investigation.md Q11 supplied vested-interest example).
- Web: 5 search calls (Carr-Shepherd, PNF, Brunnstrom, Peto, CIMT). 6th search attempt (UK contemporary Bobath/ACPIN practice signals) blocked by a credit cap — non-blocking gap; the UK-named-clinician friction signals (Tyson/Siddells/Penny/JB8205) already cover UK contemporary practice testimony.

---

## The two fault lines

Before per-school detail, two structural distinctions the build's debate-mode behaviour must surface to avoid summariser collapse:

### Fault line 1 — Facilitation-based vs Task-oriented

This is the canonical contemporary debate. Generic LLMs and surface-level summarisers collapse it.

- **Facilitation-based (older, neurophysiological-theory-driven):** Bobath/NDT, PNF, Brunnstrom. Assume the therapist's manual handling, postural cues, and stimulus-driven movement elicitation are causally load-bearing for recovery. Theory roots in mid-20th-century reflex-hierarchical motor control models.
- **Task-oriented (newer, motor-learning-theory-driven):** Carr-Shepherd (Motor Relearning Programme), CIMT. Assume motor relearning is driven by task-specific, high-repetition, goal-directed practice. Theory roots in motor-learning research (Schmidt, Lee) and neuroplasticity literature emerging from the 1980s onward.
- **Hybrid / non-categorical:** Peto (Conductive Education) — task-series + rhythmical-intention + group-class structure; not cleanly in either camp.

**Current systematic-review verdict:** task-specific training produces moderately greater benefit on lower-limb activities than Bobath therapy (SMD 0.48, 95% CI 0.01 to 0.95) [1]. Bobath therapy was *not* clearly inferior to combined interventions or strength training, and was superior to PNF for standing balance in one trial [1]. So the literature does NOT say "facilitation doesn't work" — it says "task-specific training beats it where it's been directly compared." This nuance is the gold finding for the build's debate-mode behaviour (an earlier call captured this verbatim — *"What the evidence actually showed is that Bobath isn't any better than other approaches"* — `user-profile-investigation.md` § C).

### Fault line 2 — "Treatment method" vs "Movement-observation training framework"

The Penny quote already named this distinction [§P2 Friction B, Penny]. The contemporary UK Bobath community (Bobath Tutors UK, EBTA) explicitly defends Bobath as a *framework* that has given therapists a clinical-reasoning tool, separate from its evidence-base as a treatment intervention [2]. Margaret Mayston (UCL Senior Teaching Fellow + Senior Bobath Tutor) makes the explicit nuanced case: Bobath as "contributor to client-based neurorehabilitation, not the leading actor" [2]. A debate-mode AI must surface both layers (intervention-vs-framework); a summariser collapses to just one.

---

## Schools — per-school encoding

### 1. Bobath Concept / Neuro-Developmental Treatment (NDT)

- **Founders:** Dr Karel Bobath (medical doctor) + Berta Bobath (physiotherapist). Jewish refugees from Germany; relocated to UK in 1930s. Developed the approach from their London treatment centres starting 1940s; taught for ~50 years [2].
- **Geographic anchor:** UK-origin (London). Adopted in US as "Neuro-Developmental Treatment (NDT)" — name coined by Berta Bobath [2].
- **Core theoretical claim (original, 1940s–60s):** Recovery from CNS damage achievable via inhibition of abnormal tone + facilitation of normal movement patterns through manual handling. Therapist's hands guide patient's movement to elicit "normal" motor responses; abnormal synergies inhibited.
- **Core theoretical claim (contemporary, post-1990s revision):** Reframed as a problem-solving clinical-reasoning framework anchored on movement analysis + individualised goal-setting, not a fixed technique. Mayston 2008 [2] explicitly argues against treating Bobath as an "approach" and toward treating it as a contributor to client-centred neurorehab.
- **Current evidence stance:**
  - **Scrivener et al. 2020 (Australian J Physiotherapy, PROSPERO CRD42019112451)** [1]: systematic review + meta-analysis of 22 trials, 17 in meta-analyses. Bobath therapy *inferior* to task-specific training (SMD 0.48 for lower-limb activities, 95% CI 0.01 to 0.95). Not superior to combined interventions (SMD -0.06, 95% CI -0.73 to 0.61), strength training (SMD 0.35, 95% CI -0.37 to 1.08), or PNF (PNF inferior for standing balance in one trial only). Conclusion: *"Prioritising Bobath therapy over other interventions is not supported by current evidence."*
  - **Pollock et al. 2014** [§P2 Friction B]: same conclusion at the SR level — Bobath inferior to task-specific training, not superior to other interventions except PNF.
  - **Novak et al. 2013** [2]: cerebral-palsy-focused review, gave Bobath/NDT a "red light, don't do it" verdict that prompted EBTA's published rebuttal.
- **Contemporary defenders (UK):**
  - **Margaret Mayston** (UCL Senior Teaching Fellow, Senior Bobath Tutor) [2] — nuanced position: Bobath as framework, not as evidence-validated treatment.
  - **Gill Stern** (past President, European Bobath Tutors' Association / EBTA) [2] — formal institutional defender.
  - **Nikki Penny** (UK neuro physio, ex-Bobath tutor track) [§P2 Friction B] — declared no financial stake; defends Bobath courses as movement-observation training, not as treatment method.
  - **Bobath Tutors UK / European Bobath Tutors' Association (EBTA)** — institutional bodies maintaining UK course delivery.
- **Contemporary critics (UK + international):**
  - **Sarah Tyson** (UK neuro physio educator/researcher) [§P2 Friction B] — *"Many have invested time, effort, finances and reputation on the named approaches... vested interests in keeping them going."*
  - **Zack Siddells** (former UK neuro physiotherapy teacher) [§P2 Friction B] — *"Such 'schools of thought' as the Bobath Method still has so much popularity amongst physios... the more-or-less complete failure of trials investigating BB to show benefit. Yet a huge body of therapists just don't get it and continue to flog a dead horse."*
  - **JB8205** (UK acute neuroscience unit physio) [§P2 Friction B] — first-person testimony of EBP-aligned physio in Bobath-dominant team.
  - **Ruud van der Veen** (Netherlands physio) [§P2 Friction B] — *"Bobath was abandoned in the Netherlands in 2007 in favor of an evidence-based approach."*
  - **Erik Prinsen** [§P2 Friction B] — evidence-based-facts-vs-experience framing.
- **Vested-interest signal:** cuts both ways — defenders hold commercial course-delivery / credential stakes (Bobath Tutor status described as "a very lucrative place to be"); critics can hold their own non-commercial stakes (reputation, career investment in the competing evidence-based paradigm).
- **UK NHS uptake:** Still widely practised in UK NHS stroke units (JB8205's first-person evidence of being in the minority *as an EBP physio* implies Bobath-dominance is the local norm). EBTA + Bobath Tutors UK continue commercial course delivery; Bobath Centre London still operates.
- **Build file density verdict:** ✅ **HIGH.** Dense enough to drive a defensible `reference/schools/bobath.md` with the framework-vs-treatment distinction + UK named defenders + critics + vested-interest example + systematic review citations.

### 2. Carr & Shepherd / Motor Relearning Programme (MRP)

- **Founders:** Janet Carr + Roberta Shepherd, Australian physiotherapists. Approach developed late 1980s; canonical paper "A Motor Learning Model for Stroke Rehabilitation" published 1989 [3].
- **Geographic anchor:** Australia-origin (Sydney). UK NHS adoption widespread — physio.co.uk (UK private clinic chain) lists MRP as routine [4].
- **Core theoretical claim:** Stroke rehabilitation is a motor-relearning process driven by task-specific, goal-oriented practice. The brain is dynamic and capable of reorganisation following CNS injury (early neuroplasticity-aware framework). Treatment principles [4]:
  - Treatment is task-oriented (real ADLs — sit-to-stand, walking, reach, grasp).
  - Active patient participation; verbal + visual cues; cognitive engagement.
  - Use of affected side; discourage compensatory movement with unaffected side.
  - Prevent muscle shortening (spasticity precursor).
  - Treatment in stimulating, functional, context-specific environment.
  - Four steps: analyse essential task components → practise missing components → practise whole task → transfer to real environment.
  - Facilitation techniques de-emphasised; verbal instruction, demonstration, manual guidance emphasised [5].
- **Current evidence stance:**
  - **Scrivener et al. 2020** [1]: task-specific training (the MRP family) significantly outperforms Bobath therapy for lower-limb activities (SMD 0.48). This is the SR finding that MRP / task-oriented advocates cite.
  - **Alfaleh et al. 2025** [6]: prospective, multicentre RCT in Saudi Arabia (n=32 chronic stroke patients). MRP + conventional PT vs conventional PT alone; 18 sessions over 6 weeks. Large effect sizes (Cohen's d = 1.46 for Barthel Index; r = -0.865 for Motor Assessment Scale sit-to-stand). Conclusion: *"MRP significantly improves sit-to-stand transfer and ADL performance in chronic stroke patients."* Limitations: small sample, baseline MAS imbalance.
  - **Ghrouz et al. 2022** [7]: RCT protocol (n=66, sub-acute stroke). Three-month follow-up. Trial registered Oct 2021 (NCT05076383); results pending at search date.
- **Contemporary defenders:** Janet Carr + Roberta Shepherd themselves (still publishing into the 2010s — "Stroke Rehabilitation: Guidelines for Exercise and Training to Optimise Motor Skill" textbook). Task-oriented community broadly (most current motor-learning researchers).
- **Contemporary critics:** Less polarised than Bobath. Critique mostly methodological — Alfaleh 2025 small sample; older trials methodological quality varied (PEDro 2-8/10 per Scrivener) [1].
- **Vested-interest signal:** Low. MRP doesn't have the named-course-tutor commercial structure Bobath does; no equivalent of "Bobath Tutor" credentialing.
- **UK NHS uptake:** Implicitly endorsed by current EBP/task-specific guidance. NICE NG128 and RCP stroke guidelines align with task-specific principles.
- **Build file density verdict:** ✅ **HIGH.** Dense enough for `reference/schools/carr-shepherd.md` covering motor-learning theory anchor + MRP four-step method + Scrivener 2020 SR + Alfaleh 2025 RCT + the SR-comparative-stance against Bobath.

### 3. PNF (Proprioceptive Neuromuscular Facilitation) — Kabat / Knott / Voss

- **Founders:** Dr Herman Kabat (neurophysiologist + neurologist) + Margaret Knott (PT). Voss (Dorothy Voss) developed the technique further. Origin: late 1940s / 1950s, Kabat-Kaiser Institute (US).
- **Geographic anchor:** US-origin. Worldwide uptake. UK uptake substantial in private clinic / outpatient setting.
- **Core theoretical claim:** Motor function can be facilitated by stimulation of proprioceptors. Three-element approach [8]:
  - **Basic procedures:** resistance, irradiation, reinforcement, body mechanics, multimodal sensory stimuli (tactile-kinaesthetic / auditory / visual), traction + approximation, timing.
  - **Techniques:** rhythmic stabilisation, isotonic combinations, dynamic reversal, stretch, contract-relax, hold-relax.
  - **3D patterns** (the most distinctive element): diagonal-spiral movement patterns of scapula, pelvis, upper limbs, lower limbs, neck, trunk.
- **Current evidence stance:**
  - **Aggarwal et al. 2021** [9]: systematic review + meta-analysis. 17 RCTs, 656 subjects. PNF effective for **balance deficits** — Berg Balance Scale (Z=2.639, p=0.0083), Functional Reach (Z=3.2458, p=0.0012). PNF **not** effective for: Timed Up & Go, Trunk Impairment Scale, walking speed, Performance-Oriented Mobility Assessment. Conclusion: *"PNF intervention techniques may be effective for addressing balance deficit, but not sure for physical function recovery in the stroke population."*
  - **Scrivener et al. 2020** [1]: one trial in the Bobath SR compared PNF directly; PNF inferior to Bobath for standing balance (SMD -1.40, 95% CI -1.92 to -0.88). PNF + Bobath did not differ on any other outcomes.
  - **Hwangbo et al. 2017** [10]: SR protocol only; complete SR not located. Eligibility-restrictive — RCTs and quasi-RCTs in English/Spanish/French/Portuguese.
- **Contemporary defenders:** PNF-certification course infrastructure (similar to Bobath in tutor-commercial dynamic, though smaller). International PNF Association (IPNFA).
- **Contemporary critics:** Aggarwal 2021's mixed verdict is the strongest empirical critique. Not as politically contested as Bobath in the UK — quieter institutional position.
- **Vested-interest signal:** Moderate. IPNFA + Kaiser Permanente affiliation maintains commercial course delivery; less politically loaded than Bobath in UK NHS context.
- **UK NHS uptake:** Practised in NHS but not centrally guideline-recommended. Often combined with other approaches.
- **Build file density verdict:** ✅ **MODERATE-HIGH.** Dense enough for `reference/schools/pnf.md` covering Kabat-Knott-Voss origin + 3D pattern signature + Aggarwal 2021 mixed verdict (effective for balance, not for other functional outcomes) + Scrivener-comparative-stance.

### 4. Brunnstrom Movement Therapy

- **Founder:** Signe Brunnstrom, Swedish physical therapist. Approach developed 1960s, primarily in the US (Brunnstrom emigrated). Canonical reference: Brunnstrom's seven-stage motor recovery model [11].
- **Geographic anchor:** Sweden-origin / US-developed. Worldwide use of the Brunnstrom Stages framework even where the therapy itself isn't practised.
- **Core theoretical claim:** Recovery from stroke proceeds in reverse development — reflexes resurface first, then subcortical synergy patterns, then progress to voluntary, isolated movement. Treatment intentionally USES reflexes + associated reactions + proprioceptive/exteroceptive stimuli to elicit motion at early stages, then progressively de-emphasises them as voluntary control returns [11]. Seven-stage recovery sequence: (1) flaccidity → (2) synergy emerging → (3) synergy at peak/spasticity → (4) movement out of synergy → (5) complex movement combinations → (6) coordinated isolated joint movement → (7) normal motor function.
- **Current evidence stance:**
  - **Direct evidence of Brunnstrom Therapy as a treatment is sparse.** Physiopedia explicitly notes: *"There are several methods on rehabilitation of stroke patients however very little evidence is present"* [11]. The build's honest position must acknowledge this thin-evidence gap (the thin-evidence uncertainty flagging behaviour).
  - **The Brunnstrom Stages framework (separate from the therapy)** is widely used as a recovery-staging tool; Fugl-Meyer Assessment derives from this framework. Hsieh et al. 2016 [12] explored improving Brunnstrom-stage utility — confirms the staging framework persists even where the therapy doesn't.
  - **Comparison studies:** at least one direct comparison study of Brunnstrom vs MRP exists (Wang et al. 2011 [13]) — full text not retrieved within web-cap.
- **Contemporary defenders:** Limited institutional infrastructure compared with Bobath. Brunnstrom's textbook ("Movement Therapy in Hemiplegia") remains canonical reading.
- **Contemporary critics:** Theoretical objection — the reflex-hierarchical motor-control model the approach assumes is largely superseded by motor-learning + neuroplasticity-based theory. *"Using reflexes to facilitate voluntary movement"* is a 1960s neurophysiological framework, not a contemporary one.
- **Vested-interest signal:** Low. No active named-tutor commercial infrastructure equivalent to Bobath.
- **UK NHS uptake:** Brunnstrom Stages widely used as descriptive recovery staging; Brunnstrom Therapy as a treatment intervention rarely the named primary approach.
- **Build file density verdict:** ⚠️ **MODERATE.** The school is well-defined (founder + theory + stages) but the therapy-as-intervention evidence is thin. The honest `reference/schools/brunnstrom.md` file frames this explicitly — "framework still useful for staging, intervention has limited contemporary evidence base." This IS the source-weighing behaviour judging criterion #3 rewards.

### 5. Peto / Conductive Education (CE)

- **Founder:** András Pető, Hungarian physician. Approach developed in Hungary in the 1940s [14]. Originally for children with cerebral palsy; adult stroke / Parkinson's / MS applications later.
- **Geographic anchor:** Hungary-origin (Pető Institute, Budapest). UK uptake centred on the **National Institute of Conductive Education (NICE) in Birmingham** [14] — load-bearing UK anchor for the build's geographic frame.
- **Core theoretical claim:** Rehabilitation is a learning process, not a medical treatment. Programmes use a "task series" structure: functional tasks broken into components, practised repeatedly + rhythmically with verbal reinforcement ("rhythmical intention") in a specific order [14]. Group-class delivery is structurally part of the approach (vs Bobath's 1:1 manual handling).
- **Current evidence stance:**
  - **Charlesworth et al. 2016** [14]: single-blinded RCT **feasibility** study at NICE Birmingham. n=77 (37 intervention + 33 waiting period). Intervention = 10 weekly 1.5-hour CE sessions. Outcome measures: Barthel Index, Stroke Impact Scale, TUG, HADS. Result: feasibility confirmed; *"A definitive trial is feasible"* — but the **definitive trial has not yet been conducted as of search date**. The build's honest position is that CE has no definitive RCT evidence in adult stroke as of 2026.
  - **Three small pre/post studies** [14, refs 12-14 therein] — show promise in motor performance, ADL, QoL, but no control groups → specific effects of CE not demonstrated.
  - **Caregivers report decreased burden** [14, ref 15 therein].
- **Contemporary defenders:** NICE Birmingham; European Conductive Association [15]; Pető Institute Budapest.
- **Contemporary critics:** Mainly the absence-of-evidence position — without a definitive RCT, CE remains exploratory for adult stroke. No strong politicised critique equivalent to Bobath.
- **Vested-interest signal:** Low in commercial / political terms; high in institutional terms (NICE Birmingham is a dedicated facility — institutional preservation incentive).
- **UK NHS uptake:** Available but not centrally guideline-recommended. NICE Birmingham operates as an independent facility; NHS referrals possible but not routine.
- **Build file density verdict:** ⚠️ **MODERATE.** The school is well-defined and has a clean UK institutional anchor (Birmingham), but evidence base is feasibility-stage only. Defensible `reference/schools/peto.md` written as: school exists, has UK institutional presence, feasibility RCT done 2016, definitive RCT pending. This is judging criterion #3 behaviour — honest about uncertainty.

### 6. Constraint-Induced Movement Therapy (CIMT)

- **Founder:** Edward Taub (psychologist + neuroscientist, University of Alabama at Birmingham). Original mechanism research 1960s-80s on deafferented primates ("learned non-use" concept). Translation to stroke human upper-extremity rehab from late 1980s onward.
- **Geographic anchor:** US-origin (UAB). Worldwide uptake. UK NHS adoption variable — eligibility-restrictive (see below).
- **Core theoretical claim:** Stroke patients develop "learned non-use" of the impaired upper extremity — the brain learns to ignore the limb after initial paralysis even when motor capability partially returns. CIMT counteracts this by:
  - **Restraining the unaffected limb** (padded safety mitt worn ~90% of waking hours) for 2 weeks.
  - **Massed practice** with the affected limb — 6 hours/day of behavioural shaping + repetitive task practice from a library of ~60 graded tasks.
  - **Behavioural transfer package** — strategies to transfer gains to home/community use.
- **Current evidence stance:**
  - **Wolf et al. 2006 (EXCITE trial, JAMA)** [16]: multisite RCT, n=222 patients 3-9 months post-stroke. CIMT vs usual-and-customary care. Statistically significant improvements on **all primary outcomes**: WMFT Performance Time (mean time 19.3s → 9.3s vs 24.0s → 17.7s, between-group difference 34%, p<.001); MAL Amount of Use (1.21 → 2.13 vs 1.15 → 1.65, p<.001); MAL Quality of Movement (1.26 → 2.23 vs 1.18 → 1.66, p<.001); SIS Hand domain (decrease 19.5 vs 10.1, p=.05). EXCITE was the **first multisite RCT of a non-surgical/non-pharmacological intervention** in this stroke population.
  - **Wolf et al. 2010 (EXCITE follow-up)** [17]: early (3-9 months) vs delayed (15-21 months) CIMT comparison. Both groups improved significantly. Early group greater improvement at 12 months on WMFT Performance Time, MAL, SIS Hand + Activities. By 24 months: no statistically significant difference between groups. **Implication:** CIMT works at both timepoints in this eligibility window.
  - **Eligibility window matters (load-bearing constraint):** CIMT requires initiation of active extension of wrist and fingers — patients with very severe motor impairment (no active wrist/finger movement) do not meet eligibility criteria. This is the practical NHS-resource constraint.
- **Contemporary defenders:** Taub's lab at UAB; widespread motor-learning-research community; included in international stroke rehab guidelines for eligible patients.
- **Contemporary critics:** Practical-implementation critics — 6 hours/day for 2 weeks is high-resource and not feasible in standard NHS outpatient delivery (forced clinic attendance, supervision, mitt compliance). Modified-CIMT protocols (mCIMT, lower intensity over longer duration) have emerged to address this.
- **Vested-interest signal:** Lower than Bobath. UAB licensing of training exists; not as politically contested in UK debate.
- **UK NHS uptake:** Variable. Eligibility criteria + 6-hr/day resource demand limit routine NHS delivery; mCIMT more practical but evidence base for mCIMT separate.
- **Build file density verdict:** ✅ **HIGH.** Dense enough for `reference/schools/cimt.md` covering Taub origin + learned non-use mechanism + EXCITE 2006 primary trial + EXCITE 2010 follow-up + eligibility-window constraint + practical NHS-delivery barrier.

### Side-note: Johnston approach

Dad's call (Q8) named **Johnston** alongside Bobath/PNF/Brunnstrom/Peto/Carr-Shepherd/CIMT. This is most likely **Margaret Johnstone's approach** (Scottish PT, splinting + pressure-air-splints for stroke + brain injury rehab, 1970s-80s). Not retrieved within web-cap; flagged as a possible 7th school but lower-priority than the six covered.

---

## Synthesis — implications for the build

### For `reference/schools/` folder structure

All six schools have enough density to drive a defensible file. Suggested per-file shape (derivable from each school's section above):

```
reference/schools/<school>.md
├── # <School name>
├── ## Founder + origin
├── ## Core theoretical claim
├── ## Evidence stance (current, with SR/RCT citations)
├── ## Contemporary defenders (named UK where possible)
├── ## Contemporary critics (named, with quotes where possible)
├── ## Vested-interest signal
├── ## UK NHS uptake
└── ## Build's debate-mode handling
```

### For `rules.md` — schools-aware debate behaviour

The five-friction-pattern + two-fault-line structure above translates directly to rules:

1. **Rule — separate framework-vs-treatment claims.** When debating Bobath specifically: surface the Mayston/Penny nuanced position. Don't collapse "Bobath as movement-observation training" with "Bobath as evidence-validated treatment intervention."
2. **Rule — surface fault-line 1 explicitly.** When the tutor brings a contested claim about any of the six schools, name which fault line it sits on (facilitation-based vs task-oriented vs hybrid) before debating particulars.
3. **Rule — flag thin-evidence schools explicitly.** Brunnstrom Therapy and Peto/CE have thin direct evidence. The AI must hedge explicitly when the contractor asks about these — *"This school has [feasibility-stage / very-little-direct] evidence; here's what we know vs don't know."*
4. **Rule — surface vested-interest patterns proactively.** When debating Bobath specifically, the vested interest cuts both ways (defender commercial stakes; critic reputational / career stakes); the AI can mention vested-interest dynamics where the tutor's planned audience may have financial/status stakes.
5. **Rule — UK-anchor sources where named.** ACPIN, Bobath Tutors UK, EBTA, NICE Birmingham, NICE NG128, RCP stroke guidelines, PEDro — these are the canonical UK touchpoints.

### For `identity.md` — clinical-safety frame

The build's positioning (the clinical-safety frame locked earlier) is **reinforced** by this research: the systematic reviews (Scrivener 2020, Pollock 2014, Aggarwal 2021) consistently warn against confident over-claiming; even the EBTA defenders frame Bobath as "framework not intervention." The AI offers pattern-matched material; the tutor verifies primary literature; the AI never claims authority on clinical effectiveness.

### For `examples.md` — vivid demo content

The Bobath debate (with Pollock 2014 + Scrivener 2020 + Penny/Tyson/Siddells named-clinician quotes) is the sharpest worked-example available. This is the build's primary differentiator. examples.md should bias toward Bobath-vs-task-specific worked dialogue rather than diluting across all six schools.

---

## Coverage matrix — schools × judging criteria

| School | Crit #2 (domain specificity) | Crit #3 (source weighing / uncertainty) |
|---|---|---|
| Bobath / NDT | ✅ Dense — UK named defenders + critics + vested interest + framework-vs-treatment | ✅ Dense — Pollock 2014 + Scrivener 2020 SR + named systematic reviews + EBTA rebuttal of Novak 2013 |
| Carr-Shepherd / MRP | ✅ Dense — task-oriented theory + 4-step method + UK clinical adoption | ✅ Dense — Scrivener 2020 SR + Alfaleh 2025 RCT (with limitations explicit) |
| PNF | ✅ Dense — Kabat/Knott/Voss + 3D patterns + procedures + techniques | ✅ Dense — Aggarwal 2021 meta-analysis (mixed: balance yes, other functional no) |
| Brunnstrom | ⚠️ Moderate — well-defined school but thin contemporary intervention literature | ✅ Dense in honesty — explicit thin-evidence flagging IS the source-weighing |
| Peto / CE | ⚠️ Moderate — well-defined school with UK Birmingham anchor | ✅ Dense in honesty — Charlesworth 2016 feasibility + no definitive RCT explicit |
| CIMT | ✅ Dense — Taub origin + EXCITE trial + eligibility constraint | ✅ Dense — EXCITE 2006 primary + 2010 follow-up + mCIMT critique |

**All 6 schools clear the threshold for a defensible build file.** Brunnstrom and Peto are explicitly honest about their evidence gaps — that honesty is the source-weighing behaviour the brief rewards, not a deficiency.

---

## Verdict

**PASS.** All 6 named schools have enough density for `reference/schools/<n>.md` files that defend against judging criterion #2 (domain specificity) and #3 (source weighing / uncertainty flagging). The fault-line structure (facilitation-vs-task-oriented + treatment-vs-framework) gives the AI a debate-mode navigation tool no general LLM has at the same anchored density.

The per-school stances translate into specific debatable claims (e.g. "should we use CIMT in NHS-resourced settings given the 6-hr/day requirement?"; "is facilitation real?"; "Bobath as framework — when is that defensible?"). Many candidate debates already surfaced inline above.

---

## Open questions surfaced

- **Q1 — Johnston approach (Margaret Johnstone, Scottish PT, splinting-based stroke rehab).** Dad's call mentioned Johnston as a 7th school; not retrieved within web-cap. **Resolution:** if a need for a 7th school surfaces, do a focused single-query search (lower priority than other work).
- **Q2 — Modified CIMT (mCIMT) evidence base.** Touched but not unpacked. **Resolution:** if rules.md or examples.md surfaces a need for the "CIMT in NHS-resourced settings" debate, retrieve mCIMT systematic reviews.
- **Q3 — UK contemporary Bobath/ACPIN/Bobath Tutors UK course delivery and current commercial scale.** Sixth search blocked by firecrawl credit cap. **Resolution:** the UK-named-clinician friction signals (Tyson/Siddells/Penny/JB8205) already give us the contemporary UK testimony; the commercial-scale gap is non-blocking for the build but could sharpen the vested-interest claim in `reference/schools/bobath.md` if needed.

---

## Citations

1. **[web]** `https://www.sciencedirect.com/science/article/pii/S183695532030103X` — **Scrivener et al. 2020** (Australian J Physiotherapy, PROSPERO CRD42019112451). Systematic review + meta-analysis: 22 trials, 17 in meta-analyses. Bobath therapy inferior to task-specific training (SMD 0.48, 95% CI 0.01 to 0.95); not superior to combined interventions, strength training, or (except for standing balance in one trial) PNF. Conclusion: *"Prioritising Bobath therapy over other interventions is not supported by current evidence."*
2. **[web]** `https://www.bobathtutors.com/concept.php` — Bobath Tutors UK / European Bobath Tutors' Association (EBTA) Concept page. Karel + Berta Bobath origin (1940s, London, refugees from Germany); NDT name coined by Berta Bobath for US transfer; Mayston 2008 "framework not approach" position; EBTA rebuttal of Novak et al. 2013 "red light don't do it" verdict.
3. **[web]** `https://www.sciencedirect.com/science/article/pii/S0031940610625886` — Carr JH 1989 "A Motor Learning Model for Stroke Rehabilitation." Canonical paper establishing the MRP framework.
4. **[web]** `https://www.physio.co.uk/treatments/neurological-rehabilitation/carr-and-shepherd.php` — UK private clinic chain page summarising Carr-Shepherd principles (task-oriented; verbal/visual prompts; discourage compensatory movement; prevent muscle shortening; active participation; functional environment).
5. **[web, derived from 4]** Carr & Shepherd principles synthesis from physio.co.uk + Ghrouz protocol [7].
6. **[web]** `https://pmc.ncbi.nlm.nih.gov/articles/PMC12711097/` — Alfaleh et al. 2025 (J Comparative Effectiveness Research). Prospective single-blinded multicentre RCT (Saudi Arabia, n=32 chronic stroke). MRP + conventional PT vs conventional PT alone, 18 sessions over 6 weeks. Large effect sizes on Barthel Index (Cohen's d=1.46) + Motor Assessment Scale sit-to-stand (r=-0.865). NCT06690073.
7. **[web]** `https://pmc.ncbi.nlm.nih.gov/articles/PMC8921790/` — Ghrouz et al. 2022 (Eur Stroke J). RCT protocol for MRP vs conventional PT (n=66, sub-acute stroke). NCT05076383; results pending at search date.
8. **[web]** `https://www.physio-pedia.com/Proprioceptive_Neuromuscular_Facilitation` — Physiopedia PNF page. Kabat + Knott origin; basic procedures (resistance, irradiation, reinforcement, body mechanics, sensory stimuli, traction + approximation, timing); techniques (rhythmic stabilisation, isotonic combinations, dynamic reversal, contract-relax, hold-relax); 3D diagonal patterns.
9. **[web]** `https://world.physio/congress-proceeding/meta-analysis-and-systematic-review-effectiveness-proprioceptive-neuromuscular` — Aggarwal et al. 2021 (World Physio Congress proceedings). Systematic review + meta-analysis: 17 RCTs, n=656. PNF significantly effective for Berg Balance Scale (Z=2.639, p=0.0083), Functional Reach (Z=3.2458, p=0.0012); not effective for TUG, Trunk Impairment Scale, walking speed, POMA. Conclusion: *"may be effective for balance deficit, but not sure for physical function recovery."*
10. **[web]** `https://pmc.ncbi.nlm.nih.gov/articles/PMC5728303/` — Hwangbo et al. 2017 (BMJ Open). SR protocol; PROSPERO CRD42016039135. *"First systematic review focused on the proprioceptive neuromuscular facilitation (PNF) approach for stroke survivors."* English/Spanish/French/Portuguese language restriction.
11. **[web]** `https://www.physio-pedia.com/Brunnstrom_Movement_Therapy` — Physiopedia Brunnstrom page. Signe Brunnstrom (Swedish PT, 1960s); reflex-hierarchical motor control theory; recovery proceeds in reverse from reflexes → synergies → voluntary control; seven-stage recovery sequence; *"very little evidence is present"* explicit statement.
12. **[web]** `https://pmc.ncbi.nlm.nih.gov/articles/PMC4979857/` — Hsieh et al. 2016 (Disabil Rehabil). "Improving the utility of the Brunnstrom recovery stages." Brunnstrom-stages framework persistence even where the therapy isn't used.
13. **[web]** `https://www.sciencedirect.com/science/article/abs/pii/S1360859211001653` — Wang et al. 2011 comparison study of Brunnstrom movement therapy vs Motor Relearning Programme. Full-text not retrieved within web-cap; flagged as a debates research target if needed.
14. **[web]** `https://pmc.ncbi.nlm.nih.gov/articles/PMC4935920/` — Charlesworth et al. 2016 (Stroke Research and Treatment, Hindawi). Conductive Education feasibility RCT at National Institute of Conductive Education, Birmingham UK. n=77 (37 intervention + 33 waiting period). CE = 10 weekly 1.5hr sessions; outcomes Barthel + SIS + TUG + HADS. Feasibility confirmed; definitive RCT pending. ISRCTN84064492. *"no randomised trials of CE for stroke"* at study design date.
15. **[web]** `https://european-conductive-association.org/wp-content/uploads/2019/11/Grundtvig_Handbook.pdf` — European Conductive Association handbook (institutional defender).
16. **[web]** `https://jamanetwork.com/journals/jama/fullarticle/203876` and `https://pubmed.ncbi.nlm.nih.gov/17077374/` — Wolf et al. 2006 (JAMA). EXCITE trial. Multisite RCT, n=222 patients 3-9 months post-stroke. CIMT vs usual-and-customary care over 2 weeks. WMFT Performance Time 34% between-group improvement (p<.001); MAL Amount of Use +0.43 (p<.001); MAL Quality of Movement +0.48 (p<.001); SIS Hand 9.42 difference (p=.05). NCT00057018. First multisite RCT of a non-surgical/non-pharmacological intervention in stroke.
17. **[web]** `https://pmc.ncbi.nlm.nih.gov/articles/PMC2954658/` — EXCITE follow-up (Wolf et al. 2010, Stroke). Early (3-9 months, n=106) vs delayed (15-21 months, n=86) CIMT comparison. Both groups improved significantly. Early group greater improvement at 12 months. By 24 months: no statistically significant difference. CIMT effective at both timepoints in eligibility window.

**Prior-research references (cited but not re-retrieved):**

- **Pollock et al. 2014** systematic review — referenced in `competitive-landscape.md § P2 Friction B` (canonical Bobath SR predating Scrivener 2020 with same conclusion).
- **Tyson / Siddells / JB8205 / Penny / Prinsen / van der Veen** — first-person UK + Netherlands neuro physio testimony already captured in `competitive-landscape.md § P2 Friction B`.
- **iatrox.com 2026** — research-tools-vs-clinical-tools safety distinction; `competitive-landscape.md § P1` ref [6].
- **Dad's call** — facilitation evidence-vs-experience conflict; `user-profile-investigation.md` § D.

# Reasoning-integrity catalogue

The bounded error set Mayston tests arguments against (operationalised by `rules.md` RULE-11). This is **domain-relevant**, not a philosophy-101 taxonomy — only the errors that actually show up in stroke-rehab evidence debates. Like every reference file, `rules.md` **cites this, it does not restate it**.

The catalogue is the engine under two behaviours: it sharpens RULE-04 pushback rehearsal (spot the hole in the challenge the educator will face), and it feeds RULE-12 argument drafting (knowing *why* the opposing argument is weak is what makes a drafted rebuttal land).

---

## The guardrail gate (read before using any entry)

In a contested-epistemology clinical field, a naive "detect fallacies" reflex destroys the exact nuance the build exists to protect (`identity.md` IDENT-03). **Before naming any error, run the gate:**

> *Is this a reasoning error, or a legitimate contested position?* If it is a legitimate position, name it **as a position and its evidence tier**, not as a fallacy. If it is genuinely blurry, **surface the tension and hold both layers open** (IDENT-03) — do not declare a verdict.

Four things look like fallacies but are **not**, and must **never** be labelled as such:

1. **Clinical experience** is not an appeal-to-anecdote fallacy — it is a legitimate *lower-tier* form of evidence in a contested field.
2. **Mechanism plausibility** is not a fallacy even when unproven — flag it as unevidenced (RULE-05/08); do not call reaching for it a logical error.
3. **Framework-unfalsifiability** is not special pleading — "systematic reviews test interventions, not frameworks" is a genuine epistemic state, not an ad-hoc exemption.
4. **Source-grounding** is not an appeal to authority — *grounding* a claim in a named, verifiable source (RULE-08) is the build's discipline; only *foreclosing* debate with "an authority said so" is the fallacy.

**Tone is never preachy.** An error is surfaced as something the educator can *use* (the hole in the challenge they will face) or *guard against* (don't walk in carrying this hole) — never as a scolding. Each entry below carries three fields: **(a)** the error, **(b)** a stroke-rehab worked example, **(c)** the legitimate-position counterpart that looks similar but must not be mislabelled.

---

## Bucket 1 — Statistical / evidence-reasoning errors

### 1.1 — Single-trial quality vs body-of-evidence certainty (PEDro vs GRADE)
- **(a) Error:** treating a high PEDro score on one trial as if it raises the GRADE certainty of the whole body of evidence. Two different axes: PEDro rates the methodological quality of a single RCT (items 2–11, 0–10); GRADE rates certainty across a body of trials.
- **(b) Example:** "the trials behind the SR scored well on PEDro, so the conclusion binds harder." Scrivener's included trials span **PEDro 2–8/10** — a 10/10 PEDro trial can still sit inside a moderate- or low-quality evidence base once heterogeneity and imprecision are accounted for.
- **(c) Counterpart (not an error):** citing a PEDro score to describe *one trial's* internal validity — that is exactly what PEDro is for. The error is only the cross-axis leap from single-trial quality to body-of-evidence certainty.
- *Extends RULE-05; cite `reference/schools/bobath.md § Evidence stance` (PEDro 2–8/10 range) + `reference/retrieval-routing.md` (PEDro entry).*

### 1.2 — Indirectness / over-generalising beyond population or setting
- **(a) Error:** applying a trial's effect to a population or setting it did not study, as if directly transferable.
- **(b) Example:** citing EXCITE's **6 hours/day × 2-week** CIMT protocol as evidence for what a standard NHS outpatient service can deliver — the trial intensity and population differ from NHS outpatient reality.
- **(c) Counterpart:** noting a finding *may* transfer, hedged and flagged as indirect — legitimate, and the honest move.
- *Ties to RULE-05 (downgrade for indirectness); cite `reference/schools/cimt.md` + `reference/debates/cimt-nhs-resource.md`.*

### 1.3 — Relative-vs-absolute effect / effect-size inflation
- **(a) Error:** quoting a large relative percentage with no absolute change and no confidence interval.
- **(b) Example:** "EXCITE showed a ~34% improvement on the WMFT" stated bare. The honest version pairs the relative figure with the absolute change (MAL Amount of Use 1.21→2.13 vs control 1.15→1.65) and the interval.
- **(c) Counterpart:** quoting the effect *with* its CI — e.g. Scrivener's SMD 0.48 (95% CI 0.01 to 0.95) — per RULE-08. Legitimate.
- *Cite `reference/schools/cimt.md` (EXCITE / Wolf 2006 figures); RULE-08.*

### 1.4 — Correlation/causation + confounding
- **(a) Error:** crediting the named approach for an improvement when practice intensity, spontaneous recovery, or attention could equally explain it.
- **(b) Example:** attributing recovery to facilitation handling when Kwakkel & Veerbeek 2015 attribute CIMT gains "mainly to adaptation by learning to optimize the use of intact end-effectors" — compensation-strategy learning, not the claimed neural mechanism. The whole facilitation-as-mechanism debate is this confound.
- **(c) Counterpart:** naming a plausible-but-unproven mechanism *and flagging it as unevidenced* (RULE-05/08) — not a logical error. Mechanism plausibility is not a fallacy.
- *Cite `reference/debates/facilitation-as-mechanism.md § Against`/`§ Evidence` + `reference/schools/cimt.md` (Kwakkel & Veerbeek 2015).*

### 1.5 — Confidence exceeding the evidence tier
- **(a) Error:** asserting a low- or very-low-quality claim as settled fact.
- **(b) Example:** stating "facilitation works" or "Bobath-as-framework is validated" as established, when the mechanism claim and the framework claim both sit at **very low quality** as empirical claims.
- **(c) Counterpart:** holding a low-tier claim explicitly *as* a low-tier claim — legitimate, and exactly what RULE-05 requires.
- *Ties to RULE-05; cite `reference/debates/bobath-method-vs-framework.md § Evidence` (the framework claim is theoretical, not empirical).*

### 1.6 — Cherry-picking / suppressing the counter-trial
- **(a) Error:** citing the systematic-review consensus while hiding the trial that cuts the other way.
- **(b) Example:** leaning on Scrivener/Pollock ("Bobath inferior to task-specific training") while omitting that, within Kollen 2009, a Wang orthopedic-vs-Bobath trial *favoured* Bobath on MAS/SIS, and Pollock found Bobath superior to PNF for standing balance.
- **(c) Counterpart:** direction-of-effect honesty — naming the counter-trial yourself before the room does (RULE-08). Legitimate and required.
- *Extends RULE-08; cite `reference/schools/bobath.md § Evidence stance` (Kollen / Wang / Platz / Thaut).*

### 1.7 — Surrogate vs clinical endpoint
- **(a) Error:** reading an improvement on a measurement scale as functional recovery.
- **(b) Example:** a points gain on the MAS (Modified Ashworth — a tone measure) or the SIS/MAL read as "the patient recovered function" — impairment- or activity-scale movement is not the same as real-world functional recovery.
- **(c) Counterpart:** reporting the scale result *as* a scale result, distinguishing what the measure actually captures — legitimate.
- *Cite `reference/schools/cimt.md` (WMFT / MAL / SIS outcomes) + `reference/schools/bobath.md` (MAS/SIS).*

### 1.8 — Base-rate / eligibility-window neglect
- **(a) Error:** presenting a result as broadly applicable while ignoring the narrow window the evidence was generated in.
- **(b) Example:** recommending CIMT team-wide without flagging that only about **10% (range 3–90%)** of initially screened patients met the wrist/finger-extension eligibility criteria.
- **(c) Counterpart:** stating the effect *and* its eligibility constraint together — legitimate.
- *Cite `reference/schools/cimt.md` (eligibility window) + `reference/debates/cimt-nhs-resource.md`.*

---

## Bucket 2 — Logical / rhetorical errors

### 2.1 — False dichotomy
- **(a) Error:** forcing two positions as mutually exclusive when they are not.
- **(b) Example:** "either we teach named-approach eclecticism or we abandon individualisation." Much of the apparent guideline-level disagreement is a false dichotomy: intervention-level personalisation (RTT + strength + CIMT-when-eligible + adjuncts) and named-approach switching look similar in practice but are distinct positions.
- **(c) Counterpart:** a genuine either/or where the evidence really does force a choice — not every binary is false.
- *Cite `reference/debates/task-specific-vs-eclectic.md § Evidence` (the explicit "false dichotomy at the guideline level").*

### 2.2 — Straw man
- **(a) Error:** refuting a weaker misrepresentation of the opposing position rather than the position actually held.
- **(b) Example:** knocking down "Bobath claims it beats every other method" when the position actually defended is the movement-observation/clinical-reasoning *framework* claim — a different object that the intervention evidence does not touch.
- **(c) Counterpart:** debating the educator's *captured* position (RULE-02), stated in its strongest form (RULE-04) — the build's anti-strawman discipline.
- *Cite RULE-02 + RULE-04; `reference/debates/bobath-method-vs-framework.md` (the two-object distinction).*

### 2.3 — Red herring
- **(a) Error:** shifting to an irrelevant point to dodge the claim on the table.
- **(b) Example:** answering "what is the SR evidence for Bobath?" with "the Bobaths were pioneering refugees who treated thousands of patients" — biography and uptake, not effectiveness evidence.
- **(c) Counterpart:** raising genuinely relevant context — e.g. a vested-interest flag (RULE-06) that bears on how to weigh the source — is on-point, not a diversion.
- *Cite RULE-06 (the relevant-context contrast); `reference/schools/bobath.md`.*

### 2.4 — Appeal to authority — foreclosing vs grounding
- **(a) Error:** using "a tutor / a guideline says so" to *foreclose* the debate.
- **(b) Example:** "the senior Bobath tutor says it works, so it works" — closing the question by status rather than evidence.
- **(c) Counterpart:** *grounding* a claim in a named, verifiable source (RULE-08) is the build's discipline, not a fallacy. **The line is foreclosure vs grounding.**
- *Cite RULE-08; `reference/schools/bobath.md § UK named defenders`.*

### 2.5 — Appeal to anecdote vs legitimate clinical experience *(delicate — gate carefully)*
- **(a) Error:** presenting a single personal story as if it settles a population-level effectiveness claim — "I had one patient who recovered with handling, so facilitation works," used to *overturn* the SR evidence.
- **(b) Example:** the same handling story deployed to dismiss the systematic-review record entirely.
- **(c) Counterpart (must NOT mislabel):** clinical experience is a legitimate *lower-tier* form of evidence in a contested field — the movement-observation/clinical-utility skill Bobath-trained therapists report (Penny's account; the framework/clinical-utility claim that survives the mechanism critique). Name it as experience-level knowledge and its evidence tier; never dismiss it as "just an anecdote."
- *Cite `reference/debates/facilitation-as-mechanism.md § For` (clinical-experience reports / Penny) + `§ Evidence` (framework/clinical-utility survives); IDENT-03.*

### 2.6 — Special pleading vs framework-unfalsifiability *(delicate — gate carefully)*
- **(a) Error:** inventing an ad-hoc exemption to shield a claim from evidence that would otherwise refute it.
- **(b) Example:** a genuine special-pleading move would invent a new excuse each time a trial comes back negative.
- **(c) Counterpart (must NOT mislabel):** "systematic reviews test interventions, not frameworks, so the framework claim is not refuted by the intervention evidence" is a *genuine epistemic state* the build deliberately surfaces — the two positions are not arguing about the same object. Calling it special pleading **inverts the build's central insight** (IDENT-03).
- *Cite `reference/debates/bobath-method-vs-framework.md § Evidence` + `§ Named gaps` (the framework-vs-treatment gap); IDENT-03.*

### 2.7 — Ad hominem / genetic vs vested-interest surfacing *(delicate — gate carefully)*
- **(a) Error:** dismissing a position because of who holds it.
- **(b) Example:** "that critic only says that because they were once passed over for a tutor post" used to *dismiss* a critique; or "the tutor is just protecting their income" used to *dismiss* a defender.
- **(c) Counterpart (must NOT mislabel):** naming the vested-interest dynamic — which cuts **both ways** — per RULE-06 is legitimate context for weighing a source, not a dismissal of the person. RULE-06 already handles this carefully, both directions, and **must stay as-is**; this rule does not turn into bias-policing.
- *Cite `reference/schools/bobath.md § Vested-interest signal` (cuts both ways, both directions); RULE-06.*

---

*Catalogue ends. Every worked example and counterpart resolves to a named entry under `reference/`. The guardrail gate above governs every entry: when in doubt, name the position and hold the tension open rather than declare a fallacy.*

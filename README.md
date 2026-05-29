# Mayston — a contested-evidence research partner for stroke-rehab CPD

Mayston was built by James — not a clinician — out of 25+ years of frontline UK community-physiotherapy experience, captured directly from his father over two recorded calls and turned into the build's problem frame. The two calls are shipped verbatim so you can audit the source: [`research/dad-followup-call-2026-05-27.md`](research/dad-followup-call-2026-05-27.md), with the full problem investigation in [`research/user-profile-investigation.md`](research/user-profile-investigation.md). The whole evidence trail — the schools landscape, the canonical debates, the competitive scan, the clinical-safety reading — lives in [`research/`](research/); start there if you want to know where every claim came from before you read a line of behaviour.

> Mayston is a contested-epistemology anchor drawn from Margaret Mayston's published 2008 Physiotherapy Research International editorial. We did not seek consent. This is not an impersonation of the living physiotherapist.

---

## What Mayston is

Mayston is a research partner for **UK contracting clinical educators preparing stroke-rehabilitation CPD briefings for NHS physiotherapy teams**. The educator has to walk into a room of band-6 physios, students, and a tutor-track colleague able to push back on a contested claim — Mayston helps them interrogate the contested evidence *before* the room, never writing the slides and never making the clinical call.

Per IDENT-03, Mayston navigates the therapeutic schools as distinct **traditions** — Bobath, task-specific training, Brunnstrom, and the rest — each with a founder, a core claim, an evidence position, and named defenders and critics. It names which fault line a contested claim sits on, surfaces the asymmetry in how the "for" and "against" sides argue, and holds both layers open (e.g. Bobath-as-intervention vs Bobath-as-framework) rather than declaring a winner the evidence does not support. Where a summariser flattens the schools into one tidy answer, Mayston keeps the tension live. Per IDENT-02 it hedges on GRADE-calibrated certainty tiers and never issues a clinical directive; per IDENT-06 it anchors to UK sources (NICE NG236, the RCP National Clinical Guideline for Stroke, CSP, ACPIN) and geography-flags non-UK guidance.

**The folder is the product.** Mayston runs as a Claude Project context bundle — upload the folder, carry it between contracts. Fork it and it is yours.

---

## Quickstart for strangers

One way in, and it is the portable one — load the folder into a Claude Project (≤5 steps, ≤5 min):

1. Open https://claude.ai/projects
2. Create a project.
3. Upload 5 items: `identity.md`, `rules.md`, `examples.md`, `profile-template.md` (the blank profile schema), and the entire `reference/` folder.
4. Set the project instructions to: `Use the uploaded files as your context. Follow rules.md and identity.md exactly.`
5. Fire a sample prompt from [`JUDGE_GUIDE.md`](JUDGE_GUIDE.md) (e.g. *"Is Bobath worth defending against task-specific training for lower-limb stroke rehab?"*).

That is the whole setup. The five uploaded items *are* the AI-context bundle (see the file map below); everything else in the repo is ship-surface documentation, not behaviour.

**New here, or coming back?** Either works as a first prompt. A newcomer can just ask *"what can you do?"* and Mayston introduces itself, honestly, in five short sections — and it can offer to set you up: say *"set me up"* and Mayston walks you through a few questions, then hands back a filled `my-profile.md` for you to **save and add to the project yourself**. It cannot write or upload that file for you — you save it and add it to project knowledge, and that file (not Mayston's memory) is what carries your profile across sessions. A returning educator can fill in `profile-template.md` (or that `my-profile.md`) directly, add it to the project, and Mayston tailors which debates and evidence it surfaces — and skips the questions it already knows the answer to. Mayston never writes the file — at most it proposes lines for you to paste back — and it never asks for patient information.

---

## Adjacent tools — complements, not competitors

Per IDENT-01, Mayston sits **upstream of** the research-retrieval tools, not in competition with them. When the educator needs a specific paper, a systematic-review verdict, an effect size, or a structured-extraction table, Mayston routes them to the right tool — then helps them debate what it returns. Different tools for different moments in the same workflow:

- **Elicit** — structured extraction across many papers.
- **Consensus** — quick "what does the literature say" verdicts.
- **Cochrane** — systematic-review certainty.
- **PubMed** — primary-literature search.
- **iatroX** — UK-clinician-facing evidence Q&A.
- **Physiopedia** — physiotherapy-specific reference.

Mayston does not retrieve, rank, or extract papers itself (IDENT-01). It is the thinking layer that sits over those results.

---

## Folder portability

Mayston's outputs are files on disk, and the folder travels. The frozen example output lives at [`briefings/team-cardiff-acute/example-bobath-vs-task-specific.md`](briefings/team-cardiff-acute/example-bobath-vs-task-specific.md) — a full worked session-close briefing produced by walking STATE-1 through STATE-4 (per RULE-09), kept on disk as both output evidence and the portability claim made concrete.

The `briefings/team-cardiff-acute/` directory IS the portability claim: `ls` it. Fork the repo and add your own `briefings/team-<X>/` — the folder travels with you between contracts.

---

## How it works — file map and cross-links

Mayston is a folder. The behaviour lives in four files (plus a blank profile schema the educator fills in); the rest is the ship surface.

**The AI-context bundle** (upload these five to a Claude Project — Path B above):

| File | Role |
|------|------|
| `identity.md` | The frame — IDENT-01..07: who Mayston is, the clinical-safety envelope, the contested-epistemology stance, the UK anchor, and the evidence-snapshot/currency frame. |
| `rules.md` | The behaviour — RULE-01..15 wrapped by the STATE-1..5 debate machine that makes the runtime trajectory inspectable. |
| `examples.md` | Five worked dialogues showing the frame in action — debate-to-draft, reasoning-integrity, orientation, a profile-tailored session, and a guided onboarding capture. |
| `profile-template.md` | The **blank** educator-profile schema. You fill it in and keep it; Mayston reads it to tailor (RULE-14) and proposes paste-back updates at close (RULE-15) — it never writes the file, and never asks for patient data. |
| `reference/` | The UK-anchored domain knowledge — the schools, the canonical debates, the retrieval-routing tree, the reasoning-integrity catalogue — cited, never restated. A dated 2026-05 snapshot, currency-flagged per RULE-10. |

**The ship surface** (documentation and demos, not behaviour):

- [`JUDGE_GUIDE.md`](JUDGE_GUIDE.md) — falsifiable prompts you can fire to test Mayston against its own claims.
- [`WRITEUP.md`](WRITEUP.md) — the three-paragraph build writeup.
- Landing page: https://mayston.pages.dev
- Repository: https://github.com/JamesMack05/mayston
- Walkthrough video: __YOUTUBE_LOOM_URL__
- Behind-the-build video: __YOUTUBE_BEHIND_URL__

The boundary is deliberate: only `identity.md`, `rules.md`, `examples.md`, `profile-template.md`, and `reference/` are the AI's context. Everything else — this README, `JUDGE_GUIDE.md`, `WRITEUP.md`, the landing page, the videos — exists to let a stranger evaluate the build, not to run it.

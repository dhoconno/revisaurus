# UW-Madison CMB PhD Admissions Committee — Simulated Review Panel

This package contains a set of role-based agent prompts that together simulate the
Cellular and Molecular Biology (CMB) PhD Admissions Committee at the University of
Wisconsin-Madison. The agents are designed to evaluate an applicant's **Personal
Statement** and **Research Statement** against the published CMB Admissions Rubric
(https://cmb.wisc.edu/wp-content/uploads/sites/538/2024/11/CMB-Admissions-Committee-Rubric_11.8.24.pdf)
and the Graduate School's holistic admissions best practices
(https://kb.wisc.edu/grad/131751).

> **Important caveat built into every agent.** A real CMB review evaluates the *whole*
> application (transcripts, CV, three letters of recommendation, supplemental
> statement about interest in CMB/Madison). These simulated reviewers only see the
> personal statement and research statement. Every agent is required to explicitly
> note which rubric categories cannot be fully evaluated from these two documents
> alone, and to score conservatively in those cases, flagging where evidence from a
> CV or letters would be needed.

---

## The Committee

| # | File | Role |
|---|------|------|
| 01 | `01_Committee_Chair.md` | Admissions Committee Chair — orchestrates the review, leads deliberation, writes the committee summary |
| 02 | `02_Faculty_Reviewer_Alder.md` | Faculty Reviewer #1 — Prof. "Alder" (molecular/biochemical; skeptical, rigor-focused) |
| 03 | `03_Faculty_Reviewer_Bemis.md` | Faculty Reviewer #2 — Prof. "Bemis" (cell biology/developmental; mentor-minded, holistic) |
| 04 | `04_Faculty_Reviewer_Chen.md` | Faculty Reviewer #3 — Prof. "Chen" (microbes/virology/systems; fit- and focus-group-minded) |
| 05 | `05_Student_Reviewer_Delgado.md` | Student Reviewer — "Delgado" (5th-year CMB student, DEIC member; community-and-wellness lens) |
| 06 | `06_Deliberation_Synthesizer.md` | Deliberation Synthesizer — reconciles reviewer scores into a committee consensus |
| 07 | `07_Rubric_Reference.md` | Shared reference document — the rubric categories, anchor descriptions, and scoring scale |
| 08 | `08_Applicant_Feedback_Writer.md` | Applicant Feedback Writer — produces the detailed, reviewer-attributed feedback letter |

---

## How to run a review (recommended sequence)

1. **Load the Rubric Reference (07)** into context. Every other agent depends on it.
2. **Provide the applicant materials** — the Personal Statement and Research Statement
   (paste text, or attach the two documents).
3. **Run each of the four reviewers (02, 03, 04, 05) independently.** Do *not* let
   them see each other's scores yet. Each produces an independent rubric scoring and
   narrative justification.
4. **Run the Deliberation Synthesizer (06)** with all four reviewer outputs as input.
   It produces a reconciled committee score, flags discrepancies, and drafts a
   preliminary recommendation (Admit-Interview / Direct-Admit-List / Waitlist /
   Decline — per the categories used in the CMB process).
5. **Run the Committee Chair (01)** to produce the official committee summary,
   including the admissions recommendation and the rationale for how individual
   reviewer perspectives were integrated.
6. **Run the Applicant Feedback Writer (08)** to produce a candidate-facing letter
   that transparently attributes scores to individual reviewer perspectives and
   explains how the committee integrated them — this is the unusual feature of
   *this* simulated committee (real committees generally do not share this level
   of detail with applicants).

You can run the agents sequentially in one long conversation (pasting each agent
prompt in turn) or in separate conversations and then combining outputs.

---

## The Rubric at a Glance

CMB uses a holistic rubric organized around four criteria
(https://cmb.wisc.edu/admissions/):

1. **Engagement in Research** *(Most Important)* — in-depth research experience,
   independence, intellectual engagement in the research question(s), and evidence
   the applicant actively sought out opportunities.
2. **Resilience / Grit / Work Ethic** *(Most Important)* — persistent behaviors,
   initiative, positive outcomes from personal or research challenges, and
   self-directed pursuit of opportunities, funding, resources, and mentors.
3. **Readiness / Fit for Program** — problem-driven (vs. technique-motivated)
   research interests aligned with CMB faculty; grounding in biology and chemistry
   through coursework, teaching, or work experience.
4. **Why UW-Madison & CMB?** — specific engagement with UW-Madison and CMB:
   named CMB faculty and research areas, and mention of Madison beyond the
   science.

Each criterion is scored on the **1.0 to 4.0 scale in 0.5 increments** used by
the actual CMB rubric (4.0 Outstanding, 3.0 Excellent, 2.0 Good, 1.0 Poor; with
0.5 increments of 3.5, 2.5, 1.5 for intermediate scores). Categories 3 and 4
cap at 3.0 (Excellent) — the 4.0 cell is N/A in the published rubric. The
Overall Score is **weighted, not averaged**: the two "Most Important" categories
carry more weight. See `07_Rubric_Reference.md` for the full anchor descriptions.

Importantly, CMB's process is deliberately *holistic*: no single metric is
disqualifying, GRE scores are **not** used, and reviewers are expected to have
completed WISELI implicit-bias training.

---

## Ethical guardrails built into every agent

- Agents must not penalize applicants for grammar errors suggestive of being a
  non-native English speaker, or for socioeconomic markers outside the applicant's
  control.
- Agents must not attempt to infer demographic characteristics (race, gender,
  nationality, religion, disability status) from the statements and must not use
  such inferences in scoring.
- Agents must flag, rather than score, any rubric element for which the two
  statements provide genuinely insufficient evidence.
- Agents must reason from the text; quoting more than short phrases from the
  applicant's statements in the final feedback is avoided to respect the
  applicant's intellectual work, though the agents may reference specifics.

---

## Output format

When all agents have run, the full deliverable to the applicant consists of:

1. **Committee summary memo** (from the Chair) — one page, recommendation + rationale.
2. **Per-reviewer rubric scorecards** (four of them) — scores, narrative.
3. **Deliberation notes** (from the Synthesizer) — where reviewers agreed, where
   they diverged, how the committee reconciled.
4. **Applicant feedback letter** — the candidate-facing integration, written to be
   constructive and developmentally useful regardless of the admission outcome.

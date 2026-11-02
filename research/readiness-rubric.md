# Readiness rubric

This rubric is for judging whether a paper is ready to release. It is written for papers of the kind
*Algorithmic Agnosticism* (AA) and *The Mind of God* (MoG) are: a short argumentative paper that
derives one central claim from owned premises, written as a structured proof in lighter prose.

## How to use it

- **Score each criterion 0–3.**
  - 0: absent or failing.
  - 1: present, with serious defects.
  - 2: sound, with minor defects.
  - 3: no defects found.
- **Back every score with evidence.** Cite file:line, or list the items checked. A score without
  evidence counts as 0.
- **Gates.** Sections A, B and C are gates: every criterion in them must score 3 before release.
  Every other criterion must score at least 2.
- **Independent review.** Run each section as an independent review, one reviewer per section, in
  parallel. Give each reviewer the paper and its proof, not the author's own scores. Reconcile the
  results afterwards.
- **Re-run after edits.** After any substantive edit, re-run A and B in full, and re-run the other
  sections for the sections that changed.
- **Record each run** in `research/review-readiness-<version>.md`, as a table of criterion, score,
  evidence and fix.

---

## A. Necessity, at the statement level (gate)

Audit every sentence of the paper, including the abstract and the footnotes. Assign each sentence
exactly one role:

| Role | Meaning |
|---|---|
| **Def** | a definition |
| **Prem** | a premise, owned with its refutation condition |
| **Cite** | a result cited from elsewhere, with a locator |
| **Der** | an item derived from earlier items, with its justification |
| **D** | a defense against an objection that would otherwise defeat a step |
| **Frame** | introduces an item, signposts, or states the question; at most one or two sentences per item |

A sentence that fits no role fails A1. Then apply these tests to each sentence:

| # | Criterion | Test | Fails if |
|---|---|---|---|
| A1 | Has a role | Assign it one of the six roles above | No role fits |
| A2 | Deletion test | Delete the sentence. Does a later step, a defense, or the reader's ability to follow break? | Nothing breaks |
| A3 | Says no more than its justification supports | Compare the sentence with the items it cites | It overclaims (watch for "always", "every", "exactly", "proves", "shows", "must") |
| A4 | No duplication | Search for the same claim elsewhere | It is stated twice, other than the canonical core claim at its fixed places |
| A5 | No dependency reminders | Look for sentences that re-cite premises already given in the item | Any reminder that isn't needed to follow the step (AA's lesson: reminders sound insecure) |
| A6 | Stays in scope | Does it rule on questions the paper declines? For MoG: whether God exists; rationality and warrant; whether an argument succeeds | It adjudicates outside the scope |
| A7 | Fixed vocabulary | Compare against the style sheet's vocabulary and language table | Synonyms drift, or forbidden terms appear (for MoG: "source", "record", "computable", "knows" of a believer) |
| A8 | Examples are needed | Does the example disambiguate a definition, or show coverage? | It is decoration |
| A9 | Rhetoric | Look for wit, sneers, rhetorical questions, and characterizations of opponents | Any of these is present |

**Score.** 3 if every sentence passes. Otherwise score by the share of failing sentences: one or
more failures scores at most 2, and a failure on A3 or A6 scores at most 1.

## B. Sufficiency, at the paper level (gate)

| # | Criterion | Test | 3 means |
|---|---|---|---|
| B1 | The dependency graph closes | Build the graph of items (definitions, premises, cited results, then derived items, then the conclusion) | Every derived item follows from the items it cites, with no missing edges and no cycles |
| B2 | No hidden premises | For each step, ask what else must be true for it to go through | Every assumption it needs is a stated premise or cited result |
| B3 | Premises owned | Each premise has a "Refuted by" condition, and is a premise the author is willing to defend | Every premise has both |
| B4 | The claims agree | Compare the title, the abstract, the introduction's claim, the conclusion item and the conclusion section | They make the same claim, at the same strength and scope |
| B5 | Defeaters answered | List the objections that would defeat a step if left unanswered (use an adversarial referee) | Each one is answered in the paper, or the step is weakened to survive it |
| B6 | Coverage claims are demonstrated | Every claim of exhaustiveness ("every route", "every argument") is backed by a case-by-case demonstration, or argued for as a premise | Yes |
| B7 | Self-application | Does the conclusion undermine its own premises, or the paper itself? | This is addressed explicitly and correctly |
| B8 | Minimality | For each premise, ask whether a weaker one would do | The weaker premise is used, or the reason it won't do is given |
| B9 | Conditional form | The paper is clear about what is proved outright and what is proved only relative to its premises | Yes |

## C. Correctness (gate)

| # | Criterion | 3 means |
|---|---|---|
| C1 | Validity | An independent logic referee finds no invalid step |
| C2 | Cited results are faithful | Every restated result matches its source in content, strength and dependence on premises, with a locator. For MoG, this means its restatement of AA |
| C3 | Quotations verified | Every quotation has been checked word for word against a primary source, with its page or locator, in a separate pass from drafting. Anything unverified is paraphrased |
| C4 | References verified | Every entry has been checked against Crossref, OpenAlex, a publisher or a catalog. DOIs resolve. No uncited entries. Years and editions match the locators cited |
| C5 | Attributions are fair | Each position attributed to a thinker is one they hold, in its strongest form. Spot-check against the source |
| C6 | Technical results (formal papers, AA) | Every theorem is proved, or cited with a locator. Known results are labeled as known. Edge cases are checked (randomized methods, probabilistic records, relativization) |

## D. Structure

| # | Criterion | 3 means |
|---|---|---|
| D1 | Title | Names the claim or the question. Any allusion is legible to the field (for example, Hawking's "mind of God"). A subtitle carries the claim if the title does not |
| D2 | Abstract | 150–250 words: the question, the premises, the method, the conclusion and its scope. No citations, no undefined terms. It states only claims the paper proves |
| D3 | Introduction | States the question, the answer and its scope, what the paper adds and does not add, and the map of the paper. It defines no new terms that §2 repeats |
| D4 | Order follows dependency | Sections run in proof order (framework, results, coverage, objections, conclusion). There are no forward references, except in the map |
| D5 | Items are findable | Every item is labeled (D1, P1, C1, and so on), has a cross-reference label, and appears exactly once |
| D6 | Conclusion | Restates the result and its scope, and makes no new claims. A closing image is fine if it adds no claim |
| D7 | Length is proportional | Each section's length matches its share of the argument. Coverage and objections do not outgrow the proof. Target length: AA as formal epistemology, about 8–12k words; MoG, about 4–7k words |
| D8 | Back matter | The AI-use statement, references, and (for repositories) README, LICENSE and CITATION.cff are present and accurate |

## E. Aesthetics and prose

| # | Criterion | 3 means |
|---|---|---|
| E1 | Plain and confident | Short declarative sentences, one claim per sentence. No hedges where the claim is proved, and no confidence where it is only assumed |
| E2 | Register of the field | AA: formal epistemology, with theorem environments and notation. MoG: philosophy of religion, no math mode, machine terms only in citations of AA |
| E3 | Consistency | The same term for the same thing throughout. Spelling (American), hyphenation, capitalization of item names, and numbering are all consistent |
| E4 | Readability | A reader in the field can follow each step without the proof file. Each item has at most one or two framing sentences |
| E5 | Typography | Builds with no warnings. No overfull boxes. Tables use booktabs and fit `\linewidth`. Cross-references resolve. Consistent quotation marks and dashes |
| E6 | Tables and figures | Each one carries content the text needs, has a caption that stands on its own, and is referred to in the text |
| E7 | Even-handedness (MoG) | Theism, naturalism and skepticism are treated alike. Traditions are described in their own terms, with standard transliteration. No thinker is given elevated status |
| E8 | No authorial presence | No discussion of the author. "We" or impersonal voice is used consistently |

## F. Scholarly positioning

| # | Criterion | 3 means |
|---|---|---|
| F1 | Closest prior work identified | A search found the nearest precedents. For AA: Müller, Vitányi, Kelly, Stanford. For MoG: Oppy, Alston, Hick, McKim, Draper. Each is either addressed, or its omission is justified because the paper makes no novelty claim |
| F2 | Novelty claims verified | Every claim of the form "to our knowledge…" is backed by a recorded literature search (`research/lit/*`). Claims that could not be verified are dropped |
| F3 | Opponents steelmanned | Each objection is stated in the form its best proponent would accept |
| F4 | The right venue and audience | The paper is pitched to its target readers (for example PhilPapers or PhilSci-Archive; *Religious Studies*, *Faith and Philosophy*, *Synthese*) and meets that venue's conventions |
| F5 | Citation norms | Author–year, consistent keys, primary texts cited by standard locators, scripture cited inline with the translation given once |

## G. Integrity and release

| # | Criterion | 3 means |
|---|---|---|
| G1 | AI disclosure | Minimal and sufficient. It states (1) that AI was used substantially; (2) which systems, with the model; (3) for what, by category; (4) that AI is not an author and the named author is responsible; (5) where the full record is. It contains nothing beyond these: no itemized author decisions, no review log, no version history, no status (status goes on the title page, G2). Everything it says is accurate |
| G2 | Status is honest | The draft or preprint status, and the absence of peer review, are stated |
| G3 | Reproducible build | A clean checkout builds the PDF with one documented command |
| G4 | Repository hygiene | Private material is gitignored. No secrets. History is as intended (flattened or kept). The README's claims about history are true |
| G5 | Versioning | A tag, a CITATION.cff version, and a DOI (Zenodo) once released. The changelog matches |
| G6 | Licence | Stated in both the repository and the PDF (CC BY 4.0) |

## H. External review

| # | Criterion | 3 means |
|---|---|---|
| H1 | Adversarial logic referee | An independent run found no FATAL or SERIOUS issues outstanding |
| H2 | Trace audit | An independent run of the draft against the proof found no unresolved items |
| H3 | Cross-model review | At least one review by a different system (for example Grok). Each of its points is adjudicated, applied or declined, with reasons recorded |
| H4 | Human reader | At least one reader in the field has read the paper, or its absence is stated (G2). Required before submission to a journal; not required for a preprint |

---

## Release thresholds

- **Preprint (GitHub, Zenodo, PhilPapers):**
  - A, B and C all score 3;
  - D–G all score at least 2;
  - H1–H3 score 3.
- **Journal submission:**
  - everything required for a preprint;
  - D–F all score 3;
  - H4 scores 3;
  - the venue's formatting requirements are met.

## Template for each run

```
| Criterion | Score | Evidence (file:line / items checked) | Fix |
|---|---|---|---|
| A1 | | | |
```

For section A, also attach the sentence-role table:

```
| file:line | sentence (first words) | role | A2–A9 failures |
```

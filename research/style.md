# Style sheet for drafting *The Mind of God*

All section authors follow this sheet. The argument spine (`research/argument-spine.md`) is the
single source of truth for content. The research notes (`research/lit/01–10`) are the source for
every quotation and citation.

## Voice and register
- **Philosophy of religion, not mathematics.** No formulas, theorem environments, or symbols such
  as K(x) or φ. Use "result", "conclusion" or "argument" rather than "theorem" in the body. Name
  AA's results in words, for example "the first result (no certification)", and cite AA for the
  proofs: `\citep[§3]{taylor2026aa}`.
- **Confident and plain.** State each claim once, where it belongs. Make no reminders of which
  premises a claim depends on beyond the canonical statement (AA's necessity rule).
- **Even-handed.** Theism, naturalism and scepticism are treated alike (the parity thesis). Never
  sneer. Represent every tradition in its own terms, with standard transliteration.
- **Never assert that a believer "knows".** Say: a believer *may hold the truth* (on externalist
  accounts, may even be said to know it); what no one can do is *establish* that they hold it.
- **No thinker gets elevated status.** Authors appear as examples within categories.
- **The author is not discussed.**
- **British or American spelling:** American (skepticism, behavior).

## The fixed vocabulary (use exactly these terms)
- **the source** (of human experience, of the record): what God is mapped to. Never "the
  universe".
- **the record:** the finite body of human experience and its traces.
- **worldview:** the unit of analysis, a class of possible worlds. Use **religious tradition** for
  historical communities.
- **route to belief:** the nine routes, numbered as in the spine, §4A.
- **standard of knowledge:** the seven standards, numbered as in the spine, §4B.
- **rival:** a **whole-record rival** agrees with everything that could ever be experienced (AA's
  third result). A **rival that differs on the unobserved** is eventually distinguishable but not
  certifiably so (AA's first and second results).
- **imposed constraint:** a choice among surviving worldviews that the record does not make (AA C′).
- **parity thesis:** the core claim (spine §0).
- **AA's three results:**
  - the **first result**: no certification, for methods of any kind;
  - the **second result**: no reliable discovery by any followable route;
  - the **third result**: permanent underdetermination, even for an ideal knower.

## Citations
- Use natbib author–year: `\citet{key}` gives "Author (Year)"; `\citep{key}` gives "(Author Year)";
  `\citep[p.~191]{key}` adds a page.
- **Key convention:** lowercase first-author surname plus year, e.g. `plantinga2000`, `hick1989`,
  `law2010`. Add a suffix letter for a second work in the same year (`derose1999`; `hick1960`). For
  multiple authors, use the first author only (`griffiths2006`).
- **Fixed keys for primary and classical texts** (use exactly these):
  - `taylor2026aa`: Algorithmic Agnosticism (AA)
  - `hawking1988`
  - `davies1992`
  - `huxley1889`
  - `draper2022`: SEP, "Atheism and Agnosticism"
  - `flew1972`
  - `hume1748`: *Enquiry*; cite as `\citep[§10]{hume1748}`
  - `aquinas-st`: *Summa Theologiae*; cite as `\citep[II-II q.4 a.8]{aquinas-st}`
  - `aquinas-scg`
  - `vatican1870`: *Dei Filius*
  - `ccc1992`: the Catechism
  - `calvin1559`: *Institutes*
  - `berkeley1710`: *Principles*
  - `berkeley1713`: *Three Dialogues*
  - `pascal1670`: *Pensées*
  - `james1896`: "The Will to Believe"
  - `clifford1877`
  - `newman1870`: *Grammar of Assent*
  - `kierkegaard1846`
  - `maimonides-guide`
  - `maimonides-mt`: *Mishneh Torah*
  - `halevi-kuzari`
  - `ghazali-munqidh`
  - `ignatius-exercises`
  - `john-of-the-cross-ascent`
  - `teresa-life`
  - `jsh1838`: Joseph Smith—History
  - `jsp-firstvision`: the Joseph Smith Papers accounts
  - `lds-firstvision-essay`
  - `quran`
  - `bible`
  - `bukhari`
  - `tabari-history`
- **Scripture** is cited inline by book, chapter and verse ("Exodus 4:1–9"; "Qur'an 22:52"; "Sahih
  al-Bukhari 3"), without a `\cite` each time. Cite `bible` / `quran` / `bukhari` once, at first
  use, for the translation used.
- **Only cite works that appear in the research notes** (lit/01–10) or the spine. List every key you
  use, with its full bibliographic details, at the end of your final reply. A bibliography agent
  will build `refs.bib` from these lists.
- Items marked **unverified** in the research notes may be used only without quotation marks, or
  with "[verify]" in a LaTeX comment beside them.

## LaTeX
- Each section is a file `paper/sections/NN-name.tex` beginning `\section{Title}\label{sec:name}`.
- **Section labels:**
  - `sec:intro`
  - `sec:aa`
  - `sec:mapping`
  - `sec:routes`
  - `sec:standards`
  - `sec:diversity`
  - `sec:objections`
  - `sec:conclusion`
- **Subsection labels** use the prefix `ss:`. Footnotes are fine.
- **Tables:** use booktabs with p-columns, no wider than `\linewidth`.
- **No theorem environments, no math mode** beyond the occasional symbol.

## Word budgets (target about 10,000 words in total)
| Section | Words |
|---|---|
| 1. Introduction | 1,000 |
| 2. Algorithmic agnosticism without mathematics | 1,100 |
| 3. The mapping | 1,100 |
| 4. Routes to belief | 2,400 |
| 5. Standards of knowledge | 1,300 |
| 6. Religious diversity and the width of the field | 800 |
| 7. Objections | 1,500 |
| 8. Agnosticism, justified | 500 |

---

## v3 addendum (the structured-proof draft)

This addendum overrides anything above that conflicts with it.

- **Source of truth:** `research/proof.md`. Every statement in the paper is an item of the proof, or
  short prose that introduces one. Nothing else is stated.
- **Items in the text:** each definition, premise, lemma and conclusion appears as a labelled,
  bold run-in item, numbered as in the proof (**D1**, **P1**, **L1**, **C-a**, …), followed by its
  justification in brackets, e.g. "(from P2, D4 and L1)". Use the labels `item:D1`, `item:L2`, and
  so on, so that items can be cross-referenced.
- **Prose:** light. One or two sentences introduce each item, and an example appears only where it
  is needed. Do not repeat a dependency in prose once it is stated in the item.
- **Word budget:** about 6,000–7,000 in total.
- **First-draft text** (git commit `8e177bc`, `paper/sections/*`) may be reused where it states a
  proof item exactly. Retrieve it with `git show 8e177bc:paper/sections/NN-name.tex`.
- **Quotations:** use only those verified in `research/review-quotations.md` (EXACT, or corrected).
  Never use one that report marks NOT FOUND or wrong.

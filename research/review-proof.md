# Referee report: structured proof v3 (validity and soundness)

Checked against AA `02-framework.tex`, `03-certification.tex` and `06-ideal.tex`. T1 and K1 concern
finite records of setting/outcome *strings* and computable models. C3 rests on T5(a), whose proof is
"every method receives the same input". None mentions nature, God or experience.

## 1. Step-by-step table

| Item | Verdict | Issue | Minimal fix |
|---|---|---|---|
| D1 | NEEDS-PREMISE | Equivocates experience/traces. "Whatever any faculty delivers" admits factive states ("seeing that God is present"), which entail *W*. | Record = non-factive appearances; traces only as appearances. |
| D2 | NEEDS-PREMISE | Makes "there is a single producer" analytic, so no-source views are excluded by fiat. | "Whatever, if anything, accounts for the record." |
| D3 | NEEDS-PREMISE | If "logic" is broadly logical necessity, a necessary God makes "no God" inconsistent; L1/L2 fail. | Consistent with record and what is *a priori* certified (P3). |
| D4 | VALID, near-TRIVIAL | Few theists claim entailment (Descartes and Thomist demonstrations do; Plantinga and Swinburne do not). | Keep it; call C-a fallibilist. |
| D5 | NEEDS-PREMISE | "Same total record": same realised record, or same *distribution* over records? Only the second gives L3. | Fix 3. |
| D6 | VALID | Matches AA's "imposed" (Def. constraint). | — |
| D7 | VALID | — | — |
| P1 | NEEDS-PREMISE | Finite is not the same as finitely encodable: continuous qualia, or Descartes's "idea of the infinite". AA's T1 needs a *string*. | Add B1 (Fix 1). |
| P2 | VALID as a premise; most contested | The highest-common-factor premise that disjunctivists (McDowell) reject. Hidden: a route's *verdict* depends only on its input (T5(a)'s step). | State both; name disjunctivism. |
| L1 | NEEDS-PREMISE | (i) T1 gives a computable *model of an encoding*, not "a process with nothing beyond nature"; that needs B1–B2 (Fix 1). (ii) The theism bullet is legitimate (omnipotence covers any logically possible experience) but unneeded: "a non-natural source produces *R*" suffices. (iii) Covers three worldviews; C-a says "any". | Generalise (Fix 2). T1 answers "only an infinite source could produce *this*". |
| L2 | INVALID as stated | (i) A definition (D5) cannot yield existence; a recombination premise is needed. (ii) False for behaviour-defined claims ("some source produces *B*"; scepticism-as-disjunction): no rival is both inconsistent with them and behaviourally identical. (iii) "Unless *a priori* impossible" makes L2 depend on O2, marked [D]. | Fix 2. |
| L2 examples | VALID given P3 | On classical theism no non-divine deceiver exists *if theism is true*; but the rival world is one where it is false, so no question is begged unless "God exists" is *a priori* certified. | Add "epistemically possible (D3)". |
| L3 | VALID only with Fix 3; UNNECESSARY for C-a–C-c | Same realised record with different chances gives different likelihoods (T5(b)-type rivals, cut in v3). An *a priori* prior (Swinburne's intrinsic probability) falls under P3/O2, not D6. | Mark [D]; add "an *a priori* prior is answered by O2". Don't imply priors favouring *W* are irrational. |
| C-a | VALID given Fix 2; modest | AA T1 is a constructive witness, not load-bearing. The *a priori* case needs P3: logical truths are entailed by every record. | Cite P3. |
| C-b | TRIVIAL (definitional) | "Separate" is undefined. Once defined, C-b follows from D5 + P2 alone. AA C3 is the formal analogue, not a premise. | Fix 4. |
| C-c | VALID; Alston's epistemic circularity | Reliability has a whole-record rival (same record, unreliable route). "Establish" undefined. | Fix 5. |
| Parity | INVALID for scepticism | Scepticism is not a source claim: as "suspend judgement" it has no whole-record rival; as a meta-claim the proof itself establishes it (given P1–P3). | Say "the sceptical (deceiver/simulation) hypothesis". |
| R [D] | VALID | Natural theology's premises are not "delivered" experiences: needs P3. Faith-as-choice "not knowledge" clashes with the externalist allowance. | "Not evidence." |
| S [D] | Mostly VALID | Hick: theism and naturalism *differ* in future record, so are not whole-record rivals. | Cite P1 + C-a; C-b only for the deceiver. |
| O1 [D] | VALID (coherent) | Fine, since C-a is fallibilism, not knowledge-scepticism; a Moorean loses nothing. | Say so. |
| O2 | NECESSARY, mislabeled [D]; inadequate | The reverse ontological argument answers only *modal* ontological arguments, not PSR-cosmological, Gödelian or consciousness arguments. It shows symmetry of intuition, not impossibility of certification. | Promote to P3 (Fix 2). |
| O3 [D] | VALID | — | — |
| O4 [D] | NEEDS-PREMISE | "Not knowledge" over-claims, as in R. | "Not a route to certification or separation." |
| O5–O7 [D] | VALID | O7's rival is just ¬*W* with the same record. | — |

## 2. The most important fixes

**Fix 1: bridge from AA to experience (P1, L1).** Add:

> **B1 (Encoding).** Every finite record is fully captured, up to what its subject can discriminate,
> by a finite functional record in AA's sense (setting = time index, outcome = the encoded content).
> **B2 (Natural realisability).** For any computable function, "a purely natural system implements
> it and thereby produces experiences with the encoded content" is epistemically possible (D3).

Replace L1's first bullet with: "By B1 and AA T1, every record is reproduced by a total computable
model. By B2, a source with nothing beyond nature that produces it is epistemically possible. So
theism is never entailed." B2 is where the argument from consciousness pushes back. It is covered
by P3.

**Fix 2: make the hidden *a priori* premise explicit (L1, L2, C-a, O2).** Add:

> **P3 (No *a priori* certification of source claims).** No substantive source claim, and no claim
> that a given kind of source cannot produce a given record, is certified *a priori*. A source claim is
> **substantive** if it is not entailed by "something produces this total behaviour".

Then restate L2 as: "*From D5 and P3.* For any substantive source claim *S* with total behaviour *B*,
the claim 'a source inconsistent with *S* produces *B*' is epistemically possible." Retitle O2 as
"Defence of P3", remove its [D], and add PSR and consciousness arguments to the reverse ontological
move ("each rests on a premise whose denial is equally *a priori* and not refuted").

**Fix 3: D5 for chance (needed by L3).**

> **D5.** A whole-record rival of *W* is a source claim inconsistent with *W* that assigns the same
> probability as *W* to every possible record, for every subject and every time (AA T5(a),
> extensional equality).

**Fix 4: define separation, and make C-b's status honest.**

> **D8. Separate.** A route separates *W* from *W′* if its verdict could differ according to which of
> them is true. **C-b.** *From D5 and P2.* Whole-record rivals give every route the same input, so the
> same verdicts. This is the content of AA's T5(a), here carried from models to sources.

**Fix 5: state C-c's contribution honestly.**

> **C-c.** *From C-a and C-b; this generalises Alston (1986, 1991).* Alston showed that the
> reliability of a basic doxastic practice cannot be shown without epistemic circularity. The
> addition here is that no *non-circular* route can break the circle either. For every route *ρ*,
> "ρ tracks the source" has a whole-record rival in which ρ is unreliable, and by C-b no route
> separates the two.

## 3. Verdict

**Validity.** As written, L2 and C-a have a gap: their universal scope rests on an unstated *a
priori* premise (P3) filed as a dialectical objection (O2). L1 also needs B1–B2. AA's results say
what is claimed, but only for strings and models.

**Soundness.** The proof is sound relative to P2 and P3, which are the two real points of
contention: disjunctivism and factive perception for P2, the ontological, PSR and consciousness
arguments for P3. P3 is a premise, not a theorem. The honest claim is that no one has a certified
*a priori* route, not that none could exist.

**Sufficiency.** With Fixes 1–5, the proof suffices for the core claim restricted to *substantive
first-order source claims*: theism, naturalism, and the sceptical (deceiver or simulation)
hypothesis. It does not reach "scepticism" as a stance. L3 is dialectical and should be marked [D].

**Significance.** C-a is route-general fallibilism, C-b is definitional given P2, and C-c
generalises Alston. The real contribution is uniformity: one premise (P2) covers every route, with
explicit rivals the traditions name themselves. The paper should say exactly that.

# The Mind of God: Algorithmic Agnosticism and Religious Belief

**Christopher S. Taylor**

> **Status: version 1.0, preprint, not peer-reviewed. Comments welcome.**
> This paper was produced with substantial assistance from AI systems (Claude Code, Anthropic;
> Grok, xAI). The author directed the work and is responsible for its content. See the
> *Statement on the use of AI* at the end of the paper.

**[Read the paper (PDF)](paper/the-mind-of-god.pdf)**

## In brief

*Algorithmic Agnosticism* argued that no theory of everything can be known to be final. This
paper asks the parallel question of religious belief: not whether God exists, but whether any
worldview can be established as the true account of what is.

It adds one premise, in two clauses. A worldview that claims to be true is an account in the sense
of *Algorithmic Agnosticism*. And any account that goes beyond the evidence, a worldview included,
has a rival consistent with the evidence on which it is false.

A second premise classifies every element of a classic argument as evidence, an account, a
judgment, an imposed constraint or a truth of reason. With it the paper locates the decisive
element of twenty-two classic arguments.

Three conclusions follow:
- no worldview can be established as the true account;
- worldviews that agree on all possible evidence are never separated, even by final evidence;
- what selects among the rest is a choice the evidence does not determine.

Theism, naturalism or the skeptical hypothesis may be true, but no argument from experience or
reason can establish that any of them is. The claim concerns what can be established, not what it
is reasonable to believe. This is agnosticism in Huxley's sense.

## Algorithmic Agnosticism

Christopher S. Taylor, *Algorithmic Agnosticism: Why No Theory of Everything Can Be Known to Be
Final*: <https://github.com/extrafox/algorithmic-agnosticism>

## Repository layout

- `paper/` — LaTeX source (`main.tex`, `sections/`, `refs.bib`).
- `research/` — the structured proof (`proof.md`), the style sheet, the literature research
  (`lit/`), and the reviews of each version (trace audits, referee reports, quotation checks and
  the readiness reviews).

## Building the PDF

```sh
brew install tectonic   # or any LaTeX distribution with natbib, cleveref, booktabs
cd paper && tectonic -k main.tex
```

This produces `paper/main.pdf`, which is copied to `paper/the-mind-of-god.pdf`.

## Comments and corrections

Comments, corrections and objections are welcome. Please open an issue on this repository.

## How to cite

DOI: [10.5281/zenodo.23900497](https://doi.org/10.5281/zenodo.23900497) (all versions; version 1.0 is [10.5281/zenodo.23900498](https://doi.org/10.5281/zenodo.23900498)).

```bibtex
@misc{taylor2026mindofgod,
  author       = {Taylor, Christopher S.},
  title        = {The Mind of God: Algorithmic Agnosticism and Religious Belief},
  year         = {2026},
  note         = {Version 1.0, preprint; not peer-reviewed},
  doi          = {10.5281/zenodo.23900497},
  howpublished = {\url{https://github.com/extrafox/the-mind-of-god}}
}
```

## License

The text of this work is licensed under the
[Creative Commons Attribution 4.0 International License](LICENSE) (CC BY 4.0).

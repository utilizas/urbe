# Overrun

**A Resident's Report on a City Past Its Limits**  
*Civic Darwinism, Volume I*

[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-rust.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
[![Quarto](https://img.shields.io/badge/built%20with-Quarto-blue)](https://quarto.org/)
<!-- DOI badge to be added after first Zenodo release -->

A hybrid analytical-satirical essay examining urban habitability
degradation through five civic perspectives — residence, commuting,
leisure, public space, and education — in a Mediterranean city
reconstituted as a platform of value extraction.

The volume is set in Granada (Spain) but written so that the
processes described are recognisable wherever similar pressures
operate; explicit naming is kept indirect throughout. The narrator
is a moderately-paid qualified professional who has become, against
his expressed wishes, a reluctant witness to the conditions
he documents.

---

## Read the volume

The canonical deployment is on Vercel. Mirrors are provided for
redundancy and serve identical content.

| Deployment    | URL                                                          |
|---------------|--------------------------------------------------------------|
| **Canonical** | <https://urbe-ten.vercel.app/>                               |
| Netlify       | <https://urbe.netlify.app/>                                  |
| Cloudflare    | <https://urbe.utilizas.workers.dev/>                         |
| GitHub Pages  | <https://utilizas.github.io/urbe/> *(partial assets)*        |

The GitHub Pages mirror does not serve all illustration assets and
is retained only for redundancy; for the complete reading
experience, the Vercel deployment should be preferred.

---

## Structure

The volume is composed of a preface, five central chapters, a coda,
a glossary, a data appendix and a methodological note. Each chapter
examines the same city through a different functional encounter;
the cumulative portrait emerges from the convergence of partial
views rather than from a single authoritative position.

```
urbe/
├── _quarto.yml                       Project configuration
├── index.qmd                         Preface
├── 00-before-the-threshold.qmd       A City Still Worth Loving
├── 01-residents-return.qmd           The Resident's Return
├── 02-commuters-gauntlet.qmd         The Commuter's Gauntlet
├── 03-citizen-without-leisure.qmd    The Citizen Without Leisure
├── 04-flaneur-under-siege.qmd        The Flâneur Under Siege
├── 05-academic-observer.qmd          The Student Who Stayed On
├── 07-coda.qmd                       Neither Sentimentality nor Resignation
├── glossary.qmd                      Glossary of Terms in Occasional Use
├── appendix-traffic-sanctions.qmd    Comparative sanctions, Andalusian capitals
├── note-on-method.qmd                Note on Authorship and Method
│
└── _assets/
    ├── civic-darwinism.scss          Light theme
    ├── civic-darwinism-dark.scss     Dark theme
    ├── references.bib                Bibliography
    └── figures/                      Plates and data figures
```

---

## Build locally

The volume is authored in [Quarto](https://quarto.org/) and renders
to HTML.

```bash
git clone https://github.com/utilizas/urbe.git
cd urbe
quarto render
```

To preview with live reload:

```bash
quarto preview
```

The output is written to `_book/`. Two SCSS themes — light and
dark — are declared in `_quarto.yml` as separate files; Quarto's
native toggle handles the switch and persists the reader's
preference in `localStorage`.

---

## Citation

If you cite this work, please use the metadata in
[`CITATION.cff`](./CITATION.cff). GitHub renders it automatically
as a "Cite this repository" widget in the sidebar. A DOI will be
minted on the first Zenodo release and added to this README at
that point.

A working citation in author-date form, prior to the DOI:

> Moreno, M. (2026). *Overrun: A Resident's Report on a City
> Past Its Limits.* Civic Darwinism, Vol. I.
> <https://urbe-ten.vercel.app/>

---

## Licence

© 2026 Miguel Moreno.

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0
International Licence](https://creativecommons.org/licenses/by-nc-sa/4.0/)
(CC BY-NC-SA 4.0). You are free to share and adapt the material
for non-commercial purposes, provided you give appropriate credit
and distribute any derivative work under the same terms. The
illustrations, generated as described in the methodological note,
are subject to the same licence as the text they accompany.

The terms permit translations, critical editions and academic
adaptations under the same licence; they do not permit commercial
reuse without explicit permission.

---

## Method

The text was composed between early 2025 and spring 2026 as a
collaboration between a human author and a large language model,
under a working brief and tonal rules established before any
chapter was drafted. The conditions of production are documented
in [`note-on-method.qmd`](./note-on-method.qmd) and rendered at
the end of the volume; they are recorded not as a disclaimer but
as a methodological fact, on the principle that withholding them
would be inconsistent with the analytical standards the volume
has tried to maintain elsewhere.

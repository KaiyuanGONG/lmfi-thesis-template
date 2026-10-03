# LMFI thesis recommendations / Recommandations pour les mémoires LMFI

## Status and sources

These recommendations are **not official**. They are descriptive defaults based
on an aggregate review of 119 past master's theses dated from 2016 through 2025.
The local archive held 183 PDF files. The 119 analysed documents are every PDF
in the ten yearly folders that has at least two pages (this drops single-page
jury forms and scans), minus two slide decks. The subset still contains one
exact duplicate and two near-duplicate pairs, and the files alone cannot confirm
that every document belongs to the LMFI track, so it should be read as a sample
of past theses in the archive, not as a verified LMFI census. Only aggregate
observations are published here: no past thesis text, image, name, or personal
metadata is redistributed by the template.

The figures were re-derived from the PDFs on 2026-10-02 (page count, paper size,
fonts and producer metadata, and text extraction). The corpus contains no
`.tex` sources, so the document class, chapter structure, bibliography style
and front-matter items are estimates from the rendered layout and carry an
uncertainty of a few documents.

As of 2026-08-20, the public [LMFI programme page](https://master.math.u-paris.fr/annee/m2-lmfi/)
describes the research internship/master's thesis and its 16 ECTS value, but the
review did not locate a public LMFI rule for page count, font, margins, cover, or
chapter structure. Programme or supervisor instructions discovered later override
everything in this document.

## Aggregate observations

| Observation | Corpus result | Template response |
|---|---:|---|
| Main language | 62% English, 38% French | English default; complete French entry point |
| Recent language trend | about 80% English in 2024 (20 of 25) | Keep English as the default Overleaf main file |
| Document class (estimated from layout) | about 79% without a chapter level; about 21% chapter-structured | Use `report` deliberately for long chapter-based work |
| Length | median 37 pages; wide 11--104 range | No mandatory length; report the observed range and defer to the supervisor |
| Top-level divisions | median 5 numbered sections or chapters (mean 5.3); chapter-structured theses: median 4 | Ship five independent chapter files |
| Engine | 105/119 pdfLaTeX; 6 XeLaTeX or LuaLaTeX; 8 other or unknown | Default to pdfLaTeX and portable TeX Live packages |
| Paper | 59% A4; 40% Letter | Enforce A4 for a French university context |
| Typeface | 82% Computer/Latin Modern; Libertine 3 cases | Libertine/NewTX is a readability choice, not a corpus rule |
| Bibliography | 63% numeric; 27% alphabetic; 4% author-year; 6% unlabelled or none | Use numeric citations in order of appearance |
| Figures and tables | 80% had no captioned figure; 94% had no captioned table | Demonstrate one of each; keep their lists disabled |
| Front matter (dedicated heading) | acknowledgements 10%; appendix 16%; notation 5% | Keep these as switches; the example enables acknowledgements by default |
| Title page (pages 1--2) | year or date 83%; thesis/report wording 71%; programme name or acronym 50%; supervisor named about 69% | Keep a concise editable cover without a jury table; optional academic-referent line and up to three logo slots |

These percentages describe the available historical corpus, not a judgement of
quality. Page count, paper size and producer are read from PDF metadata; the
other rows come from automated text and layout extraction, which can
misclassify scanned pages, math fonts, bibliography labels or front-matter
headings (the notation share, for instance, depends on how a notation list is
defined). The strongest layout decisions were therefore checked against
rendered examples.

## Why this template uses chapters

The corpus majority used `article`, but a reusable template for a long
chapter-based internship or research report benefits from `report`: chapters start cleanly,
each has a separate source file, and `\includeonly` supports focused drafting.
This is a template design decision. It does not imply that an `article` thesis is
invalid.

The neutral five-chapter skeleton can be expanded without changing the style:

- Theory: Introduction; Preliminaries; Main Result I; Main Result II;
  Applications; Conclusion.
- Applied work: Introduction; Background; Method or Formal Setting; Experimental
  Protocol; Results; Discussion; Conclusion.

Theorem-like environments and equations are numbered by chapter (Theorem 3.2,
equation (3.1)), which keeps numbers short in a `report` with few sections.

---

## Statut et sources

Ces recommandations sont **non officielles**. Elles décrivent des tendances
agrégées observées dans 119 anciens mémoires de master datés de 2016 à 2025.
L'archive locale contenait 183 fichiers PDF. Les 119 documents analysés sont
tous les PDF des dix dossiers annuels comptant au moins deux pages (ce qui écarte
les fiches de soutenance d'une page et les scans), moins deux présentations
projetées. Cet ensemble contient encore un doublon exact et deux paires de
quasi-doublons, et les fichiers seuls ne permettent pas de confirmer que chaque
document relève du parcours LMFI : il faut le lire comme un échantillon d'anciens
mémoires de l'archive, non comme un recensement LMFI vérifié. Le modèle ne
redistribue aucun texte, nom, visuel ou renseignement personnel provenant d'un
ancien mémoire.

Les chiffres ont été recalculés à partir des PDF le 2026-10-02 (nombre de pages,
format du papier, polices et métadonnées du producteur, extraction du texte).
L'archive ne contient aucune source `.tex` : la classe de document, la structure
en chapitres, le style bibliographique et les éléments liminaires sont donc des
estimations fondées sur la mise en page rendue, avec une incertitude de quelques
documents.

Au 20 août 2026, la [page publique du LMFI](https://master.math.u-paris.fr/annee/m2-lmfi/)
présente le stage/mémoire de recherche et sa valeur de 16 ECTS, mais aucune règle
publique LMFI concernant longueur, police, marges, couverture ou chapitres n'a
été trouvée. Toute consigne ultérieure du programme ou de l'encadrement prévaut.

## Lecture des résultats

Les chiffres du tableau anglais sont descriptifs et ne constituent ni un barème
ni une évaluation de qualité. Ils justifient notamment l'anglais par défaut, A4,
pdfLaTeX (105 documents sur 119), les citations numériques (63 %) et le caractère
facultatif des listes (80 % sans figure légendée, 94 % sans tableau légendé). Le
choix de `report` et de Libertine/NewTX reste un choix explicite de conception.

La structure à cinq chapitres correspond à la médiane des divisions numérotées de
premier niveau (5 ; 4 pour les seuls mémoires structurés en chapitres). Elle peut
être divisée en plusieurs résultats pour un mémoire théorique, ou en méthode,
protocole, résultats et discussion pour un mémoire appliqué. Les longueurs
observées (11 à 104 pages, médiane 37) sont descriptives ; aucune longueur n'est
une exigence officielle du LMFI.

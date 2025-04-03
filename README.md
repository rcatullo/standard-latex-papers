# Mathematics LaTeX Templates and Papers

## Standard Paper

The standard paper style file contains the basic formatting necessary for a standard research paper written in LaTeX. This includes almost every standard package that one imports to most TeX documents (amsmath, amsthm, etc...) as well as custom packages for formatting. A full list of required packages can be found in the header at the top of the document. Some particular features are listed below
- Indenting of paragraphs is replaced by `0.5em` paragraph lineskips
- Geometry package used to fix one inch margins on all sides
- Section Formatting
  - Section titles are centered in small caps
  - Subsection titles are formatted inline in bold font on their own line
  - Abstracts are included by `abstract{#1}`, and are centered with center-justified text
  - Table of contents has both sections and subsections listed with no indentation, `0.5em` spacing between sections, normal (not bold) font, and proper numbering. Dots connect section/subsection titles on the left with page numbers on the right.
  - Bibliography is generated with `bibtex` using `biber` backend, entries are styled alphabetically (e.g. `[BK04]`)
- Fancy headers and footers are applied, with headers containing section on the left and page number on the right
- Enumerate environments default to `(\roman*)` labels, i.e. `(i) (ii) (iii)`
- Theorem environments
  - Includes standard numbered theorem environments `\thm, \lem, \prop, \cor, \defn, \exmp, \exer` numbered first by section, then by order of environment
  - Also includes unnumbered environments `\rem, \conj, \todo`
  - Theorem titles are bold font, statements are in italics, and numbers are normal font (if applicable)
 
## Standard Operators

This style file's purpose is to create standardized commands for all of the commonly used math functions and symbols that standard TeX compilers can't recognize. It is an ever-growing list of standard operators, commands, and redefined commands categorized by subject within math. Here is a broad overview, where we use `*` to denote any alphabetic character and `**` for the same character capitalized (e.g. `* = a` and `** = A` in the first command means `\bba = \mathbb{A}`)
- `\bb* = \mathbb{**}`
- `\mf* = \mathfrak{*}`
- `\mf** = \mathfrak{**}`
- `\cal* = \mathcal{**}`
- `\fan* = \mathscr{**}`
- Categories
  - Most categories are included by the command you expect, and are formatted by `\mathsf`. Here are a few examples.
  - `\Set = \mathsf{Set}`
  - `\Mod = \mathsf{Mod}`
  - `\Sch = \mathsf{Sch}`
  - `\Grpd = \mathsf{Grpd}`
  - Some standard operators are also included like `\op, \coker, \coim`
- Algebra
  - Most commands one uses regularly are included as operators, including the following. Note these aren't commands with arguments, so for example Hom(A,B) should be formatted `\Hom(A,B)`. It is my opinion that this is much faster to type in practice than `\Hom{A}{B}`. 
  - `\Ext`
  - `\Hom`
  - `\Tor`
  - `\Aut`
  - `\End`
- Algebraic Geometry
  - `\ox = \mathcal{O}_X` - this one is a huge timesaver
  - `\spec` is a math operator, such that one can write `\spec(A)` for Spec(A) and `\spec A` for Spec A
  - `\Hilb, \Quot, \Gr, \proj`, and so on.
- Analysis
  - Better formatting for differential forms. In this case `*` can be taken as a greek letter, e.g. `\dtheta` for `\mathrm{d}\theta`
  - `\d* = \mathrm{d}*`
  - `\d** = \mathrm{d}**`
  - **Warning**: I had to exclude `\dp` since this is used by LaTeX compilers to define box depth
  - `\del = \partial`
  - `\veps = \varepsilon`, `\vphi = \varphi`
  - `\curl` and `\grad` operators

## Skeleton

The skeleton folder contains a basic outline for a mathematics paper written in LaTeX. The *main.txt* file contains a basic paper outline. The *standard.sty* file contains standard mathmode shorthands for common objects as well as formatting of titles, sections, subsections, tocs, and bibliographys. The *refs.bib* file should contain bibliography references.

## Beamer Skeleton
The skeleton-beamer folder contains an outline for beamer presentations. The *main.txt* file contains a basic presentation outline. The theme and colortheme are contained in *standard-beamer.sty*, as well as nonconflicting packages and mathmode shorthands from standard.sty. The logo is contained in *Images/block_logo.png* and can be changed from within standard-beamer.sty.

## Papers

This contains the TeX files for my publically available mathematics research papers and lecture notes. I cannot guarantee correctness of any material contained
in these papers but you are welcome to contact me if there is a glaring issue that needs attention.

## Contact

Ryan Catullo

e: rcatullo@stanford.edu

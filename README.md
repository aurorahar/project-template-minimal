# Specialization Project Template (minimal)

## Quick start
1. Fill in title, name, course and supervisor at the top of `main.tex`.
2. Write in `frontmatter/`, `chapters/` and `appendices/`.
3. Add references to `references.bib`, cite with `\cite{key}`.
4. Put images in `figures/`.
5. Build with `latexmk` (or save in VS Code). Output: `build/main.pdf`.

## Structure
Title page → Abstract → Sammendrag → Contents →
1 Introduction → 2 Theory → 3 Method → 4 Results and Discussion →
5 Conclusion and Further Work → References → Appendix A

Add or remove chapters with the `\input{...}` lines in `main.tex`.

## Tips
- `\cref{fig:example}` → "Figure 3.1" (works for tables, equations, chapters).
- `\todo{...}` for notes; hide all with `\usepackage[disable]{todonotes}`.
- Need a list of figures? Add `\listoffigures` after `\tableofcontents`.
- Customising: open `settings/preamble.tex` and search for `EDIT`.
  - **Colours** (top of the file): blue links, green citations. Set them to black for print.
  - **Font**: swap the font lines for one of the listed alternatives.
  - **Your own packages and commands**: add them in the marked section near the end
    (above `hyperref`, which must stay last).

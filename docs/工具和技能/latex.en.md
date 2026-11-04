# TOOL-108: LaTeX

## Descriptions

- Offered by: The official LaTeX project plus Chinese material from the CTEX community ([LaTeX project](https://www.latex-project.org/))
- Prerequisites: Basic computer literacy only, no typesetting experience needed; for coursework use, basic competence with mathematical notation helps
- Programming Languages: Source files are written in LaTeX markup and compiled with engines such as `pdflatex` or `xelatex`
- Difficulty: 🌟🌟
- Class Hour: About 8 hours for syntax and document structure, or 20 or more hours to typeset a complete paper on your own

LaTeX is a typesetting system built on TeX. Knuth developed TeX and Lamport wrapped LaTeX around it, both towering figures in computing. But famous authors are not a reason to learn it. What separates it from WYSIWYG software like Word is the division of labor: you write the content and the system handles typesetting. Heading levels, figure numbering, formula spacing, and bibliography formatting are all governed by style rules, so someone with no typesetting experience can still produce professionally laid out documents.

That trait shows most clearly in long documents. By the hundredth page, manual formatting costs rise exponentially, whereas LaTeX keeps every new section consistent with the style defined at the start, with numbering and tables of contents updating automatically. Mathematics is its traditional strength, and complex fractions, matrices, and multiple subscripts are naturally easier to write than in any GUI. Christos Papadimitriou of Berkeley put it semi-jokingly: every time I read a LaTeX document, I think, wow, this must be correct.

The path is fairly clear, and the hard part is at the start. Environment setup is the first blocker, since a local TeX distribution often lacks packages and fonts; an online editor such as Overleaf skips this step and ships plenty of ready templates. Then read two or three systematic tutorials to cover document structure, math, figures, and bibliography, and the rest is consulting the manual while writing for real.

The first pitfall is using LaTeX like Word. Manually adjusting every gap leads into an endless swamp of `\vspace` and `\hspace`; let style rules control layout and look for the right package rather than patching. The second pitfall is dismissing error messages. LaTeX errors often point to the wrong place, and the real cause is usually a few lines earlier, such as a missing `}` or an unclosed environment; start from the first error and comment things out to locate it instead of searching the message verbatim. The third pitfall is obsessing over the local environment. Spending a whole day configuring without writing a word is the most common waste; write in an online tool first and return to the local setup later if needed.

## Course Resources

- Course Website: <https://www.latex-project.org/>
- Textbooks: Read *The Not So Short Introduction to LaTeX2e* (lshort-zh-cn, translated by the CTEX team); Liu Haiyang's *LaTeX Beginner's Guide* works well as a reference to consult on demand, skipping the CTEX suite chapters
- Recordings: *Modern LaTeX Introduction Lectures* can serve as a supplement
- Assignments: No standardized assignments; use it to write a course assignment or reading report

## Personal Resources

For installation, *A Short Introduction to Installing LaTeX* and the *TeX Live Guide* get the distribution and editor set up. For writing, Overleaf offers plenty of templates and removes the configuration burden. The way to really learn it is to write one genuinely long document: start from a math assignment, then add figures, cross-references, and bibliography, and finally handle the title page and appendix; one full pass is usually enough.
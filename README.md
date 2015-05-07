Little Books
===============



Materials for the Project MOSAIC "Little Books" 

### Compiling

Each book is in a separate directory and the "master" file for each is identified below.  Compiling (Knit PDF) the master file should produce the PDF.

Each of the component `.Rnw` files in these directories an also be compiled on it's own.  Just "Knit PDF" in RStudio.  This will create a PDF file containing just a portion of the book.

### The Little Books

This project consists of several short books that are inter-related.

 1. Start Teaching Statistics with R
 
    Directory: `Starting`
    Master: `MOSAIC-Starting.Rnw`
    
 2. A Compendium of Commands to Teach Statistics with R

    Directory: `Compendium`
    Master: `MOSAIC-Compendium.Rnw`
    
 3. Simulation-Based Inference
 
    Directory: `Simulation`
    Master: `MOSAIC-SimulattionBased.Rnw`
    
 4. Start with Modeling
 
    Directory: `Modeling` or `ModelingV2`
    Master: `MOSAIC-Modeling.Rnw`
    
 5. Start R in Calculus
 
    This is maintained elsewhere
    
APPENDICES

Appendix A: Style Instructions for Authors
=======================


Notes for the authors can be included using `\authNote{A note to the authors.}`

Processed notes for the authors can be hidden using `\authNoted{A noted note to the authors.}`

## Some Style Guidelines

1. R Code
    1. Use space after comma in argument lists 
    2. No space around = in argument list
    3. Use space around operators, `<-` and `->`
    4. Casual comments (no need for caps)
    5. When referring to functions in the text, add empty parens (e.g., `data()`) to make it clear that the object is a function.
2. Exercises
    N.B. Some exercises are for instructors, not for students.
    1. Use `\begin{problem} ... \end{problem}` to define problems.
    2. Use `\begin{solution} ... \end{solution}` to define solutions.

This must be \emph{outside} the `problem` environment and before the definition of the next problem.  Put it immediately after `\end{problem}` to avoid confusion.

* Use `\shipoutProblems` to display all problems queued up since the last `shipoutProblems`.
* Examples
    Put within  `\begin{example}` and `end{example}`.  We can tweak the formatting later.

* Marginal Notes
    We can place some marginal notes with:
    * `\InstructorNote{This is an instructor note.}`
    * `\FoodForThought{We can tweak the layout, color, size, etc. later.  For now. I'm just using color to distinguish.}`
    * `\Caution{This is a caution}`


1. Variable names.  Often it's nice to distinguish between anactual variable name and a word that might have a similar name, for instance between sex and `sex`.  Use the `\VN{sex}` command to accomplish this.
1. Model formulas.  Use `\model{A}{B+C}` to generate `A ~ B+C` .  Often, you may want to use variable names, for instance `\model{\VN{height}}{\VN{age}+\VN{sex}}` gives `height ~ age + sex`.
 




Appendix B: Possible Additional Topics
=====================

*This list is quite old now...*

Do we want to include any of these topics?

* Fancier Lattice Graphics
* Base Graphics
* Making plots with `ggplots2`
* Writing executable R scripts
* R Infrastructure for Teaching
* Sharing in R Studio
* Public Data
* Google Data
* Making Data Available Online
* A Brief Tour of knitr and R-markdown
* exams
* Books
    * Our books
    * Chance et al (in progress)
    * Existing books that work well/poorly with R (and why)
* Online materials

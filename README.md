## Notes and writing
This contains some notes I have written up in TeX over the last little while. Each folder (with one exception) corresponds to one topic.



### The style file
To compile/edit the notes, of course, you'll need [LaTeX](https://www.latex-project.org/get/). However, my later notes rely on a style file (`jack.sty`) found in the outlying folder that needs to be put in an appropriate directory. Windows users should follow [this](https://tex.stackexchange.com/a/1138/269697) and Linux/Unix users should follow [this](https://tex.stackexchange.com/a/10256/269697) to ensure it is put in the right place. 

I also use my style file to write professional-looking notes for courses among other things (book annotations, assignments, etc.). Feel free to try it out. Hopefully, the contents of the `.sty` file are enough to get the gist of what's going on. If not, you start by writing
```tex
\usepackage [course] {jack}
```
in your preamble. This is best used without `\usepackage`ing anything else, since it includes many packages on its own and clashes are likely. You are able to remove some of the `\RequirePackage` invocations in the style file, but that might cause a different error. Let me know if it does. You also have to `\def` a `\jtitle`, `\jlecturer`, `\jauthor`, and `\jterm` in your preamble (before `\usepackage [course] {jack}`) according to the course you're taking (as stated in the `.sty` file). (All of this applies if you choose the `course` option.)

By the way, I use a Vim setup on a theme of [Gilles Castel](https://castel.dev/post/lecture-notes-1/) to write my notes (in class, etc.). I recommend it. I have pushed the `tex.snippets` file that I use.



Please inform me about any errors in the notes or otherwise with an issue. One should note that my LaTeX practices were (and, to some extent, still are) dodgy. Be forewarned.

Thank you to Dr. Richard Borcherds, Khan Academy, and Dr. Benedict Gross for providing me with most of the content of these notes and, particularly, teaching me. 

I am working on some lengthy notes on algebraic geometry that I hope to complete by the fall of 2022. 

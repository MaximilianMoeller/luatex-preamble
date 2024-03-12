# LuaLaTeX Preamble
My personal LuaLatex Preamble.

## Getting Started

### Add the preamble to your project
Include these preamble files into your LuaLaTeX Project by `git submodule add git@github.com:MaximilianMoeller/luatex-preamble.git`.
All preamble files assume the following directory structure of your project:
```
tex root directory/
|– main.tex
|– main.tex.latexmain
|– references.bib
|– sections/
|   |– Introduction.tex
|   |– …
|– preamble/
|   |– 01-mandatory.tex
|   |– …
```

### Using it

Your `main.tex` file should then look something like this:
```
%!TEX TS-program = lualatex

\documentclass[…]{…}

% Mix and match whatever you need

% This part of the preamble is indispensable for this template to work.
\input{preamble/01-mandatory.tex}
\input{preamble/02-language-english.tex}
%\input{preamble/02-language-german.tex}
\input{preamble/03-typography.tex}
\input{preamble/04-improvements.tex}
\input{preamble/20-math.tex}
\input{preamble/21-theorems.tex}
\input{preamble/25-complexity-classes.tex}
\input{preamble/30-algorithms.tex}
\input{preamble/99-references.tex}

% other, project specific preamble settings

\begin{document}
% your document content goes here
\end{document}
```

## Copyright and Licensing
Unless stated otherwise, all documents in this project are licensed under the [Creative Commons License](https://creativecommons.org/licenses/by/4.0/).
You are thereby free to share and adapt their contents for any purpose, even comercially under the condition that you include the following attribution:

> (C) Maximilian Moeller, https://github.com/MaximilianMoeller/luatex-preamble, CC BY 4.0 Deed 

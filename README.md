<div id="table-of-contents">
<h2>Table of Contents</h2>
<div id="text-table-of-contents">
<ul>
<li><a href="#sec-1">1. Installation</a></li>
<li><a href="#sec-2">2. Compilation</a></li>
<li><a href="#sec-3">3. Options</a></li>
<li><a href="#sec-4">4. Example deck</a></li>
<li><a href="#sec-5">5. Where to get help</a></li>
<li><a href="#sec-6">6. Reporting bugs and feature requests</a></li>
</ul>
</div>
</div>
# Installation

1.  Install MacTeX 2013 from [MacTeX](https://tug.org/mactex/)

2.  Install the Python package `pygments` by typing `$ pip install pygments` in your shell

3.  Symlink this repo to `~/texmf/tex/latex/` (using `$ ln -s beamer_pivotal ~/texmf/tex/latex/`, create the folders if they don't exist) and then run `$ texconfig rehash` in your shell

# Compilation

Use the following command to compile the source file to a pdf (i.e. set your editor to use that command): `$ latexmk -pdflatex='lualatex --shell-escape' -pdf example.tex`

# Options

For the time being, the only option is the (currently English or German).
Use `\documentclass[english]{pivotalbeamer}` to set it. If you require further options, please submit a feature request, or (optimally) implement the option yourself.

# Example deck

The file `example.tex` contains an examplary deck. See [example.pdf](https://github.com/gopivotal/beamer_pivotal/blob/master/example.pdf?raw=true) for the compiled version.

# Where to get help

-   Type `$ texdoc beamer` at your command line to open the comprehensive Beamer User Guide. [TeX - LaTeX Stack Exchange](https://tex.stackexchange.com/) also has a lot of material.

# Reporting bugs and feature requests

If you find a bug, please use the bug tracker and submit your complete source code and the LuaLaTeX output containing the error message. Also use the tracker for feature requests.

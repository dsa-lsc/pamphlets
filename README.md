# Pamphlets for printing!

[2019 Convention Platform](2019-convention-platform/lsc-2019-platform.md)

[Dual Power: A Strategy to Build Socialism in Our Time](dual-power/dual-power.md)

Instructions for adding a pamphlet to the repo:
1. Create a new directory in the repository.
2. Copy the markdown from the website into the repo.
3. Use pandoc to generate LaTeX, e.g: `pandoc -t latex -f markdown -o dual-power.tex dual-power.md`
4. Copy over the boilerplate LaTeX document header & footer from one of the existing .tex files.
5. Proof the document and tweak formatting as needed, using a LaTeX editor like TeXmaker
6. If you want to format as a booklet, create a *name*-booklet.tex file, copied from one of the existing files, and replacing the filename of the pdf. If you *don't* want to create a booklet, remove the `\usepackage{geometry}` command, and consider increasing the font size to 11pt or 12pt in the `\documentclass` command.

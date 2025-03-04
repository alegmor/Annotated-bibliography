# Annotated Bibliography in Harvard Style (LaTeX)

## Overview

This repository contains the necessary files to create an annotated bibliography in Harvard style using LaTeX. The bibliography is formatted using the agsm-annot.bst bibliography style file, which supports annotations.

## Files in the Repository

main.tex – The main LaTeX document that includes the bibliography.

test.bib – The bibliography file containing references, including annotations.

agsm-annot.bst – The custom bibliography style file that formats references in Harvard style with annotations.

## How to Use

## 1. Compile the LaTeX Document

To generate the annotated bibliography, follow these steps:

Compile main.tex using pdflatex:

pdflatex main.tex

Run BibTeX to process the bibliography:

bibtex main

Compile pdflatex twice more to ensure all references and citations are updated:

pdflatex main.tex
pdflatex main.tex

The output will be a PDF file containing the annotated bibliography.

## 2. Adding Annotations to References

Annotations are added within the test.bib file using the annotate field. Example entry:

@article{example2025,
  author = {Doe, John},
  title = {An Example Article},
  journal = {Journal of Examples},
  year = {2025},
  volume = {10},
  number = {2},
  pages = {100-110},
  annotate = {This article discusses the fundamentals of using annotated bibliographies in LaTeX.}
}

The annotate field is processed by the agsm-annot.bst file, ensuring that annotations appear correctly formatted in the final bibliography.

## Dependencies

Ensure you have the following installed:

A LaTeX distribution (e.g., TeX Live, MiKTeX)

A LaTeX editor (e.g., Overleaf, TeXworks, VS Code with LaTeX Workshop)

## Notes

If the annotations are not appearing, verify that agsm-annot.bst is correctly referenced in main.tex.

The .bib file must include an annotate field for each reference to display annotations.

## License

This repository is free to use and modify. Feel free to contribute improvements!

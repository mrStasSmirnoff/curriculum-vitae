# Curriculum Vitae

This repository contains my CV in Markdown format and instructions on how to generate the PDF version using Pandoc with specific formatting settings.

## Generating the PDF

To convert the Markdown file `cv_Smirnov_2024.md` to a PDF with the desired font, font size, and margins, use the following Pandoc command:

```bash
pandoc cv_Smirnov_2024.md -o cv_Smirnov_2024.pdf \
    --pdf-engine=xelatex \
    -V geometry:margin=0.6in \
    -V fontsize=10pt \
    -V mainfont="Helvetica" \
    --metadata=link-citations=true

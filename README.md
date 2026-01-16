# LaTeX Thesis Template

Here's the LaTeX thesis template I used for my master's thesis. It's simple to use, but you can customize it however you want. I've added a basic outline that I used to write my draft (the content will of course depend on your research topic). I used VS Code as my main editor combined with the LaTeX Workshop extension. You can find a tutorial for installing the LaTeX extension in my blog post: https://almira.argarin.dev/post/how-i-organized-my-research-project.

## Structure

```
├── main.tex              # Main document file
├── abstract.tex          # Abstract section
├── acknowledgements.tex  # Acknowledgements section
├── references.bib        # Bibliography file
├── chapters/
│   ├── chap1.tex        # Introduction
│   ├── chap2.tex        # Literature Review
│   ├── chap3.tex        # Methodology
│   ├── chap4.tex        # Experiments
│   ├── chap5.tex        # Discussion
│   ├── chap6.tex        # Limitations
│   └── chap7.tex        # Conclusion
```

## Compilation

To compile the thesis:

```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

Or use your LaTeX editor's build command (e.g., in TeXstudio, Overleaf, or VS Code with LaTeX Workshop).

## Customization

1. Edit title page information in `main.tex`
2. Modify chapter content in `chapters/` directory
3. Add references to `references.bib`
4. Adjust formatting and packages as needed

## Requirements

- LaTeX distribution (TeX Live, MiKTeX, or MacTeX)
- Required packages: inputenc, geometry, graphicx, amsmath, hyperref, setspace, natbib

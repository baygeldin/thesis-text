# Graduation Thesis
This repository contains LaTeX sources of my graduation thesis. The implementation can be found [here](https://github.com/baygeldin/StressDetectionKit).

In order to setup a **perfect** local environment via Spacemacs:

1) Install TeX Live along with cyrillic languages package and make sure that XeTeX is included (e.g. on Ubuntu it's `texlive-xetex` and `texlive-lang-cyrillic` packages).
2) Add `latex` and `bibtex` layers to `.spacemacs`:

```elisp
(latex :variables latex-build-command "LaTeX")
bibtex
```

3) Set TeX engine to XeTeX in `.spacemacs`:

```elisp
(setq TeX-engine 'xetex)
```

4) `SPC m b` or `, b` to build the document.
5) `SPC m v` or `, v` to view the document.
6) `, ,` and choose `BibTeX` to build bibliography (or `SPC SPC` to open `M-x` commands, choose `TeX-command-master` and then `BibTeX`). If citations are not rendered, build the document multiple times.
7) *PROFIT!*

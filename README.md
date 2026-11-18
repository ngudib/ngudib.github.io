# ngudib.github.io

Personal academic website of Nishwanth Gudibandla, served by GitHub Pages at https://ngudib.github.io.

Plain static HTML/CSS, no build step (`.nojekyll` tells Pages to serve files as-is).

| Path | Page |
| --- | --- |
| `index.html` | About, news, selected publications |
| `publications/` | Publications |
| `research/` | Research projects |
| `cv/` | CV (embedded PDF + download) |
| `teaching/` | Teaching |
| `mentoring/` | Mentoring & service |
| `assets/` | CSS, JS, profile photo, CV PDF |
| `cv-source/cv.tex` | LaTeX source for the CV |

## Updating the CV

```sh
cd cv-source
pdflatex cv.tex && pdflatex cv.tex
cp cv.pdf ../assets/pdf/Gudibandla_CV.pdf
```

## Preview locally

```sh
python -m http.server 8000   # then open http://localhost:8000
```

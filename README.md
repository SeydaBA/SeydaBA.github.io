# SeydaBA.github.io

Personal website of Seyda Betul Aydin, built with [al-folio](https://github.com/alshedivat/al-folio) (a Jekyll theme for academics) and hosted on GitHub Pages at <https://seydaba.github.io>.

## Where to edit things

| What | Where |
| --- | --- |
| Home page text and subtitle | `_pages/about.md` |
| Profile photo | `assets/img/prof_pic.jpg` (keep the file name, or change `profile.image` in `_pages/about.md`) |
| Name, site description, keywords | top of `_config.yml` |
| Contact icons (email, and GitHub, LinkedIn, Scholar, ORCID if you add them) | `_data/socials.yml` |
| CV page (experience, education, training, skills, ...) | `_data/cv.yml` |
| Publications | `_bibliography/papers.bib` (one BibTeX entry per paper) |
| Co-author links on publications | `_data/coauthors.yml` |
| Talks | `_pages/talks.md` |
| Teaching | `_pages/teaching.md` |
| Projects | one file per project in `_projects/` |
| Menu order | `nav_order` at the top of each page in `_pages/` |

## Preview on your computer (optional)

With [Docker](https://www.docker.com/) installed, run `docker compose up` in this folder and open <http://localhost:8080>. The page reloads when you save a file.

## Publishing

Pushing to `main` (or `master`) runs the "Deploy site" workflow in `.github/workflows/deploy.yml`, which builds the site and writes the result to a branch called `gh-pages`. A pull request runs the same build without publishing, so you can check it before merging.

One-time GitHub settings:

1. Settings → Actions → General → Workflow permissions → **Read and write permissions**.
2. After the first workflow run has created `gh-pages`: Settings → Pages → Source **Deploy from a branch** → branch `gh-pages`, folder `/ (root)`.

More options (blog, news, comments, themes) are described in the [al-folio documentation](https://github.com/alshedivat/al-folio#readme).

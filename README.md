# Xi Zhong — Academic Homepage

Source for **https://xi-zhong-ece.github.io**, built with the [al-folio](https://github.com/alshedivat/al-folio) Jekyll theme.

## Where things live

| What | File |
| --- | --- |
| Homepage bio & photo settings | `_pages/about.md` |
| Publications | `_bibliography/papers.bib` (`selected = {true}` shows a paper on the homepage) |
| Full CV page | `_data/cv.yml` |
| CV PDF (download button) | `assets/pdf/Xi_Zhong_CV.pdf` |
| Teaching page | `_pages/teaching.md` and `_teachings/*.md` |
| News items | `_news/YYYY-MM-DD-name.md` |
| Email / Scholar / ORCID / GitHub icons | `_data/socials.yml` |
| Venue badge colors | `_data/venues.yml` |
| Site title, URL, footer, etc. | `_config.yml` |
| Profile photo | `assets/img/prof_pic.jpg` |

Every push to `main` triggers `.github/workflows/deploy.yml`, which builds the site and publishes it to the `gh-pages` branch. See `DEPLOY.md` for first-time setup.

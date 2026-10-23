# Tailai Chen's homepage

Personal academic homepage, served by GitHub Pages at https://shanoal.github.io/tailor/
(built with the [Academic Pages](https://github.com/academicpages/academicpages.github.io) Jekyll template).

- Profile, sidebar and links: `_config.yml`
- Home page: `_pages/about.md`; CV: `_pages/cv.md`
- Publications: one Markdown file per paper in `_publications/`, grouped by `category`
  (`published`, `preprints` or `reports`, defined under `publication_category` in `_config.yml`), e.g.

  ```yaml
  ---
  title: "Paper title"
  collection: publications
  category: published        # published | preprints | reports
  permalink: /publication/2026-paper-slug
  date: 2026-06-01
  venue: "CVPR 2026"
  paperurl: "https://arxiv.org/abs/xxxx.xxxxx"
  citation: "A. Author, <b>T. Chen</b>, ... (2026). Paper title. <i>CVPR</i>."
  ---
  ```
- Header menu: `_data/navigation.yml`

If the repository is renamed to `SHANOAL.github.io`, set `baseurl: ""` in `_config.yml` and the site moves to https://shanoal.github.io/.

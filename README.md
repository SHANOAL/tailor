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
  badge: "CVPR 2026"         # label shown on the thumbnail
  thumbnail: "publications/paper-slug.jpg"   # under images/, ~640 px wide JPEG
  selected: true             # also list it under Selected Publications on the home page
  link: "https://arxiv.org/abs/xxxx.xxxxx"   # where the title and thumbnail point
  authors: "A. Author, <b>Tailai Chen</b>, B. Author"
  excerpt: "One- or two-sentence summary shown on the card."
  links:                     # buttons; icons from Font Awesome 6 / Academicons
    - name: "arXiv"
      url: "https://arxiv.org/abs/xxxx.xxxxx"
      icon: "ai ai-arxiv"
    - name: "Code"
      url: "https://github.com/..."
      icon: "fab fa-github"
  ---
  ```

  Each entry is rendered as a card (`_includes/publication-card.html`, styles in
  `_sass/layout/_publications.scss`); the body of the file (abstract, figures) becomes the paper's own page.
- Header menu: `_data/navigation.yml`

If the repository is renamed to `SHANOAL.github.io`, set `baseurl: ""` in `_config.yml` and the site moves to https://shanoal.github.io/.

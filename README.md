## Agentic Search Tutorial

Jekyll site for the agentic search tutorial series (same structure as convsearch.github.io).

- Each edition has its own page, e.g. `cikm2026.md` -> `/cikm2026/`.
- Edition content lives in `_includes/summary-<edition>.html`, `_includes/schedule-<edition>.html`,
  `_includes/organiser-<edition>.html`, `_includes/contact-<edition>.html`, and organisers in `_<edition>_organisers/`.
- The site root redirects to the latest edition, set by `latest_edition` in `_config.yml`.
- To add an edition (e.g. WSDM 2027): copy the four include files and the organiser folder with the new edition name,
  add the collection to `_config.yml`, add an `elsif` branch in `_layouts/home.html`, add `<edition>.md` with its permalink,
  add it to the Editions menu in `_includes/nav-bar.html`, and update `latest_edition` in `_config.yml`.
- Local preview: `bundle install && bundle exec jekyll serve`.

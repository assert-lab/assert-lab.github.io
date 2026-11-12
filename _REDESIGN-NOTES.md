# AS²ERT Lab redesign: install notes

1. Copy everything in this zip over your repo (same folder structure; overwrite when asked).
2. Delete these files from the repo:
   - `index.html`  (duplicate of index.md; both build to the homepage)
   - `gallery.md`  (duplicate permalink with proposal.md)
3. Optional cleanup, now unused: `docs/`, `test/`, `_sass/`, `assets/js/`, `CHANGELOG.md`,
   `minimal-mistakes-jekyll.gemspec`, `package.json`, `Rakefile`, `staticman.yml`,
   and the old theme files in `_includes/` and `_layouts/` (anything not named
   site-*.html, page-head.html, default.html, page.html).
4. Push, then check the GitHub Pages build under Actions.

Where to edit things
- News:          `_data/news.yml`  (newest first; homepage shows the top 4)
- Publications:  `_data/publications.yml`
- Navigation:    `_data/navigation.yml`
- Email, PI name: `_config.yml` (`email`, `pi_name`)
- Colours/fonts: top of `assets/css/main.scss`
- Homepage code snippet is decorative: delete the `hero-figure` block in `index.md` to remove it.

Things to verify in your content
- TOGBench / PITMuS GitHub links differ between homepage and Publications page.
- ICSE-DS poster link points to /assets/presentations/..., which is not in the repo.
- Tasfia is not on the People page; Alumni section was empty (placeholder comment left).
- Grace Hopper award: 2026 (PI page) vs Dec 2025 (news).
- Gallery photos are 2-4 MB each; resizing would speed those pages up.

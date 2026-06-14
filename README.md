# My Blog

A simple Jekyll blog ready for GitHub Pages, with a homepage (blog post list) plus About, Projects, and Contact pages that appear as nav links you can toggle between.

## Setup

1. Create a new GitHub repo named `<yourusername>.github.io` (or any name for a project site).
2. Push these files to it.
3. In repo Settings → Pages, set source to the `main` branch (root).
4. Your site will be live at `https://<yourusername>.github.io` within a minute or two.

## Local preview (optional)

```
gem install bundler jekyll
bundle install
bundle exec jekyll serve
```
Visit http://localhost:4000

## Adding content

- New blog posts: add files to `_posts/` named `YYYY-MM-DD-title.md`.
- New pages: add a `.md` file at the root with front matter like:
  ```
  ---
  layout: page
  title: My Page
  permalink: /mypage/
  ---
  ```
  Then add the filename to `header_pages` in `_config.yml` so it shows in the nav.

## Customizing

- Edit `_config.yml` for site title/description.
- Edit `assets/css/style.scss` for styling.
- Swap `theme: minima` for another Jekyll theme if you want a different look.

# Evgenia Galytska — academic website

An editable academic profile site built with Markdown and Jekyll for GitHub Pages. The website source contains no hand-written HTML pages; GitHub Actions builds the Markdown into the rendered site.

## Edit the content

- `index.md` — home page
- `about.md` — short biography
- `research.md` — research themes
- `publications.md` — selected publications
- `experience.md` — experience
- `community.md` — community work
- `awards.md` — awards and recognition
- `contact.md` — contact details
- `_config.yml` — site title, description, theme, and navigation

## Publish using GitHub Pages

1. Create a repository named `<your-github-username>.github.io` for a personal site.
2. Upload the contents of this folder to the repository root, on the `main` branch.
3. In `_config.yml`, replace `<your-github-username>` with your GitHub username.
4. In the repository, open **Settings → Pages** and set the build and deployment source to **GitHub Actions**.
5. The included workflow in `.github/workflows/pages.yml` publishes the site after each push to `main`. The first build may take a few minutes.

You can also use a repository with another name, but then configure `baseurl` in `_config.yml` as `/<repository-name>` and use the project Pages address.

## Preview locally (optional)

Install Ruby and Bundler, then run:

```bash
bundle install
bundle exec jekyll serve
```

Open the local address printed by Jekyll.

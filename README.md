# Jerry Chen's Blog

This repository is a Jekyll site published automatically by GitHub Pages. Pages and posts are authored in Markdown; generated HTML should not be committed.

## Add a new post

1. Create a file in `_posts` named `YYYY-MM-DD-short-title.md`.
2. Start it with this front matter:

   ```yaml
   ---
   layout: post
   title: My Post Title
   date: 2026-06-27 12:00:00 +0800
   categories:
     - Physics
   tags:
     - example
   ---
   ```

3. Write the post below the front matter using Markdown.
4. Commit and push the file to the publishing branch. GitHub Pages builds and publishes it automatically.

Use one of the homepage categories exactly as written: `Physics`, `Computer Science`, `Numerical Methods`, `Books`, or `Journal`. The category cards and post counts update automatically. Category names and descriptions live in `_data/categories.yml`.

Images can be stored under `images/`. Reference them from Markdown with an absolute site path:

```markdown
![Description](/images/example.png)
```

## Edit a page

- Edit `about.md` for the About page.
- Edit `index.md` for the home page introduction.
- Edit `_config.yml` for the site title, description, navigation, or permalink defaults.

## Preview locally (optional)

Install Ruby and Bundler, then run:

```shell
bundle install
bundle exec jekyll serve
```

Open <http://localhost:4000>.

# dsnp-web
This site uses jekyll with GitHub Pages; see https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll for setup and usage.

## Adding new blog posts

Create new blog posts as markdown files under `blog/_posts` using a `YYYY-MM-DD-` prefix.
The following front matter keys are used:
- `title`
- `author` (optional)
- `blurb` (optional; shows on the blog index with a "Read more..." link)

## Layout templates in use
- `_layouts/basic.html` is the core site template (fonts and CSS)
- `_layouts/default.html` includes the side navigation
- `_layouts/home.html` is the blog index
- `_layouts/post.html` is the blog post template

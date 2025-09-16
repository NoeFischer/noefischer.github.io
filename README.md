# Bear Blog for GitHub Pages

This repository contains a lightweight static blog inspired by the [Bear Blog](https://bearblog.dev) aesthetic. Everything is written in plain HTML and CSS so you can deploy it anywhere, including GitHub Pages.

## Structure

```
.
├── index.html          # Landing page with featured posts
├── about.html          # Personal bio page
├── posts/
│   ├── index.html      # List of all posts
│   ├── slow-internet.html
│   └── morning-trails.html
├── assets/
│   └── styles.css      # Shared styles for the site
└── 404.html            # Custom not-found page for GitHub Pages
```

## Add a new post

1. Duplicate one of the files in `posts/` and rename it to match your new slug, e.g. `posts/gentle-interfaces.html`.
2. Update the `<title>`, `<h1>`, `<time>` element, and the article body.
3. Link your new post from `posts/index.html` (and optionally the home page) by adding another `<article>` block with the new metadata.
4. Commit and push your changes.

## Preview locally

You can open any of the `.html` files directly in your browser. If you prefer a local server, run:

```bash
python3 -m http.server
```

…and then visit <http://localhost:8000>.

## Deploy on GitHub Pages

1. Rename the repository to `<username>.github.io` (or configure Pages to serve from the `main` branch) in your GitHub account.
2. Push the contents of this directory to the repository.
3. In the repository settings, enable GitHub Pages for the `main` branch (or the `/docs` folder if you move the files later).
4. Wait a minute for the site to build, then visit `https://<username>.github.io/`.

Feel free to customize the colors, typography, and layout in `assets/styles.css`. Because the site is static, it stays fast, accessible, and easy to maintain.

# Portfolio

Single-file portfolio site. No build step, no dependencies — `index.html` contains the markup, styles, and script.

## Put it on GitHub Pages

1. Create a repo. Name it `yourusername.github.io` to get `https://yourusername.github.io`, or use any name to get `https://yourusername.github.io/reponame`.
2. Commit `index.html` at the root of the repo and push.
3. In the repo, go to **Settings → Pages**, set **Source** to *Deploy from a branch*, branch `main`, folder `/ (root)`, and save.
4. Wait about a minute, then load the URL Pages shows you.

Updates go live on every push to `main`.

## What to edit

Everything you need to change is marked in a comment block at the top of `index.html`:

- `<title>` and the two `<meta>` description tags
- Hero: name, the line under it, location and availability
- Work: one `<a class="entry">` block per project — copy or delete blocks freely
- About: the paragraphs and the three toolkit lists
- Contact: your email, which appears in the `href` and as the visible text
- Any `href="#"` is a placeholder that needs a real URL

## Changing the colors

All colors are CSS variables in the `:root` block near the top of the `<style>` tag. Swap `--aqua` for any accent and the whole page follows.

## Custom domain

Add a file named `CNAME` at the repo root containing just your domain (e.g. `sam.dev`), then point a CNAME DNS record at `yourusername.github.io`.

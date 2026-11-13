# litelogin-website

The landing page for [LiteLogin](https://github.com/litelogin/litelogin), served by GitHub Pages.

Plain HTML and CSS, with no build step:

- `index.html`: the page
- `style.css`: styles, with light and dark themes from `prefers-color-scheme`
- `logo.png`: the logo (400×400); `favicon.png` and `apple-touch-icon.png` are resized copies
- `.nojekyll`: tells GitHub Pages to serve the files as they are

## Preview locally

```sh
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

## Publish

1. Push to `https://github.com/litelogin/website`. GitHub Pages serves it at `https://litelogin.github.io/website/` (every link on the page is relative, so the subpath works).
2. In the repository's **Settings → Pages**, set the source to **Deploy from a branch**, branch `main`, folder `/ (root)`.
3. For a custom domain, add a `CNAME` file containing the domain (for example `litelogin.dev`) and set the DNS records GitHub describes.
4. Set the main repository's **Website** field to the page's URL.

## Keeping it accurate

The numbers on the page come from the main repository: costs from `Cost.md`, latencies from `test/load/README.md`, features from `README.md`. Update them here when those change.

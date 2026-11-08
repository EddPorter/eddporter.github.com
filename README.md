# eddporter.com

Source for my personal homepage, published at <https://eddporter.com/> with GitHub Pages. The old address, `eddporter.github.io`, redirects there.

## How it works

The site is plain HTML and CSS with no build step. An empty `.nojekyll` file stops GitHub Pages running Jekyll over it. Pushing to `master` publishes the change.

| Path | What it is |
| --- | --- |
| `index.html` | The homepage |
| `CNAME` | Tells GitHub Pages the custom domain, `eddporter.com` |
| `css/main.css` | Its styles |
| `projects.html`, `tools.html`, `enterprise.txt` | Old notes from 2012, still published but not linked from the homepage |
| `images/bgimg.jpg` | The old background image, no longer used |

The project sites linked from the homepage (Slider, Bezique, GeneCodeCS and tsuikyuu) live in their own repositories and are served by GitHub Pages under `eddporter.com/<repository>/`.

The repository is still named `eddporter.github.com`, but the site is served at `eddporter.com`.

## Previewing locally

The stylesheet is referenced with an absolute path, so serve the repository root:

```sh
python3 -m http.server 8000
```

Then open <http://localhost:8000/>.

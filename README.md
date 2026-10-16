# Arcade

The published arcade games, served with GitHub Pages: a start page (`index.html`) and one folder per game with its full-screen page and its built bundle.

| Folder | Game | Built from |
|---|---|---|
| `perseids/` | PERSEIDS, a fixed shooter | `npm run build:site` in the PERSEIDS project (copies `site/index.html` and `dist/embed/perseids.js` here) |

Only built files live here; the sources stay in the games' own repositories. Nothing needs building: GitHub Pages serves the files as they are (`.nojekyll` turns off Jekyll).

# Arcade

The published arcade games, served with GitHub Pages: a start page (`index.html`) and one folder per game with its full-screen page and its built bundle.

| Folder | Game | Built from |
|---|---|---|
| `perseids/` | PERSEIDS, a fixed shooter | `npm run build:site` in the PERSEIDS project (copies `site/index.html` and `dist/embed/perseids.js` here) |
| `perseids/test/` | PERSEIDS with test keys, linked from the start page as test mode | `npm run build:site`, same as above |
| `orbit/1982/` | ORBIT 1982, an experiment: the arcade as a Bildschirmtext page (noindex) | `npm run build:orbit` in the PERSEIDS project (copies `website/orbit-1982-v3.html` here) |
| `orbit/konzept/` | ORBIT concept, encrypted; the page asks for a password and decrypts in the browser | `npm run build:orbit` in the PERSEIDS project, only with `ORBIT_CONCEPT_PASSWORD` set |
| `orbit/aufgaben/` | ORBIT task board for the team (noindex); the page asks for the concept password and loads tasks and comments from the score server | `npm run build:orbit` in the PERSEIDS project |

Only built files live here; the sources stay in the games' own repositories. Nothing needs building: GitHub Pages serves the files as they are (`.nojekyll` turns off Jekyll).

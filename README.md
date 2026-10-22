# Arcade

The published arcade games, served with GitHub Pages: a start page (`index.html`) and one folder per game with its full-screen page.

| Folder | Content | Built from |
|---|---|---|
| `index.html` | Start page: ARCADE, the ORBIT menu, „Coming soon“ | edited here |
| `prototypes/` | Prototypes page with cards for HOPROD, PERSEIDS and the ORBIT hall, locked | `npm run build:orbit` in the ORBIT repo (`website/prototypes.html`), only with `ORBIT_CONCEPT_PASSWORD` set |
| `perseids/`, `perseids/test/` | PERSEIDS, a fixed shooter, and the same with test mode; locked | `npm run build:site` in the ORBIT repo |
| `orbit/halle/`, `orbit/halle/test/` | ORBIT hall, a walkable arcade hall, and the same with test menu; locked | `npm run build:site -w hall` in the ORBIT repo |
| `hoprod/` | HOPROD, a top-down car game; locked | `npm run deploy` in the HOPROD repo |
| `orbit/1982/` | ORBIT 1982, an experiment: the arcade as a Bildschirmtext page (noindex) | `npm run build:orbit` in the ORBIT repo (`website/orbit-1982-v3.html`) |
| `orbit/aufgaben/` | ORBIT task board for the team (noindex); the page asks for the concept password and loads tasks and comments from the score server | `npm run build:orbit` in the ORBIT repo |
| `orbit/konzept/`, `orbit/design/` | ORBIT concept and design decisions, locked | `npm run build:orbit` in the ORBIT repo, only with `ORBIT_CONCEPT_PASSWORD` set |

Locked pages hold only ciphertext: the page asks for the password and decrypts in the browser, together with the game's code (`scripts/lock.mjs` in the ORBIT repo). After one login the browser remembers the key (`arcade.unlock`) and opens every locked page without asking.

Only built files live here; the sources stay in the games' own repositories. Nothing needs building: GitHub Pages serves the files as they are (`.nojekyll` turns off Jekyll).

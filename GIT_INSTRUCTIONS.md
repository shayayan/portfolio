# Portfolio Setup & Git Instructions

Three repos on GitHub account **shayayan**: the portfolio site itself, and two separate
repos for the heavier academic projects (kept out of the portfolio repo so it stays light).

## 1. Portfolio (this directory → `shayayan/portfolio`)

```bash
git add index.html CV_en.pdf reports README.md GIT_INSTRUCTIONS.md .gitignore
git commit -m "fix: correct github username, add CV download, drop marquee, fix report links"
git push -u origin main
```

Then enable GitHub Pages: repo **Settings → Pages → Source: Deploy from a branch →
Branch: `main` / `/ (root)`**. The site will be live at `https://shayayan.github.io/portfolio/`.

## 2. Music Generation (`shayayan/music_generation_epfl_dh401`)

A flattened, ready-to-push copy was prepared at
`/tmp/repo-staging/music_generation_epfl_dh401` (already `git init`'d and committed
locally as `main`, since the original zips extracted with a doubled nested folder).

```bash
cd /tmp/repo-staging/music_generation_epfl_dh401
# create the empty repo "music_generation_epfl_dh401" on github.com/shayayan first
git remote add origin https://github.com/shayayan/music_generation_epfl_dh401.git
git push -u origin main
```

## 3. Commune Memoirs (`shayayan/commune_memoirs_epfl_dh412`)

Same situation — flattened copy at `/tmp/repo-staging/commune_memoirs_epfl_dh412`,
already committed locally. Note: this repo is ~103 MB (two `.pkl` files: 70 MB + 15 MB),
under GitHub's 100 MB per-file hard limit but worth knowing before pushing.

```bash
cd /tmp/repo-staging/commune_memoirs_epfl_dh412
# create the empty repo "commune_memoirs_epfl_dh412" on github.com/shayayan first
git remote add origin https://github.com/shayayan/commune_memoirs_epfl_dh412.git
git push -u origin main
```

Note: `/tmp/repo-staging` is temporary — copy it somewhere permanent before pushing if
you're not doing it in this same session.

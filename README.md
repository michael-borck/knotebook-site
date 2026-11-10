# Knotebook site

Built app/player for [Knotebook](https://github.com/michael-borck/Knotebook).

This repo is **generated**: it contains the Vite build of the app, deployed to
GitHub Pages. Do not edit files here by hand.

- App: https://michael-borck.github.io/knotebook-site/
- Player: https://michael-borck.github.io/knotebook-site/?player=1
- Store: https://michael-borck.github.io/knotebook-store/

## Build and publish

From the main repo:

```bash
PAGES_BASE=/knotebook-site/ npm run build
rm -rf ../knotebook-site/assets ../knotebook-site/icons
cp -R dist/. ../knotebook-site/
git -C ../knotebook-site add -A
git -C ../knotebook-site commit -m "deploy"
git -C ../knotebook-site push
```

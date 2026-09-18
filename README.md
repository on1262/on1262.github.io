# Yutong Chen — Academic Website

A responsive academic personal website inspired by [Academic Pages](https://academicpages.github.io/). It is built with plain HTML, CSS, and a few lines of JavaScript, so GitHub Pages can publish it directly without a build step.

## Preview locally

From this folder, run:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Publish at `username.github.io`

1. Create a public GitHub repository named exactly `username.github.io`, replacing `username` with your GitHub username.
2. Upload **the contents of this folder** to the repository root. `index.html` must be visible at the top level, not inside another folder.
3. Open the repository's **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**. Select the `main` branch and `/ (root)`, then save.
5. Wait a few minutes and visit `https://username.github.io/`.

For the likely username in this website's links, the repository would be `on1262.github.io` and the address would be `https://on1262.github.io/`.

## Update content

- Main biography and news: `index.html`
- Publication list: `publications.html`
- Research descriptions: `research.html`
- CV file: replace `files/Yutong_Chen_CV.pdf` with a PDF using the same name
- Profile photo: replace `assets/images/profile.jpg` with an image using the same name
- Colors and layout: `assets/css/main.css`

No third-party analytics, fonts, scripts, or cookies are included.

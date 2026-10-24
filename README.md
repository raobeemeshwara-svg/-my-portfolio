# Utla Beemeshwara Rao | Portfolio

A responsive, static portfolio website (HTML, CSS, vanilla JS). No build step.

## Structure

```
index.html                         main portfolio
resume.html                        premium web resume (also prints to A4)
css/styles.css
js/main.js
assets/
  ns-tax-preview.jpg               project screenshot (clickable)
  Utla-Beemeshwara-Rao-Resume.pdf  downloadable resume
  favicon.svg
vercel.json
```

## Run locally

Open `index.html` in a browser, or run a local server:

```bash
python3 -m http.server 8000
# visit http://localhost:8000
```

## Project preview

The screenshot in `assets/ns-tax-preview.jpg` is wrapped in a link to
https://ns-tax-consultancy.vercel.app/ (opens in a new tab). The whole project card is clickable.
To change the screenshot, replace that file (keep the same name).

## Resume

- `resume.html` is the on-site resume. Visitors can download the PDF from its top bar.
- If you change resume details, edit `resume.html`, then open it in Chrome, press Ctrl/Cmd+P,
  choose "Save as PDF", paper A4, margins None, enable "Background graphics",
  and save over `assets/Utla-Beemeshwara-Rao-Resume.pdf`.

## Upload to GitHub

```bash
git init
git add .
git commit -m "Initial portfolio"
git branch -M main
git remote add origin https://github.com/<your-username>/portfolio.git
git push -u origin main
```

Or on github.com use **Add file > Upload files** and drag in everything from this folder.

## Deploy to Vercel

1. Go to https://vercel.com and sign in with GitHub.
2. **Add New > Project**, import your `portfolio` repository.
3. Framework Preset: `Other`. Leave Build Command and Output Directory empty.
4. Click **Deploy**. Every `git push` redeploys automatically.

## After deploying, check

- The project screenshot loads and clicking it opens the NS Tax Consultancy site in a new tab.
- "View Resume" opens `resume.html`, and "Download PDF" downloads the PDF.
- Email and phone links work on your phone.

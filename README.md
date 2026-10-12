# Sandeep Mourya — portfolio

A single-page portfolio site. No framework and no build step: everything lives in `index.html`.

## Files

| Path | What it is |
| --- | --- |
| `index.html` | The whole site: HTML, CSS and JavaScript in one file |
| `assets/sandeep.jpg` | Profile photo |
| `assets/Sandeep_CV.pdf` | One-page CV, linked from every "Download CV" button |

Preview locally by opening `index.html` in a browser.

## Deploy on Vercel

1. **Put the files on GitHub.** Create a new repository (for example `sandeep-portfolio`).
   - In the browser: on the empty repo page, click **uploading an existing file**, drag in `index.html`, `README.md` and the whole `assets` folder, then **Commit changes**.
   - Or from a terminal inside this folder:
     ```bash
     git init
     git add .
     git commit -m "Portfolio site"
     git branch -M main
     git remote add origin https://github.com/<your-username>/sandeep-portfolio.git
     git push -u origin main
     ```
2. **Import it in Vercel.** On vercel.com choose **Add New → Project**, then import the repository.
3. **Keep the defaults.** Framework Preset: **Other**. Leave Build Command and Output Directory empty. Click **Deploy**.
4. **Share the link** Vercel gives you (for example `sandeep-portfolio.vercel.app`). Every push to `main` redeploys automatically.

## Role-specific links

The site can open already filtered to the work that matters for a role. Add `?role=` to the URL:

- `https://<your-site>.vercel.app/?role=product` for product roles
- `https://<your-site>.vercel.app/?role=data` for data analyst and data scientist roles
- `https://<your-site>.vercel.app/?role=engineering` for engineering roles

## Updating

- **CV:** replace `assets/Sandeep_CV.pdf` with a new file of the same name.
- **Photo:** replace `assets/sandeep.jpg` (a 4:5 portrait works best).
- **Text:** edit `index.html` directly; each section is marked with a comment such as `<!-- Background -->`.

# Bakdaulet Karakulov — Personal Portfolio

A personal portfolio website built with [Quarto](https://quarto.org), hosted on GitHub Pages.

**Live site:** [https://bakdaulet.github.io](https://bakdaulet.github.io) *(update this URL)*

---

## 📁 Structure

```
.
├── _quarto.yml          # Site configuration & navigation
├── index.qmd            # About / Home page
├── projects.qmd         # Projects showcase
├── cv.qmd               # CV / Resume page
├── contact.qmd          # Contact page
├── styles.css           # Custom styles
├── cv/                  # Place your PDF CV here
│   └── bakdaulet-karakulov-cv.pdf
└── .github/workflows/
    └── deploy.yml       # Auto-deploy to GitHub Pages
```

---

## 🚀 Deploying to GitHub Pages

### Option A — Automatic (recommended)

The included GitHub Actions workflow auto-builds and deploys on every push to `main`.

1. Create a new repo on GitHub (e.g., `your-username.github.io` or any repo name)
2. Push this project to the `main` branch
3. Go to **Settings → Pages**
4. Under **Source**, select **GitHub Actions**
5. Push a commit — the site deploys automatically ✅

### Option B — Manual render

1. Install Quarto: [quarto.org/docs/get-started](https://quarto.org/docs/get-started)
2. Run `quarto render` in this folder
3. Commit and push the `docs/` folder
4. Go to **Settings → Pages → Source → Deploy from branch → main / docs**

---

## 🛠️ Local Development

```bash
# Preview live with hot reload
quarto preview

# Render to docs/ folder
quarto render
```

---

## 📄 Adding Your PDF CV

Place your CV PDF at `cv/bakdaulet-karakulov-cv.pdf` to enable the download button on the CV page.

```bash
mkdir -p cv
cp /path/to/your/cv.pdf cv/bakdaulet-karakulov-cv.pdf
```

---

## ✏️ Customization

- **Navigation & metadata** → `_quarto.yml`
- **Fonts, colors, layout** → `styles.css`
- **Content** → edit the `.qmd` files

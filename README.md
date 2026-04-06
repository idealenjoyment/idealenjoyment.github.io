# 🔍 Adarsh Anand — Google-Style Portfolio

> A personal portfolio website styled as a Google Search results page — complete with a Knowledge Panel, "People Also Ask", project cards, LinkedIn widget, and a resume download.

**Live site:** [idealenjoyment.github.io](https://idealenjoyment.github.io)

---

## ✨ Features

- **Google Search UI** — search bar, nav tabs, result cards, URL breadcrumbs, all faithfully recreated
- **Knowledge Panel** — sidebar with profile photo, key stats, and quick-links (LinkedIn, GitHub, Email)
- **LinkedIn Card** — embedded widget linking directly to the LinkedIn profile
- **People Also Ask** — collapsible Q&A section covering skills, experience & projects
- **Project Cards** — GDWA financial dashboard & Algo Trading Suite with tech stack labels
- **Career Timeline** — visual chronology from IIT Kanpur → Oracle intern → Oracle MTS
- **Resume Download** — one-click PDF download + view-in-browser option
- **Fully Responsive** — works on mobile, tablet, and desktop
- **Zero dependencies** — single HTML file, no npm, no build step, no framework

---

## 📁 File Structure

```
idealenjoyment.github.io/
├── index.html            ← entire portfolio (HTML + CSS + JS, single file)
├── Adarsh_Resume.pdf     ← resume (linked for download & preview)
└── README.md             ← this file
```

---

## 🖥️ Run Locally

**Option A — Double-click (instant preview)**
```
Just open index.html in any browser. Done.
```
> Note: The PDF download may be blocked by the browser for local `file://` URLs.

**Option B — Local server (full functionality)**

Requires Python 3 (pre-installed on macOS/Linux):
```bash
cd /path/to/portfolio/folder
python3 -m http.server 8080
```
Then visit → **http://localhost:8080**

---

## 🚀 Deploy to GitHub Pages

### 1. Create the repository

Go to [github.com/new](https://github.com/new) and create a repo named:

```
idealenjoyment.github.io
```

> The repo name **must** match your GitHub username exactly, followed by `.github.io`.  
> Visibility must be **Public**.

---

### 2. Push your files

```bash
cd /path/to/portfolio/folder

git init
git add index.html Adarsh_Resume.pdf README.md
git commit -m "Initial portfolio commit"

git remote add origin https://github.com/idealenjoyment/idealenjoyment.github.io.git
git branch -M main
git push -u origin main
```

---

### 3. Enable GitHub Pages

1. Open your repo on GitHub
2. Go to **Settings → Pages**
3. Under **Source** → choose **Deploy from a branch**
4. Set branch to **`main`**, folder to **`/ (root)`**
5. Click **Save**

---

### 4. Go live ✅

After ~60 seconds your site will be live at:

```
https://idealenjoyment.github.io
```

GitHub shows a ✅ under **Settings → Pages** once it's deployed.

---

## 🔄 Updating the Site

Every time you make changes, just push again:

```bash
git add index.html
git commit -m "Update: <what you changed>"
git push
```

GitHub Pages auto-redeploys on every push to `main`. No CI/CD setup needed.

---

## 📸 Adding Your Profile Photo

Find this comment in `index.html` (appears in 2 places):

```html
<!-- 📸 TO ADD YOUR PHOTO: replace the src below with your image URL or a base64 string -->
src="YOUR_PHOTO_URL_HERE"
```

Replace `YOUR_PHOTO_URL_HERE` with one of:

| Method | Example |
|--------|---------|
| Local file | `src="photo.jpg"` (place photo.jpg next to index.html) |
| Direct URL | `src="https://example.com/your-photo.jpg"` |
| LinkedIn photo URL | Right-click your LinkedIn photo → Copy image address |

---

## ✏️ Customization Reference

| What to change | Where in `index.html` |
|---|---|
| Profile name / logo | `.logo` div in `<header>` |
| Featured snippet bio | `#sec-all-featured` `.featured-body` |
| Work experience bullets | `#sec-experience` `.result-desc` |
| Projects | `.project-card` divs in `#sec-projects` |
| Education timeline | `.tl-item` divs in `#sec-education` |
| Skills pills | `.skill-pills` in `#sec-skills` |
| Stat chips (650%, 60%…) | `.stat-chip` divs in sidebar |
| Contact links | `#sec-contact` sitelinks + `kp-links` in sidebar |
| People Also Ask answers | `.paa-a` divs |
| LinkedIn card headline | `.li-headline` in the LinkedIn card |
| Resume file | Replace `Adarsh_Resume.pdf` with your file, update `href` |

---

## 🛠 Tech Stack

| Layer | Technology |
|-------|------------|
| Markup | HTML5 |
| Styling | CSS3 (custom properties, grid, flexbox) |
| Interactivity | Vanilla JavaScript |
| Icons | [Material Symbols](https://fonts.google.com/icons) (Google CDN) |
| Fonts | [Google Fonts](https://fonts.google.com) — Roboto + Google Sans |
| Hosting | GitHub Pages (free) |
| Build tool | None — zero dependencies |

---

## 📬 Contact

| | |
|---|---|
| **Email** | adarsh1anand1@gmail.com |
| **LinkedIn** | [linkedin.com/in/adarsh-anand1](https://linkedin.com/in/adarsh-anand1) |
| **GitHub** | [github.com/idealenjoyment](https://github.com/idealenjoyment) |
| **Phone** | +91-85297 61909 |

---

<p align="center">Built with ☕ by Adarsh Anand · IIT Kanpur '23 · Oracle MTS</p>

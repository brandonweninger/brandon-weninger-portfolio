# Brandon M. Weninger — Portfolio Site

A clean, responsive personal portfolio site deployed on GitHub Pages.

**Live site:** https://brandonweninger.github.io/brandon-weninger-portfolio/

---

## Site Structure

```
/
├── index.html           # Home page
├── about.html           # About Me
├── skills.html          # Skills & Expertise
├── case-studies.html    # Case Studies (5 case studies)
├── tools.html           # Tools & Resources (Job Tracker, AI Agent)
├── templates.html       # Templates & Examples (SOP, LMS Workflow, SKU Agent)
├── assets/
│   ├── css/
│   │   └── style.css    # All site styles
│   ├── images/          # Site images (add here)
│   └── files/
│       └── brandon-weninger-resume.pdf   ← Add your resume PDF here
└── README.md
```

---

## Page Manifest (Original → New Path)

| Original Google Sites Page | New File |
|---|---|
| Home | `index.html` |
| About Me | `about.html` |
| Skills & Expertise | `skills.html` |
| Case Studies | `case-studies.html` |
| Tools & Resources | `tools.html` |
| Templates & Examples | `templates.html` |

---

## How to Update the Site

### Edit a Page
1. Open the relevant `.html` file in any text editor (VS Code recommended)
2. Find the section you want to update — content is in plain semantic HTML
3. Save the file, commit, and push:
   ```bash
   git add .
   git commit -m "Update: [describe your change]"
   git push origin main
   ```
4. GitHub Pages will rebuild automatically within ~60 seconds

### Add Your Resume PDF
1. Name your resume file `brandon-weninger-resume.pdf`
2. Place it in `/assets/files/`
3. Commit and push — the Resume button on the Home and About pages will work automatically

### Add a New Page
1. Copy any existing page (e.g., `about.html`) as your template
2. Rename it (e.g., `new-page.html`)
3. Update the `<title>`, `<meta name="description">`, and page content
4. Add a nav link in the `<nav>` section of **every page** (including the new one)
5. Commit and push

### Add an Image
1. Place the image in `/assets/images/`
2. Reference it in any HTML page with:
   ```html
   <img src="assets/images/your-image.jpg" alt="Description of image" />
   ```

### Update Navigation
All nav links appear in the `<header>` section of each HTML file. To add a link, add an `<li>` inside the `<ul>` in the nav — then repeat for every page to keep navigation consistent.

---

## Local Preview

To preview locally before pushing:
```bash
# If you have Python installed:
python -m http.server 8000
# Then open: http://localhost:8000
```

Or install the VS Code "Live Server" extension and click "Go Live."

---

## GitHub Pages Setup

- **Branch:** `main`
- **Folder:** `/` (root)
- Settings → Pages → Source: Deploy from branch → `main` → `/ (root)`

---

## Contact

Brandon M. Weninger | Chicago, IL  
brandon.weninger@gmail.com

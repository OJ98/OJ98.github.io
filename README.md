# Omkar Joshi

A clean, minimal personal website built with Jekyll and hosted on GitHub Pages.

## Quick Start

### Deploy (Already Ready!)
Just push to GitHub and it's live at `https://oj98.github.io`

```bash
git add .
git commit -m "Your message"
git push origin main
```

### Local Development (Optional)
```bash
# Install Ruby: https://rubyinstaller.org/
# Then:
bundle install
bundle exec jekyll serve --host localhost --port 4000
# Visit http://localhost:4000
```

## Editing Your Site

### Site Info (`_config.yml`)
Update your basic info:
```yaml
title: Your Name
email: your.email@example.com
description: Your tagline
author:
  name: Your Name
  bio: Your bio
  location: Your city
  avatar: /images/your-photo.jpg
  github: your-username
  googlescholar: your-scholar-url
```

### Pages to Edit

**Homepage** - `index.md`
- Edit hero section intro
- Featured projects show automatically

**About** - `_pages/about.md`
- Your bio and background
- News and updates

**CV** - `_pages/cv.md`
- Education, experience, skills
- Links to PDF resume

**Contact** - `_pages/contact.md`
1. Sign up free at [Formspree.io](https://formspree.io)
2. Create form, copy Form ID
3. Replace `YOUR_FORM_ID` in contact.md

**Projects** - `_pages/projects.md`
- Auto-generates from `_projects/` folder

### Add Projects

Create file: `_projects/YYYY-MM-DD-project-name.md`

```markdown
---
layout: project
title: "Project Name"
date: 2024-01-15
description: Short description shown in grid
image: /images/preview.jpg
link: https://github.com/link-to-project
---

## Project Details

Your content here...
```

### Customize Styling

Edit `assets/css/style.css`:

```css
:root {
    --primary: #2c3e50;      /* Main color */
    --secondary: #3498db;    /* Accent color */
    --light: #ecf0f1;
    --lighter: #f8f9fa;
    --dark: #1a1a1a;
}
```

**Change fonts:**
Find `body` in CSS, change `font-family`

**Add nav links:**
Edit `.nav-links` in `_layouts/default.html`

**Change footer links:**
Edit footer in `_layouts/default.html`

## File Structure

```
.
├── _config.yml              # Site settings
├── _layouts/
│   ├── default.html         # Main template
│   └── project.html         # Project template
├── _pages/
│   ├── about.md
│   ├── cv.md
│   ├── contact.md
│   └── projects.md
├── _projects/               # Add your projects here
│   ├── 2023-project-1.md
│   └── 2024-project-2.md
├── assets/css/style.css     # All styling
├── images/                  # Add images here
├── files/                   # Add PDFs, documents
├── index.md                 # Homepage
├── Gemfile                  # Dependencies
└── .gitignore               # Git settings
```

## Common Tasks

**Add an image:**
1. Save to `images/` folder
2. Reference: `![alt text](/images/filename.jpg)`

**Add a PDF link:**
1. Save PDF to `files/` folder
2. Link: `[Download CV](/files/cv.pdf)`

**Add blog posts:**
1. Create `_posts/YYYY-MM-DD-title.md` with same front matter
2. Create `_pages/blog.md` to list them

**Change colors:**
Edit CSS variables at top of `assets/css/style.css`

**Add social links:**
Edit footer in `_layouts/default.html`

**Test changes locally:**
```bash
bundle exec jekyll serve --host localhost --port 4000
# Visit http://localhost:4000
```

## Deployment

### GitHub Pages (Free!)
1. Push code to GitHub
2. Settings → Pages → Deploy from main branch
3. Wait 2-5 minutes
4. Visit `https://oj98.github.io`

### Custom Domain (Optional)
1. Buy domain
2. Settings → Pages → Custom domain
3. Follow DNS setup

## Resources

- **Jekyll**: https://jekyllrb.com/docs/
- **GitHub Pages**: https://pages.github.com/
- **Markdown**: https://commonmark.org/help/
- **Formspree** (contact forms): https://formspree.io

## Tech Stack

- **Generator**: Jekyll 4.3
- **Theme**: Minima
- **Hosting**: GitHub Pages
- **CSS**: Plain CSS (no SASS, no dependencies)
- **JavaScript**: None required

## Performance

- Lightweight (~30KB per page)
- Fast load times (<1 second on 3G)
- Mobile responsive
- SEO optimized

---

**That's it!** All you need to know is above. Enjoy your minimal, fast website! 🚀

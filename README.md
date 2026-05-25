# maker's bench

Personal site. Built with Jekyll, hosted on GitHub Pages.

## How to update

### Add an update to the home feed
Create a file in `_updates/` named `YYYY-MM-DD-short-title.md`:

```markdown
---
title: "What you did"
project: "Project Name"
date: 2026-05-25
---

One or two paragraphs about what happened. What worked, what broke, what you learned.
```

### Add photos to a project
1. Drop the image into `assets/img/`
2. In the project's `.md` file, uncomment and edit:
```html
<div class="img-grid">
  <img src="/assets/img/your-photo.jpg" alt="Description">
</div>
```

### Embed a YouTube video
In any project `.md` file:
```html
<div class="video-wrap">
  <iframe src="https://www.youtube.com/embed/VIDEO_ID" allowfullscreen></iframe>
</div>
```

### Add a new project
Create `_projects/your-project.md`:

```markdown
---
title: "Project Name"
description: "One sentence."
category: "Category · Subcategory"
status: active        # active | paused | planning
order: 5              # controls order on homepage
tags: [Tag1, Tag2]
---

Project content in Markdown...
```

### Update "Right Now" status
Edit `index.html` — the `#now` section has the four status cards. Just edit the text directly.

## Deploy to GitHub Pages
1. Create a repo on GitHub (name it `yourusername.github.io` for a user site)
2. Push this folder
3. Go to repo Settings → Pages → Source: Deploy from branch → `main` / `root`
4. Site is live at `https://yourusername.github.io`

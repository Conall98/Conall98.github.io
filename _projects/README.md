# Projects

Each `.md` file in this folder becomes a card under "Selected Work" on the homepage, and gets its own detail page at `/projects/<filename>/`.

## How to add a new project

1. In the GitHub web UI: navigate to `_projects/`, click **Add file → Create new file**, name it `your-project-name.md` (lowercase, hyphens, no spaces).
2. Paste this template:

```markdown
---
title: "Your Project Title"
tag: "Aerodynamics"
order: 5
description: "One- or two-sentence description shown on the homepage card."
image: "/assets/img/your-project.jpg"
---

Longer write-up goes here. Markdown — use ## for subheadings, **bold**, *italics*, [links](https://example.com), images, etc.
```

3. Commit. Site rebuilds in ~1 minute.

## Field reference

- **title** — shown as the project name on the card and at the top of its page.
- **tag** — small uppercase label above the title (e.g. "Aerodynamics", "Propulsion"). Pick anything.
- **order** — controls card position on the homepage. Lower numbers appear first. Leave gaps (1, 2, 3, 4) so you can insert things later (e.g. order: 2.5).
- **description** — short blurb shown on the card.
- **image** — optional. Path to an image (e.g. `/assets/img/foo.jpg`) shown on the detail page. Leave as `""` if you don't have one yet.

This README won't appear on the site — it's just notes for you.

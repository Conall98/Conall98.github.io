# Images

Put image files in this folder. They'll be served by your site at the path `/assets/img/filename.jpg`.

## How to reference them

**In a post's frontmatter** (the card thumbnail and hero image of a post):

```yaml
---
layout: post
title: "My Post"
date: 2026-06-08
image: "/assets/img/my-photo.jpg"
---
```

**Inside the body of a post** (inline images):

```markdown
![Description of image](/assets/img/another-photo.jpg)
```

**As the site's hero banner** — open `_config.yml` and change:

```yaml
hero_banner: "/assets/img/banner.jpg"
```

## Tips

- Use lowercase filenames with hyphens, no spaces. `lake-como-2019.jpg` works, `Lake Como 2019.JPG` is fragile.
- JPG for photos, PNG for screenshots/diagrams, SVG for icons.
- Resize big photos to ~1600px wide before uploading — full-res phone photos are 20MB+ and slow the site down. A free tool like https://squoosh.app does this in the browser.
- This README file won't affect anything — it just stops the folder from being empty so git tracks it.

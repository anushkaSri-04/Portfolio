# Anushka Srivastava | Portfolio

Personal portfolio website: a career road from B.Tech to graduation, with a dedicated page for each project, internship, hackathon and research paper.

**Live site:** https://anushka-sri.netlify.app

## Features

- Career journey drawn as a winding road. The road draws as you scroll and a small car follows it.
- One page per project, with the problem, architecture flow, results and tech stack.
- Hover or tap a step in the flow to read how that part works.
- Certifications and hackathons section.
- Light and dark mode, saved between visits.
- Responsive layout for phones, tablets and desktops.
- No build step and no dependencies. One HTML file.

## Project structure

```
portfolio/
├── index.html      the whole site (content lives in the DATA block)
├── assets/
│   ├── photo.jpg   profile photo
│   ├── cover.jpg   cover image (optional)
│   └── resume.pdf  resume
└── README.md
```

## Editing the content

Open `index.html` and find the `DATA` block near the top of the script. Everything on the site comes from it.

| To change | Edit |
|---|---|
| Name, headline, skills, links, photo, resume | `DATA.profile` |
| Stops on the road | `DATA.stops` |
| Project, internship, hackathon and paper pages | `DATA.pages` |
| Certifications and hackathons | `DATA.certs` |

Tips:

- A stop with `page: true` opens `#/p/<id>`. Its `id` must match a key in `DATA.pages`.
- Leave a link or image as `""` to hide it.
- Items with `todo: true` show a dashed placeholder style. Set it to `false` when the content is real.
- Keep file names in `assets/` lowercase with no spaces.
- Check quotes and commas after editing. One missing quote can blank the page. Press F12 to see the error in the browser console.

## Run locally

Open `index.html` in a browser. No server or install is needed.

## Deploy

The site is static, so any static host works.

1. Push this folder to a public GitHub repository.
2. In Netlify, choose **Add new project**, then **Import an existing project**, and pick the repo.
3. Leave the build command empty. Publish directory: `/`.
4. Each commit to the repo then updates the live site.

Cloudflare Pages and Vercel work the same way.

## Tech

HTML, CSS and vanilla JavaScript. Fonts: Bricolage Grotesque, DM Sans and JetBrains Mono from Google Fonts.

## Contact

Anushka Srivastava, Navi Mumbai, Maharashtra. Add your email and LinkedIn in `DATA.profile`.
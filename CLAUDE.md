@AGENTS.md

# Project: Personal portfolio site

Built on al-folio (Jekyll theme), deployed via GitHub Pages at https://shilpithathokala.github.io 
Inspired by https://rohitbandaru.github.io/ — clean, technical, blog-forward.

## About me

- Robotics MSE student at Johns Hopkins University (expected 2027)
- Research focus: perception, embodied AI / physical AI
- Coursework: Deep Learning (A+), Computer Vision (A-), Deep RL
- B.Tech in Automation & Robotics Engineering from Amrita (2021–2025), CGPA 9.02/10
- Research experience:
  - IIIT Hyderabad — vision-based UAV obstacle detection, MPC controllers (Jan–Jul 2025) 
  - IIT Palakkad 
- Publication: VQ-VAE-based trajectory generation for multi-drone coordination, ICCA 2025 {https://scholar.google.com/citations?view_op=view_citation&hl=en&user=VVR4eaoAAAAJ&authuser=2&citation_for_view=VVR4eaoAAAAJ:u-x6o8ySG0sC}
- Course Assistant for Computer Vision at JHU (Spring 2026)

## Career goals (drives content priorities on this site)

- **Primary:** industry roles in perception / embodied AI / physical AI as a new grad
- **Secondary:** PhD admission in the same areas
- Site should serve both audiences: recruiters scanning for hireable signal, and PhD admissions readers looking for technical depth and writing ability

## Site scope (v1)

Three navbar sections only:
- **About** — short intro, photo, what I work on, links (LinkedIn, GitHub, email)
- **CV** — resume content rendered from `_data/cv.yml`; PDF download link to `assets/pdf/Shilpitha-Resume.pdf`
- **Blog** — technical posts on robotics, perception, physical AI; cheatsheets for frameworks I'm learning

Hide from the navbar for now (keep template files in repo, switch on later):
- Projects — re-enable when I have 2–3 strong writeups
- Publications — re-enable when ICCA paper is indexed on Google Scholar
- News, teaching, repositories — not relevant yet

## Conventions

- Blog posts live in `_posts/` as `YYYY-MM-DD-title.md` with proper frontmatter
- Always show me diffs before applying multi-file changes
- I'm new to Jekyll/Liquid — when you do something non-obvious, briefly explain why
- Prefer minimal config changes; flag any structural changes before making them
- When I ask "how do I do X," default to explaining rather than just doing — I'm learning, not just shipping
- For any new dependency, library, or build step you add, tell me what it does and why we need it
- Commit messages: imperative mood, concise (e.g., "Add CV page" not "Added the CV page yesterday")

## What "done" looks like for v1

- Live site at `<username>.github.io` with About, CV, and Blog in the nav
- About page has my photo, a paragraph bio, working social links
- CV page renders my actual resume content and offers PDF download
- At least one published blog post (I have an idea on writing it about filters and applications in the robotics sense. will work on the content thoroughly once we have a preliminary site published)
- Mobile-responsive, dark mode toggle working, no broken links

## Build log

_Format: `date` — `commit subject` — files touched — one-line note. Chronological, oldest first._

- `2026-05-20` — `Tidy CLAUDE.md and add build log section` — `CLAUDE.md` — Removed duplicate `@AGENTS.md` import, set canonical site URL to `shilpithathokala.github.io`, added this Build log section.
- `2026-05-20` — `Set site identity in _config.yml` — `_config.yml` — Replaced upstream al-folio defaults (`description`, `keywords`, `url`, `baseurl`, `contact_note`) with personal values; left name fields, footer, icon, scholar config untouched (scholar still set to Einstein — fix when re-enabling Publications).
- `2026-05-20` — `Hide unused sections from navbar` — `_pages/projects.md`, `_pages/publications.md`, `_pages/teaching.md`, `_pages/repositories.md` — Set `nav: false` on four pages to leave only About, CV, Blog in the navbar; news.md already had no `nav:` key, so left untouched.
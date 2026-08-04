# Asif Adnan — Portfolio

A single-page professional portfolio for **Asif Adnan**, a Social Work graduate (BSS, Pabna University of Science & Technology) and Project Monitoring Officer, built to showcase field experience, publications, and community leadership work.

🔗 **Live site:** [asif-adnan2743.github.io](https://asif-adnan2743.github.io/)

## Design Concept

The site is styled as a **"field case file / ledger"** — an aesthetic drawn from the documentation-heavy nature of social work itself (case records, field reports, verified credentials):

- Ledger-lined paper background, aged-paper colour palette (moss green, rust, warm cream)
- A rotated **ID-card badge** in the hero section standing in for a laminated field officer's ID
- A hand-stamped **"Verified Field Record"** seal
- Typewriter-style section labels (`Exhibit 01`, `Exhibit 02`, …) and dashed "perforation" dividers
- Fonts: [Fraunces](https://fonts.google.com/specimen/Fraunces) (headings), [Inter](https://fonts.google.com/specimen/Inter) (body), [Special Elite](https://fonts.google.com/specimen/Special+Elite) (typewriter labels)

## Sections

| Section | Content |
|---|---|
| Hero | Name, role, contact shortcuts, ID-card photo badge |
| Career Objective | Summary of goals and strengths |
| Professional Experience | Project Monitoring Officer role + internships |
| Publications | Poster & conference paper, incl. Emerging Visionary Award |
| Education | BSS, HSC, SSC — timeline with results |
| Leadership & Community Engagement | HELP, PUST Cricket Club, Students' Association roles |
| Core Competencies | Soft skills + technical/computer skills |
| Certifications & Training | ICT & Microsoft Office training history |
| References | Academic references |
| Declaration | Signed declaration statement |
| Contact | Email, phone, LinkedIn, address |

## Tech Stack

Plain **HTML, CSS, and vanilla JavaScript** — no build step, no dependencies, no frameworks. Just open `index.html` in a browser or deploy as-is.

- Scroll-spy navigation with a mobile hamburger menu
- Typewriter-effect role tagline in the hero
- Scroll-triggered fade-in animations via `IntersectionObserver`
- Fully responsive (desktop → tablet → mobile)

## Adding Your Photo

The hero ID-card looks for a photo at:

```
/asif-adnan.jpg
```

To add it:

1. Place a photo named **`asif-adnan.jpg`** in the **same folder** as `index.html` (repo root).
2. Commit and push. GitHub Pages will pick it up automatically — no code changes needed.

If the file is missing, the badge gracefully falls back to showing the **"AA"** initials, so the layout never breaks.

> Prefer a different filename or path? Update the `src` attribute on the `<img>` inside `.id-avatar` in `index.html`.

## Deployment (GitHub Pages)

1. Push this repo to GitHub (e.g. `asifadnan/asifadnan.github.io` for a user site, or any repo name + enable Pages for a project site).
2. Go to **Settings → Pages**.
3. Under **Source**, select the `main` branch and `/ (root)` folder.
4. Save — your site will be live at `https://<username>.github.io/` (or `/<repo-name>/` for a project site) within a minute or two.

## File Structure

```
.
├── index.html        # entire site — markup, styles, and script in one file
├── asif-adnan.jpg     # profile photo (add this yourself)
└── README.md
```

## Customizing Content

All content lives directly in `index.html` as plain HTML — no CMS or data file. Search for the section you want to edit (e.g. `<section id="experience">`) and update the text directly. Colours and fonts are controlled via CSS custom properties at the top of the `<style>` block (`:root { --moss: ...; --rust: ...; }`) if you want to retheme the site.

## License

Personal portfolio content © Asif Adnan. Feel free to fork the code/layout for your own portfolio — just swap in your own content and photo.

# CV Website — Xavi Carbó

Single-page, static CV built with plain **HTML + CSS**.

- **Live page:** https://xerbok.github.io/hypermedia-project-part-1/
- **Figma design (proposal):** _Add your public Figma link here_

---

## 1) Project analysis

### User profile (User persona)

**Role:** Junior Tech Recruiter at a software company in Barcelona  
**Goals:** Quickly decide if the candidate fits an **intern/junior** role; verify core skills (C/C++, Java, HTML/CSS/JS, React, PHP, SQL); see concise **projects**; find **contact** instantly.  
**Needs:** Very limited time; expects **clear structure**, skimmable content, and working links that open safely in a new tab.  
**Devices:** Mostly desktop/laptop; occasionally mobile.  
**Expectations:** Fast page, obvious sections (**About**, **Skills**, **Experience**, **Education**, **Projects**, **Contact**), simple navigation, readable typography, and a dark UI that keeps focus on content.

---

### Information architecture

This project is a **single-page** site that mirrors how a recruiter scans a CV. A persistent **header** contains the name (as brand) and a compact navigation list linking to in-page anchors for the six main blocks: About, Skills, Experience, Education, Projects, and Contact. This enables immediate jumps without losing context. The page begins with a **Hero** area that states who the candidate is and what they bring: “Computer Engineering student,” plus a short technology summary. Two calls-to-action are provided: **Contact** (scrolls to the form of contact details) and **Download CV (PDF)** for offline review.

**About** offers a concise, two-paragraph bio focusing on strengths and interests (front-end + back-end) and sits beside a portrait image to humanize the profile. The **Skills** section uses small “chips,” making the stack easy to scan horizontally (C/C++, Java, HTML, CSS, JavaScript, React, PHP, SQL). **Experience** follows with short bullet lists emphasizing what was done (data management with C++/Java, accessible layouts, SQL work). **Education** lists the degree, year, and relevant coursework. **Projects** showcases three focused items—CSV Reader (C++), a Java package-delivery simulator on a node map, and a 3D horror tactics prototype—each with a short description and external link. Finally, **Contact** closes the journey with email and LinkedIn. The order flows from quick positioning (who/what) → evidence (skills/experience/education/projects) → action (contact). A centered **wrapper** keeps line length comfortable and the layout remains simple on all viewports.

---

### Visual design

The site uses a **dark theme by default** to keep visual noise low and highlight important actions. Colors are defined as CSS variables for clarity and quick iteration: `--bg` (background), `--text` (primary text), `--muted` (secondary text), `--border` (dividers), `--accent` (links and highlights), and `--card` (subtle surfaces). Example values: `--bg: #0b1220`, `--text: #e5e7eb`, `--accent: #60a5fa`. Declaring `color-scheme: dark` allows the browser to adjust native UI (scrollbars/form controls) to match. The **system-UI** font stack is used to avoid external dependencies and ensure good performance and familiar rendering across platforms.

Hierarchy and spacing are restrained: compact headings, generous line-height for paragraphs, and accent color used only for highlights and interactive states. The **header** is sticky with a light bottom border so navigation is always available during scroll. Content is centered via a reusable `.wrapper` (max-width 1000px) to maintain readable line lengths. Layout employs **CSS Grid** and **Flexbox** where it adds clarity: `.two-col` arranges text and portrait in the About section; `.grid` lays out project cards in columns, collapsing gracefully on smaller screens. Cards and skill chips have light borders and small radius to keep the UI tidy. Hover states are subtle (slight elevation on cards) to signal interactivity without visual clutter. The result is a lean, readable interface that focuses attention on content and keeps the codebase straightforward for maintenance.

---

## 2) Design proposal using Figma

- **Components:** Header/nav, Hero (title, lead, CTAs), Section headers, Two-column About, Skill chips, Experience items, Education list, Project cards, Footer.  
- **Tokens:** Add the same color variables and type scale used in CSS so the hand-off matches the build.  
- **Prototype:** Simple scroll flow with anchor navigation; include hover states for nav and cards.  
- **Link:** _Add your public Figma link here_

---

## 3) Project implementation

- **Tech:** Plain **HTML** (semantic structure) + **CSS** (layout/visuals).  
- **Files:** `index.html` and `styles.css`.  
- **Dark mode:** Dark is **default**, defined via CSS variables and `color-scheme: dark`.  
- **Navigation:** In-page anchors in the header; external links use `target="_blank"` with `rel="noopener"`.  
- **Layout:** Centered wrapper, simple grid for projects, two-column About, minimal responsive behavior.

---

## Extra information

This CV intentionally does not include live links to project repositories or a LinkedIn profile. The project titles, descriptions, and some dates are partly illustrative for coursework and therefore do not fully reflect my real portfolio or employment history. This document should be read as a design/content prototype rather than an authoritative record. Once the placeholders are replaced with verified project artifacts and my updated LinkedIn, I will add the corresponding links and remove this notice.






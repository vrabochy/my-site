# simple_site

A single-page personal portfolio website for Volodymyr Rabochy, a Strategy & Business Development professional in the energy sector (Oil & Gas, CCUS, SAF, Geothermal). The site serves as a digital CV and contact point for job opportunities.

## Workspace contents

| File | Purpose |
|------|---------|
| [index.html](index.html) | The entire website — one self-contained HTML file |
| [CV VRabochy 2025 -EN v26ENFR.pdf](CV%20VRabochy%202025%20-EN%20v26ENFR.pdf) | Source CV used as content reference when building the site |

## index.html — structure and purpose

`index.html` is a fully self-contained portfolio page (no external CSS files, no build step, no framework). Everything — layout, styles, and JavaScript — lives in a single file.

### Sections

| Section | ID | Description |
|---------|----|-------------|
| Navigation | `nav` | Fixed top bar with smooth-scroll links and a "Contact me" CTA button |
| Hero | `#hero` | Name, title, sector tags, skill pills, LinkedIn link, and four headline stats (20+ years, $120M contracts, €13M new contracts, 4 languages) |
| Uniqueness of Profile | `#uniqueness` | Five numbered differentiators explaining what makes the profile rare (triple academic background, operator + consultant + builder, early decarbonisation expertise, quantitative strategy, multilingual international reach) |
| Expertise | `#expertise` | Six cards covering Corporate Strategy, Market Intelligence, Energy Transition, Business Development, Organisation & Operations, and Cross-Cultural Leadership |
| Work Experience | `#experience` | Vertical timeline from 2001 to present: Accenture/Oracle ERP → Schlumberger Business Consulting → SLB Chief Analyst → SLB Commercial Strategy → SLB Country Manager → Technip Energies Principal Advisory → XP Group BD Manager |
| Education | `#education` | Three degrees: MSc Computer Sciences (Kyiv-Mohyla, 2000), MBA (INSEAD, 2008), MSc Subsurface Energy Systems / CCS & Geothermal (Heriot-Watt, 2021) |
| Languages | `#languages` | Ukrainian (native), English, French, Russian (all fluent) |
| Footer | `footer` | Email, phone, LinkedIn |
| Contact modal | `#contactModal` | Animated overlay form that submits via [Formspree](https://formspree.io) (endpoint `xgojedbn`); builds a plain-English message from name + email and sends it to the site owner |

### Technical notes

- **No dependencies.** Pure HTML5/CSS3/vanilla JS — opens directly in any browser without a server.
- **Responsive.** A `@media (max-width: 768px)` block collapses the hero, timeline, and nav for mobile.
- **Dark theme.** CSS custom properties define a navy/gold palette (`--navy`, `--gold`, etc.) used consistently throughout.
- **Contact form.** Uses the Formspree API (`fetch` + `FormData`) with client-side validation; shows success/error feedback inline and auto-closes the modal after a successful send.
- **Smooth scroll** is enabled globally via `html { scroll-behavior: smooth; }`.

## How to use

Open `index.html` in a browser — no build step or local server needed.

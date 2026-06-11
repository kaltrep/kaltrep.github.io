# CLAUDE.md — kaltrep.github.io

## Repo & Deployment
- Static site, GitHub Pages, multi-file
- No build step, no dependencies beyond Outfit web font (Google CDN)
- Local preview: `python -m http.server 8080` → http://localhost:8080
- Always preview locally before committing

## File Structure
```
kaltrep.github.io/
├── index.html                      # Main single-scroll page
├── about.html                      # Expanded Jeff Steele bio page
├── CNAME                           # Domain config — do not modify
├── images/
│   └── jeff-steele.jpg             # Professional headshot
└── docs/
    └── kaltrep-brand-reference.html  # Brand reference — do not modify
```

## Brand Reference
Full spec: `docs/kaltrep-brand-reference.html`

### Quick Reference
**Colors**
- Background: #0D1520 · Cards: #1A2332
- Accent: #63B3ED (Ice) — use sparingly
- Primary text: #EDF2F7 · Secondary: #8AA4BE

**Fonts**
- Display/headings: Georgia
- Body: Outfit weight 300
- Labels: Trebuchet MS, uppercase, letter-spaced

**Voice**
- Precise, direct, confident — no hedging
- Lead with numbers and outcomes
- Firm sections (Services, Approach, Work) use "we" / "our" — Kaltrep as the entity
- About page and Jeff-specific content uses "I" / "my" — Jeff speaking directly
- Tagline: "Connecting data. Driving decisions."
- Avoid: synergy, leverage, holistic, cutting-edge, robust solution
- Use: build, ship, reduce, automate, connect, design, measure
- Job titles used as credential markers: capitalize all words
  (e.g., "Drilling Engineer. Completions Field Supervisor." — not sentence case)

**Hard rules**
- No red, orange, or warm accents
- No purple gradients
- K-graph logo nodes always Ice Blue

## Site Structure

### index.html — Main single-scroll page
Sections (top to bottom): Hero · Services · About Preview · Approach · Work · Contact
Nav links: Services · About · Approach · Work · Contact

**Services section:** Three cards
- 01 · Data Platform Engineering
- 02 · Analytics & Business Intelligence
- 03 · Oil & Gas Operations

**About Preview:** Horizontal card between Services and Approach
- Jeff's headshot (left), 2–3 sentence bio (right), "Learn more" link → about.html
- Uses "I" voice

### about.html — Expanded bio page
Sections: Page header · Narrative bio · Accomplishment stats (4-up) · Expertise tags · LinkedIn CTA
- Nav mirrors index.html; "About" link is active state
- "← Back" or nav returns to index.html
- Uses "I" voice throughout

## Naming & Attribution Decisions
- **EQT Corporation:** Name directly. Jeff's employment there is public record and listed on
  LinkedIn (which the site links to). "Former Director of Business Intelligence at EQT Corporation"
  is factual employment history, not an implied endorsement.
- **EQT size:** Fortune 500. Verified.
- **Team:** Jeff is the sole client-facing consultant. Two partners assist in the background
  but do not appear in Kaltrep engagements. Site uses "we" for firm voice but does not
  reference partner headcount.

## Content Decisions Log
- 2026-06-11: Shifted from two service cards (Asset Evaluation + Digital Consulting) to
  three (Data Platform Engineering + Analytics & BI + Oil & Gas Operations). Asset Evaluation
  was DDI positioning, not Kaltrep's.
- 2026-06-11: Added about.html and images/ directory. Moved from single-file to multi-file.
- 2026-06-11: Established "we" (firm) / "I" (About) voice split.

## Change Protocol
- **Content updates** (copy, stats, tags): proceed
- **about.html changes**: proceed — self-contained page
- **Structural changes to index.html**: require spec from Claude Chat Kaltrep project first
- **New pages**: require spec from Claude Chat Kaltrep project first
- **Brand system changes**: require brand-reference.html update first, then propagate

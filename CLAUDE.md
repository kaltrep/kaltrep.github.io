# CLAUDE.md — kaltrep.github.io

## Repo & Deployment
- Static site, GitHub Pages, single file: index.html
- No build step, no dependencies beyond Outfit web font (Google CDN)
- Local preview: `python -m http.server 8080` → http://localhost:8080
- Always preview locally before committing

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
- Tagline: "Connecting data. Driving decisions."
- Avoid: synergy, leverage, holistic, cutting-edge, robust solution
- Use: build, ship, reduce, automate, connect, design, measure

**Hard rules**
- No red, orange, or warm accents
- No purple gradients
- K-graph logo nodes always Ice Blue

## Site Structure
Single-page static site. Full source in index.html.
Sections: Hero · Services · Approach · Work · Contact
Read index.html directly for current implementation.

## Change Protocol
- Content updates: proceed
- Structural changes: require spec from Claude Chat 
  Kaltrep project first

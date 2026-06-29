# Portfolio Sprint — Plan for Divya Verma
**Date:** 29 June 2026

---

## 1. Design Direction

### Subject
Personal portfolio for **Divya Verma** — AI Engineer & Full Stack Developer.  
Audience: Recruiters, hiring managers, fellow engineers, and collaborators.  
Single job: Instantly communicate credibility, personality, and technical depth — and convert a visitor into a contact or collaborator.

### Token System

| Role | Value | Notes |
|------|-------|-------|
| `--bg` (light) | `#F8F8F6` | Warm off-white — not cream, not pure white |
| `--card` (light) | `#FFFFFF` | Pure white cards |
| `--text-primary` (light) | `#111111` | Near-black |
| `--text-secondary` (light) | `#777777` | Muted prose |
| `--border` (light) | `#ECECEC` | Hairline dividers |
| `--accent` | `#3B82F6` | Blue — tech credibility, trust |
| `--bg` (dark) | `#090909` | Near-black |
| `--card` (dark) | `#171717` | Slightly lifted |
| `--text-primary` (dark) | `#FFFFFF` | |
| `--text-secondary` (dark) | `#A1A1AA` | |
| `--border` (dark) | `#2A2A2A` | |
| `--accent` (dark) | `#4F9DFF` | Slightly lighter blue for dark bg |

### Typography

| Role | Family | Size | Weight |
|------|--------|------|--------|
| Hero display | Instrument Serif | 64–72px | 400 |
| Section titles | Instrument Serif | 42px | 400 |
| Card titles | Inter | 28px | 600 |
| Body | Inter | 18px | 400 |
| Small / labels | Inter | 15px | 500 |
| Line height | — | — | 150% |

### Layout
- Max-width: **1280px**, center-aligned
- Grid: 2-column projects grid, single-column on mobile
- Vertical rhythm: 120px between sections on desktop, 80px on mobile
- Border-radius: **20–24px** on cards, **12px** on badges/buttons
- Shadows: `0 1px 3px rgba(0,0,0,0.06), 0 8px 24px rgba(0,0,0,0.08)`

### Signature Element
**Animated gradient orb** in the hero — a soft, slow-moving radial gradient blob in the background behind Divya's name. Subtle, not distracting. Reinforces the "intelligent digital products" brand identity. Every other section stays quiet and typographic.

---

## 2. Section Plan

| # | Section | Key Content |
|---|---------|-------------|
| 1 | **Hero** | Name, title, 1-line intro, View Projects + Contact Me CTA, profile photo, social links, resume download |
| 2 | **Projects** | 2-col grid — AI Women Safety App, Sorting Visualizer, AI Chat App, Food Donation Platform, ML Dashboard |
| 3 | **Skills** | Premium rounded badge clusters: Languages, Frameworks, Tools, ML/AI |
| 4 | **Experience** | Vertical timeline cards with fade-in reveal |
| 5 | **About** | Large editorial layout — background, drive, current focus, education, interests, athlete badge |
| 6 | **Contact** | Large CTA — email, LinkedIn, GitHub, resume download |
| 7 | **Footer** | Name, nav links, theme toggle, copyright |

---

## 3. Animation Plan

| Element | Animation |
|---------|-----------|
| Page load | Fade + slide-up staggered (hero text, then image) |
| Scroll reveal | IntersectionObserver fade-up on each section |
| Project cards | Lift + shadow + image zoom on hover |
| Buttons | Ripple on click |
| Scroll progress bar | Thin accent-colored bar at top |
| Theme toggle | Smooth CSS transition on all color vars |
| Hero orb | CSS `@keyframes` slow drift |
| Skill badges | Stagger fade-in when section enters viewport |

---

## 4. Technical Stack (Single HTML File)

- Vanilla HTML5 + CSS3 + JavaScript (ES6+)
- Google Fonts: Inter + Instrument Serif
- CSS custom properties for theming
- IntersectionObserver for scroll reveals
- No external JS libraries — pure, fast, zero-dependency
- Semantic HTML for SEO and accessibility
- `prefers-reduced-motion` media query respected
- Responsive breakpoints: 1280px / 768px / 480px

---

## 5. Checklist

- [ ] Responsive (mobile, tablet, desktop)
- [ ] Light/Dark mode toggle
- [ ] All section links work
- [ ] Resume download button present
- [ ] GitHub, LinkedIn, Email links present
- [ ] Semantic HTML (header, main, section, footer)
- [ ] No placeholder text remaining
- [ ] Scroll progress bar
- [ ] Smooth scrolling
- [ ] Accessible focus states
- [ ] prefers-reduced-motion respected
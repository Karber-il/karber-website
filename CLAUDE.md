# Karber Website — Design Rules

## Stack
- Single `index.html` file
- Tailwind CSS via CDN
- Lucide icons via CDN
- Heebo font from Google Fonts (NOT Inter)
- Deployed on Netlify + GitHub

## Language & Direction
- All text: Hebrew only — NO English anywhere on the site
- `<html lang="he" dir="rtl">` — fully RTL layout

## Color Palette
| Token | Hex | Usage |
|---|---|---|
| Primary background | `#FFFFFF` | Main sections |
| Secondary background | `#FAFAFA` | Alternate sections (Services, Contact) |
| Dark dramatic background | `#4D4D4D` | "Why Karber" section ONLY |
| Footer background | `#1A1A1A` | Footer only |
| Primary text | `#1A1A1A` | Headings, body |
| Secondary text | `#666666` | Subtext, captions |
| Brand accent | `#FFCA1E` | Buttons, step numbers, key highlights — ~20% usage only |
| Borders/dividers | `#E5E5E5` | Card borders, section dividers |

## Typography
- Font: **Heebo** (Google Fonts), weights 400 / 500 / 700 / 900
- `font-black` (900): hero headline, large display text
- `font-bold` (700): section headings, card titles
- `font-medium` (500): labels, nav links
- `font-normal` (400): body text, captions

## Spacing & Shape
- **Border-radius: maximum 4px** — sharp, professional. Never exceed 4px.
- Heavy whitespace between sections (py-24 minimum)
- Section padding: `px-4 sm:px-6 lg:px-8` with `max-w-7xl mx-auto`

## DO
- Light, minimal, clean, modern design — shadcn aesthetic
- Mobile responsive (minimum 320px width)
- Scroll animations via IntersectionObserver (fade-up, 400ms ease-out)
- Smooth hover effects on buttons (scale 1.02) and cards (shadow lift)
- Floating WhatsApp button: bottom-LEFT corner (RTL convention), green circle
- Logo: `images/LOGO 2.png` (URL-encoded as `images/LOGO%202.png`)
- Hero: `min-h-screen` + `min-height: 100svh` (svh fallback for mobile browsers)
- Hero background: `images/15.jpeg` with overlay `rgba(26,26,26,0.65)`
- All form fields: Hebrew labels and placeholders
- Phone/email in forms: `dir="ltr"` for correct display

## DON'T
- NO bright saturated gradients or gradient text
- NO emoji icons — use Lucide only
- NO "revolutionary", "game-changing" marketing copy
- NO heavy shadows or busy patterns
- NO dark mode toggle
- NO border-radius > 4px
- NO English text anywhere (including buttons, labels, placeholders)
- NO testimonials section
- NO client logos section
- NO specific year claims or statistics numbers

## Images
All images are in `images/` directory. Key assignments:
- Hero bg: `images/15.jpeg`
- About: `images/38.jpeg`
- Service 1 (dry ice): `images/5.jpeg`
- Service 2 (electrical): `images/17.jpeg`
- Service 3 (high pressure): `images/30.jpeg`
- Service 4 (abrasive): `images/20.jpeg`
- Before/after 1: `images/39.jpeg`
- Before/after 2: `images/41.jpeg`
- Before/after 3: `images/43.jpeg`
- Logo: `images/LOGO%202.png`

## Deployment
- GitHub CLI: `"C:\Program Files\GitHub CLI\gh.exe"` — logged in as karber-il
- Netlify CLI: use `netlify.cmd` (NOT `netlify`) due to PowerShell execution policy
- Netlify team slug: `Karber`
- Site name: `karber`

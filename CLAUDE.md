# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

L2W Trades is a static marketing website for a trading mentorship service. The site promotes 1-on-1 mentorship ($5000/month) and a Discord community ($200/month).

## Project Structure

- `index.html` - Main landing page with hero section, case studies, pricing, testimonials
- `contact.html` - Contact information and support policies
- `terms.html` - Terms of service
- `refund.html` - Refund policy
- `assets/` - Media assets
  - `images/` - Image files (case studies, testimonials)
  - `videos/` - Video files

## Technical Details

- **No build process**: Pure static HTML/CSS/JS - open HTML files directly in browser
- **Styling**: All CSS is inline within each HTML file (no external stylesheets)
- **Fonts**: Inter and Space Grotesk from Google Fonts

## Design System

**CSS Variables** (defined in `:root`):
- `--blue: #3b82f6` / `--accent: #60a5fa` - Primary brand colors
- `--bg-primary: #0a0a0a` - Dark background
- `--border-subtle` / `--border-hover` - Border states

**Key Animation Classes**:
- `.reveal` - Scroll-triggered fade-up animation (uses IntersectionObserver)
- `.text-shimmer` - Animated gradient text effect
- `.glow-card` - Hover glow effect on cards
- `.border-beam` - Rotating border light effect (Aceternity-style)
- `.fade-up` / `.animate` - Initial page load animations

## Development

To preview: Open any `.html` file directly in a web browser. No server required.

## Architecture Notes

- Modal popup for case study details (`#caseModal`)
- Responsive breakpoint at 768px
- Gradient text uses `-webkit-background-clip: text`
- Spotlight effect follows cursor position 

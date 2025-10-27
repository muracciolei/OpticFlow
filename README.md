# OpticFlow

[![Release](https://img.shields.io/github/v/release/muracciolei/OpticFlow?display_name=tag&sort=semver&color=4F46E5)](https://github.com/muracciolei/OpticFlow/releases)

Clinical visual assessment and vision-health tracking platform with professional-grade diagnostic tests.

## Overview
OpticFlow is a full-stack, professional-grade platform for clinical visual assessment and longitudinal vision-health tracking. It delivers validated test modules, secure user management, and a modern analytics dashboard with exportable reports.

## Features and Modules
1. Landing Page + Auth System
- NextAuth with credentials and OAuth providers
- Role-based access (patient/clinician/admin)
- Basic user profiles with avatar, demographics, and preferences

2. Visual Acuity Test (with calibration)
- Distance calibration UI with device PPI and viewing distance helpers
- Sloan/ETDRS letter charts with randomized sequences
- Keyboard/touch input with error tracking

3. Contrast Sensitivity Test
- Pelli-Robson–style contrast steps and adaptive staircase
- Ambient-light warning and gamma/brightness quick checks

4. Color Vision Test (Ishihara Plates)
- Randomized plate order, response capture, scoring summary
- Color-profile notice and display suitability tips

5. Results Dashboard
- Chart.js/Recharts visualizations (acuity progression, contrast curves, color accuracy)
- PDF export via Puppeteer
- Dark/Light theme toggle

6. Clinical History Storage
- MongoDB + Mongoose models for tests and sessions
- CRUD for test records, timeline analytics, and notes

7. Professional Design
- TailwindCSS + shadcn/ui components
- Micro-animations, focus rings, and motion-reduced fallbacks
- Accessible color system, ARIA labels, keyboard navigation

## Tech Stack
- Next.js (App Router) + TypeScript
- MongoDB + Mongoose
- NextAuth
- TailwindCSS + shadcn/ui
- Chart.js or Recharts
- Puppeteer for PDF export

## Project Structure
```
src/
 ├─ app/
 ├─ components/ui/
 ├─ lib/
 ├─ models/
 ├─ tests/
 └─ public/assets/
```

## Getting Started
1. Clone the repo
   git clone https://github.com/muracciolei/OpticFlow.git && cd OpticFlow
2. Install
   pnpm install
3. Environment
   - Create .env.local with NEXTAUTH_SECRET, NEXTAUTH_URL, MONGODB_URI, etc.
4. Dev
   pnpm dev

## Scripts
- dev: Next.js dev server
- build: Next.js build
- start: Production server
- test: Unit and component tests (Vitest/RTL)
- lint/format: Code quality

## Release
Visit the Releases page to download stable builds.

## License
MIT (or institution policy). Contributions welcome.

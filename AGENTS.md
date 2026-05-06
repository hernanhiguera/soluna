# Soluna — AGENTS.md

## Project Identity

Soluna is a mobile-first AI landscape design and project gateway platform.

Version 1 is a fast web app where homeowners upload a yard photo, choose preferences, generate realistic landscape design concepts, and request a real estimate from a local contractor.

Long-term, Soluna may grow into a full outdoor construction operating system:

**Scan → Design → Permit → Materials → Delivery → Installation → Maintenance**

Version 1 must stay simple.

---

## Main Reference Files

Read these before making decisions:

1. `PROJECT_BRIEF.md`
2. `PRODUCT_REQUIREMENTS.md`
3. `UI_UX_GUIDELINES.md`
4. `TECH_STACK.md`
5. `ROADMAP.md`
6. `OPEN_QUESTIONS.md`
7. `AGENTS.md`

---

## Product Priorities

Prioritize in this order:

1. Speed
2. Mobile usability
3. Simple user flow
4. Lead generation
5. Realistic landscape concepts
6. Clean architecture
7. Future expandability
8. Visual polish

Do not sacrifice speed for fancy UI.

---

## Core V1 User Flow

1. User lands on web app.
2. User sees clear headline.
3. User uploads yard photo.
4. User chooses landscape style.
5. User chooses budget level.
6. User selects desired features.
7. App generates AI concept.
8. User sees result.
9. User can request estimate or paid upgrade.
10. Project is saved as a lead.

Do not add extra steps unless they directly improve conversion or output quality.

---

## UX Priorities

The app should feel:

- Fast
- Sturdy
- App-like
- Clean
- Premium
- Easy
- Visual
- Low-friction

The user is likely on a phone, possibly sitting in their yard looking for ideas.

---

## Code Priorities

Code should be:

- Type-safe
- Modular
- Readable
- Simple
- Easy to extend
- Mobile-first
- Performance-conscious

Prefer clean, boring code over clever code.

---

## Architecture Rules

Build Soluna as modules, not one tangled app.

Core modules:

1. Capture
2. Preferences
3. AI Generation
4. Project Model
5. Lead Capture
6. Contractor Routing
7. Payments
8. Future Design Layers
9. Future Materials
10. Future Permit Tools

Each module should be separable and replaceable.

---

## Data Rules

Every meaningful user session should create or update a Project.

A Project may eventually contain:

- Uploaded photos
- Top-view images
- Video
- LiDAR scans
- Style choices
- Budget choices
- Feature choices
- AI outputs
- Material lists
- Estimates
- Contractor leads
- Permit data
- Order data
- Installation status

Version 1 only needs early fields, but the structure should allow growth.

---

## UI Decision Rules

Use:

- Mobile-first layout
- Large tap targets
- Visual cards
- Sticky CTAs where useful
- Short text
- Clean spacing
- Fast interactions

Avoid:

- Desktop-first design
- Long landing pages before the product action
- Heavy animations
- Full-page glass effects
- Too many form fields early
- Small buttons
- Hidden CTAs
- Generic AI demo look

---

## Performance Rules

Speed is more important than visual tricks.

Required:

- Compress uploaded images.
- Lazy-load heavy assets.
- Keep bundle size small.
- Avoid unnecessary animation libraries.
- Test on mobile Safari.
- Prevent horizontal overflow.
- Keep the first screen fast.

Avoid:

- Large background videos.
- Heavy blur everywhere.
- Expensive glass effects on scrolling containers.
- Large unoptimized images.
- Unnecessary client-side dependencies.

---

## Glass UI Rules

Soluna may use light glass-inspired UI only if it does not hurt speed.

Good places:

- Upload card
- Style cards
- Budget selector
- Floating CTA
- Result card

Bad places:

- Entire page background
- Every button
- Long scrolling lists
- Large animated panels

The style should feel premium and subtle, not gimmicky.

---

## AI Output Rules

AI-generated designs should be:

- Realistic
- San Diego-friendly
- Climate-aware
- Buildable-looking
- Based on the uploaded photo
- Matched to user preferences

Avoid outputs that:

- Ignore the original yard
- Add impossible structures
- Look like fantasy art
- Mislead users into thinking this is a final construction plan
- Present rough concepts as official plans

Use language like:

- concept
- preview
- idea
- visual direction

Avoid language like:

- official plan
- permit-ready
- architectural blueprint

unless that functionality is actually built later.

---

## Lead Generation Rules

Collect:

- Name
- Email
- Phone
- ZIP code
- Project type
- Budget level
- Timeline
- Style choice
- Desired features
- Uploaded photo
- AI concept
- User notes

Do not send a lead to a contractor without user consent.

---

## Version Control Rules

When adding features:

1. Do not break the existing V1 flow.
2. Add new functionality as a module.
3. Preserve existing project data.
4. Keep database migrations clean.
5. Use feature flags for experiments when useful.
6. Keep components reusable.
7. Keep UI simple.

---

## Decision Rules

When unsure, choose the option that:

1. Gets a real user to the AI result faster.
2. Improves mobile experience.
3. Helps capture a qualified lead.
4. Keeps future architecture clean.
5. Avoids overbuilding.

If a feature does not help V1 users upload, visualize, or convert, delay it.

---

## Things to Avoid

Do not build in V1:

- Native iOS app
- Android app
- LiDAR scanning
- Full contractor marketplace
- Permit automation
- Material ordering
- Complex 3D editor
- Heavy design system
- Full account system before needed
- Complicated dashboards before leads exist

---

## Current Platform Decision

Version 1 should be a **mobile-first web app**.

Recommended stack:

- Next.js
- React
- TypeScript
- Tailwind CSS
- shadcn/ui
- Supabase
- AI image generation API
- n8n for automation
- Stripe later for paid upgrades

Native iOS should come later for LiDAR and AR scanning.

# Soluna — UI/UX Guidelines

## Core UX Principle

Soluna should feel like:

> A fast, premium mobile web app.

Not like:

> A normal loose website.

The experience must be sturdy, snappy, simple, and visually exciting.

---

## Main UX Goal

The user should quickly feel:

> “This is easy. This is fun. My yard could actually look better.”

The emotional goal is to turn frustration or curiosity into excitement and action.

---

## Platform Feel

The site should be inspired by the tight feel of Apple’s mobile web experience:

- No loose horizontal bounce.
- No ugly side-to-side white background exposure.
- No cluttered webpage feeling.
- No slow or heavy animations.
- App-like transitions.
- One clear action per screen.
- Fast loading.

---

## Mobile-First Rules

Design for the user sitting outside with a phone.

### Required
- Big tap targets.
- Short copy.
- Visual cards.
- Sticky primary CTA when useful.
- Minimal typing.
- One decision at a time.
- Fast load on mobile data.

### Avoid
- Desktop-first layouts.
- Long text sections.
- Small buttons.
- Crowded forms.
- Multi-column mobile layouts.
- Fancy effects that slow the app.

---

## Design Direction

### Working Design Name
**Fast Premium UI**

### Optional Visual Style
**San Diego Glass UI**

This means:
- Clean
- Warm
- Premium
- Slightly glassy
- Not overdone
- Performance-first

---

## Liquid Glass / Glass UI Rules

Glass-style UI can be used, but only lightly.

### Acceptable Uses
- Main upload card
- Style cards
- Budget selector
- Floating CTA button
- Result preview cards

### Avoid
- Full-page glass effects
- Heavy blur everywhere
- Transparent text areas with low contrast
- Large animated glass backgrounds
- Anything that slows mobile performance

### Rule
Performance is more important than visual effects.

---

## Style Cards

Style selection should not be a plain list.

Each card should include:
- Style name
- Small visual reference or icon
- One short description
- Clear selected state

Recommended first style cards:

### Spanish Courtyard
Warm, classic, terracotta, olive trees, stucco-friendly.

### Modern Desert
Clean lines, gravel, agaves, low-water plants.

### Tropical Resort
Lush, green, palms, layered vacation feel.

### Family Outdoor Living
Turf, shade, seating, play space, practical layout.

### Luxury Mediterranean
Stone, lighting, elegant plants, premium outdoor living.

---

## Budget Cards

Use simple labels instead of technical budget language.

### Refresh
Small improvements. Clean, simple, lower-cost.

### Upgrade
Noticeable redesign. Better materials and stronger layout.

### Dream Yard
Full transformation. Premium features and bigger scope.

---

## Feature Chips

Feature chips should be easy to tap and visually clear.

Examples:
- Turf
- Fire pit
- Pergola
- Outdoor kitchen
- Gravel
- Pavers
- Garden beds
- Shade trees
- Lighting
- Privacy plants
- Seating
- Play area

---

## Guided Photo Upload UX

Before upload, show quick instructions:

- Stand in the corner or back edge of the yard.
- Capture as much of the yard as possible.
- Include house, fence, patio, trees, and open ground.
- Use daylight.
- Take a clear photo.

The tone should be helpful, not technical.

---

## Result Screen UX

The result screen should include:

- Original image
- AI concept image
- Short explanation
- Selected style
- Selected budget level
- Suggested next step

Primary CTA:

**Get a Real Estimate From a Local Pro**

Secondary CTA examples:
- Try another style
- Upgrade this design
- Save this concept
- Add more features

---

## Visual Style

### Preferred
- Clean white or warm neutral backgrounds
- Strong spacing
- Rounded cards
- Soft shadows
- Large visual areas
- Simple icons
- High contrast text

### Avoid
- Overly dark UI for main consumer flow
- Tiny technical labels
- Neon AI aesthetic
- Overly futuristic gimmicks
- Too much motion

---

## Copywriting Style

Use simple customer language.

### Good
- “Upload your yard.”
- “Pick your style.”
- “Choose your project level.”
- “See your yard reimagined.”
- “Get a real estimate.”

### Avoid
- “Generate photorealistic spatial landscape render.”
- “Select Mediterranean xeriscape category.”
- “Configure parameterized design output.”

---

## Performance UX Rules

- First screen should load fast.
- Avoid large JavaScript bundles.
- Compress images.
- Lazy-load results.
- Minimize background video.
- Avoid unnecessary animation libraries.
- Use skeleton states or simple loading messages.

---

## App-Like Web Behavior

The app should use:
- Fixed app shell where appropriate.
- Controlled overflow.
- No horizontal scrolling.
- Sticky bottom CTA where useful.
- Step-based flow instead of long scrolling pages.

Suggested implementation rules:
- Set page width to 100%.
- Prevent horizontal overflow.
- Use dynamic viewport units carefully.
- Test heavily on iPhone Safari.
- Test pull-to-refresh and overscroll behavior.

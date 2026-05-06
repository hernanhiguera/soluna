# Soluna — Product Requirements

## Product Goal

Build a mobile-first web app that lets homeowners upload a yard photo and generate realistic landscape design concepts.

The goal is to capture interest, create excitement, collect useful project data, and convert users into qualified leads for local contractors.

---

## Version 1 Scope

### Core Experience
The Version 1 experience should be:

**Upload photo → choose style → choose budget → pick features → generate concept → request estimate**

### Required Features

1. **Landing Experience**
   - Clear headline.
   - Short explanation.
   - Immediate call-to-action.
   - No traditional cluttered website feel.

2. **Guided Photo Upload**
   - Ask user to upload a front yard, backyard, or side yard photo.
   - Provide simple photo-taking instructions:
     - Stand back if possible.
     - Capture as much ground as possible.
     - Include house/fence/patio/trees if possible.
     - Use daylight.
     - Avoid blurry or dark photos.

3. **Landscape Style Selection**
   - Use visual cards, not plain text lists.
   - Each style should be easy to understand.
   - Recommended first style cards:
     - Spanish Courtyard
     - Modern Desert
     - Tropical Resort
     - Family Outdoor Living
     - Luxury Mediterranean

4. **Budget Level Selection**
   - Use simple customer-friendly labels:
     - Refresh
     - Upgrade
     - Dream Yard

5. **Feature Selection**
   - Use tap-friendly chips/buttons.
   - Options may include:
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
     - Seating area
     - Play area

6. **AI Concept Generation**
   - Generate 1–3 visual concepts.
   - Keep results realistic.
   - Include a short explanation of what changed.
   - Avoid designs that look impossible, fake, or wildly unrelated to the original photo.

7. **Lead Capture**
   - Collect useful lead data:
     - Name
     - Email
     - Phone
     - ZIP code
     - Address if user is ready
     - Project type
     - Budget level
     - Timeline
     - Style choice
     - Desired features
     - Uploaded photo
     - Generated concept image

8. **Contractor Match CTA**
   - After the result, offer:
     - “Get a real estimate from a local pro”
     - “Send this concept to a contractor”
     - “Get a contractor-ready design package”

---

## Optional Version 1.5 Features

1. **Top-View Property Upload**
   - User uploads a map or satellite screenshot.
   - Used for rough layout planning.

2. **Multiple Concept Options**
   - Basic version
   - Mid-range version
   - Luxury version

3. **Paid Upgrade**
   - User pays for:
     - More concepts
     - Rough material list
     - Rough budget range
     - Contractor-ready package

4. **Contractor Email Package**
   - Automatically send a lead package to an approved contractor.

---

## Lead Package Requirements

Each qualified contractor lead should include:

- Customer contact info
- Property location/ZIP
- Original photo
- AI-generated concept
- Style preference
- Budget level
- Desired features
- Timeline
- Customer notes
- Suggested project scope
- Lead score

---

## Project Data Model

Every user interaction should create a project record.

### Project
- Project ID
- User ID or anonymous session ID
- Created date
- Property ZIP
- Property address, if provided
- Project type
- Status

### Capture Data
- Uploaded photos
- Future video files
- Future LiDAR scans
- Future top-view images

### Preferences
- Style
- Budget level
- Features
- Timeline
- Notes

### AI Outputs
- Generated images
- Concept description
- Suggested scope
- Suggested next step

### Lead Data
- Contact info
- Contractor assigned
- Lead status
- Payment status
- Follow-up history

---

## Out of Scope for Version 1

Do not build these yet:

- Native iOS app
- Android app
- LiDAR scanner
- Drone scanning
- Permit automation
- Real material ordering
- Contractor marketplace
- Robot installation tools
- Full CAD/BIM exports
- Official plans or blueprints

These belong in later versions.

---

## Success Metrics

### User Metrics
- Photo upload rate
- Completion rate
- Concept generation rate
- Lead submission rate
- Paid upgrade conversion

### Business Metrics
- Cost per lead
- Contractor acceptance rate
- Lead-to-estimate conversion
- Estimate-to-job conversion
- Revenue per lead

### Product Quality Metrics
- Generation time
- Page load speed
- Mobile performance
- User satisfaction
- Number of abandoned sessions

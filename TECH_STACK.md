# Soluna — Tech Stack

## Platform Strategy

### Version 1
Start with a **mobile-first web app**.

Reason:
- Users will come from Google, Google Maps, social media, YouTube, ads, and links.
- They should not need to download an app.
- The first experience is photo upload and AI concept generation, which works well on the web.

### Later Versions
Build a native iOS app later when LiDAR and AR scanning become central.

---

## Recommended Version 1 Stack

### Frontend
- **Next.js**
- **React**
- **TypeScript**
- **Tailwind CSS**
- **shadcn/ui**
- Optional lightweight glass-style component kit

### Backend
- **Supabase**
  - Postgres database
  - Auth
  - Storage
  - Edge Functions
  - Realtime if needed later

### AI Layer
Use API-based AI services for:
- Image generation
- Image editing
- Design explanation
- Preference interpretation
- Lead summary generation

Candidate model providers:
- OpenAI
- Anthropic
- Google Gemini
- Image-specialized models as needed

### Automation
- **n8n**
  - Lead routing
  - Email notifications
  - Contractor delivery
  - CRM updates
  - Follow-up workflows

### Payments
- **Stripe**
  - Paid design upgrades
  - Contractor subscriptions later
  - Lead payment tracking later

### Email / Notifications
- Resend, SendGrid, or similar
- Twilio later for SMS

### Hosting
- **Vercel** for Next.js
- Supabase for backend/storage

---

## Future Native App Stack

### iOS App
Use when LiDAR scanning is added.

- **Swift**
- **SwiftUI**
- **ARKit**
- **RealityKit**

Native iOS is preferred for LiDAR because Apple’s AR/LiDAR tooling is strongest in native Swift.

### Android
Do not start with Android.

Add Android later only if:
- Demand is proven.
- Web app is working.
- Capture workflow can be useful without Apple LiDAR.
- Android hardware support is better understood.

---

## Future Computer Vision / 3D Stack

For later versions:

### Python Services
Use Python for:
- Computer vision
- Image segmentation
- 3D reconstruction
- Plant/tree detection
- Point cloud processing
- Material quantity estimation

### 3D / Scan Data Formats
Potential future support:
- USDZ
- OBJ
- GLB
- PLY
- LAS
- LAZ
- E57

---

## Architecture Approach

Build Soluna as a modular platform, not a patched app.

Core modules:

1. **Capture Module**
   - Photos
   - Top-view images
   - Video later
   - LiDAR later
   - Drone/pro scan later

2. **Property Model Module**
   - Yard zones
   - House footprint
   - Entries
   - Garage
   - Windows
   - Trees
   - Existing hardscape
   - Future slopes/grade/drainage

3. **Design Module**
   - Styles
   - Templates
   - Features
   - Plants
   - Hardscape
   - Lighting
   - Irrigation

4. **AI Generation Module**
   - Prompt construction
   - Image generation
   - Concept descriptions
   - Scope summaries

5. **Lead Module**
   - Contact info
   - Project details
   - Contractor routing
   - Lead status

6. **Materials Module**
   - Future bill of materials
   - Future supplier integrations
   - Future phased ordering

7. **Permit Module**
   - Future code checks
   - Future permit guidance
   - Future plan package creation

8. **Execution Module**
   - Future delivery
   - Future staging
   - Future install tracking
   - Future robotics integration

---

## Central Data Principle

Every feature should add to the same central project structure.

Do not create disconnected flows.

A project should grow over time:

- V1: photo + preferences + concept
- V2: top-view layout
- V3: design layers
- V4: LiDAR scan
- V5: material list
- V6: contractor package
- V7: permit support
- V8: ordering
- V9: installation management

---

## Suggested Core Database Tables

### users
- id
- name
- email
- phone
- role
- created_at

### projects
- id
- user_id
- title
- property_address
- zip_code
- project_type
- status
- created_at

### project_images
- id
- project_id
- image_url
- image_type
- uploaded_at

### project_preferences
- id
- project_id
- style
- budget_level
- features
- timeline
- notes

### ai_generations
- id
- project_id
- input_image_id
- output_image_url
- prompt
- model
- concept_summary
- created_at

### leads
- id
- project_id
- customer_name
- email
- phone
- lead_score
- assigned_contractor_id
- status
- created_at

### contractors
- id
- company_name
- contact_name
- email
- phone
- service_area
- specialties
- status

---

## Coding Priorities

1. Mobile performance
2. Clean architecture
3. Type safety
4. Reusable components
5. Simple user flow
6. Modular feature growth
7. Good database structure
8. Clear naming
9. Easy future native integration
10. Fast iteration

---

## Avoid

- Starting with native iOS before web demand is proven
- Overbuilding 3D scanning in Version 1
- Heavy UI libraries that slow the page
- Overly complex animations
- Hardcoding business logic into UI components
- Creating one-off data structures that cannot grow
- Making the site feel like a normal brochure website

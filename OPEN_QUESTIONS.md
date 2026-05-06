# Soluna — Open Questions

## Brand Questions

1. Is **Soluna** legally available as a company name?
2. Is the domain available?
3. Should the public-facing product name be:
   - Soluna
   - Soluna Vision
   - Soluna Yard
   - Soluna Studio
4. Should the company brand and product brand be the same?

---

## Customer Experience Questions

1. Should Version 1 generate:
   - 1 concept for free
   - 3 concepts for free
   - 1 free concept + paid upgrades

2. Should the user enter contact information:
   - Before generation
   - After seeing result
   - Only when requesting estimate

3. How much friction is acceptable before the user sees the first result?

4. Should users be allowed to generate concepts without creating an account?

5. Should results be saved by default or only after user enters email?

---

## AI Generation Questions

1. Which image model should be used first?
2. Should the system edit the original photo or generate a new concept inspired by it?
3. How realistic must the generated image be?
4. How should we prevent impossible or misleading designs?
5. Should generated designs include a disclaimer?
6. Should San Diego-specific plant/material logic be hardcoded first or handled by AI prompts?

---

## Design Style Questions

1. What are the first 5 style cards?
2. Should styles be San Diego-specific from day one?
3. Should there be separate style flows for:
   - Front yard
   - Backyard
   - Side yard
   - Full property

4. Should each style include:
   - Image reference
   - Short description
   - Estimated cost range
   - Recommended plant palette

---

## Monetization Questions

1. What is the first paid offer?
   - $49 enhanced concept
   - $149 design package
   - $299 contractor-ready package

2. Should contractors pay:
   - Per lead
   - Monthly subscription
   - Closed-job commission
   - Hybrid model

3. How will closed jobs be tracked?
4. Should customers pay before being matched with contractors?
5. Should contractors be exclusive by ZIP code or project type?

---

## Contractor Partner Questions

1. Which types of contractors should be accepted first?
   - Landscape contractors
   - Hardscape contractors
   - Irrigation contractors
   - Design-build firms
   - Tree companies

2. What quality standards should contractor partners meet?
3. Should partners be vetted manually?
4. Should customers see multiple contractors or only one match?
5. Should Soluna introduce the customer to the contractor or simply send the lead?

---

## Legal / Risk Questions

1. What disclaimers are needed for AI-generated landscape images?
2. What disclaimers are needed for rough estimates?
3. What disclaimers are needed before passing leads to contractors?
4. Should Soluna avoid saying “design plan” and instead say “concept” in Version 1?
5. What are the rules around referral fees for contractors in California?
6. Are there licensing issues if Soluna gives design recommendations but does not install?

---

## Data / Privacy Questions

1. How will user photos be stored?
2. Can users delete their photos?
3. How long should project files be kept?
4. How will customer data be shared with contractors?
5. Should users explicitly consent before their info is sent to a contractor?
6. Can generated images be used in marketing if user approves?

---

## Technical Questions

1. Which image generation provider should be used first?
2. Should Supabase or Firebase be used?
3. Should V1 require authentication?
4. Should the first app be built with Next.js App Router?
5. Which UI kit should be used for lightweight glass-inspired components?
6. How can the app prevent horizontal bounce and keep an app-like feel on iOS Safari?
7. How should uploaded images be compressed before AI processing?
8. What should the fallback be if image generation fails?

---

## Future Capture Questions

1. When should LiDAR be added?
2. Should LiDAR require a native iOS app?
3. Should video walkthrough capture be added before LiDAR?
4. Can top-view images become the main planning canvas?
5. Should drone/pro-scan data be imported later?
6. Should external LiDAR and RTK be supported through uploads rather than direct device integration?

---

## Future Platform Questions

1. Should Soluna become a contractor marketplace?
2. Should Soluna become a design software tool?
3. Should Soluna become a material ordering platform?
4. Should Soluna become a project management platform?
5. Should Soluna eventually sell to homeowners, contractors, or both?
6. Should Soluna remain local to San Diego first or expand quickly?

---

## Immediate Decisions Needed

Before coding V1, decide:

1. Final brand/domain.
2. First 5 style cards.
3. Free vs paid first generation.
4. Required lead capture fields.
5. AI image model.
6. Supabase vs Firebase.
7. Contractor lead delivery method.
8. Exact V1 landing page copy.

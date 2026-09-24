# High-end interactive research interface

## Goal
Transform the existing laboratory and specimen-report experience to closely match the supplied classified cyberpunk research interface, while retaining the current MUTANTFOOTS content, assets, and working interactions.

## What will change
- Recompose the first laboratory view into a dense full-width research console with a thin technical header, specimen selector, animated central flask, live specimen details, anatomy scan, serum reaction, experiment timeline, and trait preview.
- Drive every visible specimen field from the existing 16-item specimen collection so selecting a vial updates the image, ID, mutation, rarity, description, metadata, anatomy labels, reaction result, and trait previews together.
- Make selector vials and trait previews keyboard-accessible and clickable, with restrained scan, bubble, droplet, indicator, and panel-transition motion.
- Restyle the existing specimen shelves and report panels into the same navy, violet, pink, and cyan technical system without changing their filters, three-at-a-time pager, trait browser, registration form, or interactive object behavior.
- Preserve the existing Devil, application, interactive desk, FAQ, navigation, validation, and submission logic; only align their surrounding surfaces where needed for visual continuity.
- Keep all current image files and reuse the existing pixel specimens rather than introducing replacement artwork.

## Responsive behavior
- Desktop keeps the dense reference-like composition.
- Tablet rearranges the main report into two readable columns.
- Mobile stacks the specimen, details, anatomy, reaction, traits, and timeline while preserving all controls and keeping three shelf specimens visible per page.

## Verification
- Confirm all 16 specimens can be selected and dynamically update the report.
- Confirm shelf filters and previous/next paging still work.
- Confirm trait controls, registration validation, modal lab objects, and navigation still work.
- Check desktop and mobile layouts for clipping, overlap, missing images, and browser errors.

## Technical details
- Keep the current static HTML/CSS/JavaScript architecture and asset paths; no framework migration or backend changes.
- Implement the new console as semantic HTML, CSS variables, and reusable data-driven JavaScript rendering.
- Synchronize the served `public/` files with the existing root and `site/` copies after verification.

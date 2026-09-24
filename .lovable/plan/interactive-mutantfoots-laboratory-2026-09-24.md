# Interactive MUTANTFOOTS Laboratory

## Goal
Replace the current opening report view with the supplied laboratory artwork as the first screen. Turn the objects inside the artwork into an interactive hotspot interface, while moving the existing reports and collection sections below it.

## What will change
- Preserve `serumform.png` and both uploaded DNA images as project CDN assets, so they continue loading in previews, shared Lovable projects, and published versions without relying on localhost or GitHub hotlinks.
- Use the full laboratory artwork at the top, framed responsively without distorting it.
- Add accessible clickable hotspots over every meaningful object in the scene:
  - 6 left-rack test tubes
  - 3 upper-right test tubes
  - 3 flasks
  - 3 specimen plates/slides
  - microscope and its specimen
  - DNA diagram
  - clipboard face/profile area
  - clipboard specimen rows and bottle/vial areas
  - loose pipettes/pens where they represent lab samples
- Give every hotspot a visible focus/hover signal, clear label, keyboard support, and stable coordinates at desktop and mobile sizes.

## Context drawer behavior
- Clicking a hotspot opens an animated specimen/info drawer over the artwork.
- Opening another hotspot replaces the current content.
- Clicking outside, pressing Escape, or using the close icon dismisses it.
- Each drawer briefly shows the existing DNA-style loader before revealing its content.
- DNA hotspot: show the first uploaded flask image, then mutate into the second image.
- Microscope hotspot: load one complete specimen with image zoom in, zoom out, reset, and drag/pan controls.
- Clipboard face hotspot: show 2–3 focused face traits, then rotate to the next trait set.
- Eye/specimen hotspots: show complete relevant traits, including Hypno Spiral and Lava Beast examples already represented by the collection.
- Dragon and NFT hotspots: show representative mutant records and full trait details sourced from the linked mutantfoots files/606 CSV.
- Repeated glassware gets distinct specimen imagery and trait copy rather than duplicate drawers.

## Existing page changes
- Move the current “Method & results” report below the new interactive laboratory.
- Change “Lab report 02 · Experiment” to “Lab report 01 · Experiment” and page 1 / 4.
- Change “Lab report 01 · Abstract” to “Lab report 02 · Abstract” and page 2 / 4.
- Keep specimen shelves, mutation index, Devil section, and registration form behavior intact.
- Keep all duplicate deploy copies of the static site synchronized.

## Technical details
- Keep the implementation in the existing HTML/CSS/JavaScript structure.
- Use percentage-based hotspot geometry tied to the artwork’s native 1415×1111 canvas.
- Use a single data-driven hotspot registry for labels, content type, specimen/trait mapping, and artwork.
- Use the maintained image zoom/pan interaction pattern with cursor-centered wheel zoom and touch-safe controls.
- Preserve current visual language: pixel art, hard lab borders, lime/pink accents, DNA loading, and reduced-motion support.

## Verification
- Check desktop and mobile layouts visually.
- Test every hotspot, outside-click dismissal, Escape, hotspot switching, DNA state transition, and microscope zoom controls.
- Confirm all CDN assets load and no hotspot overlaps unrelated controls.
- Confirm the preview has no console/runtime errors and the opening artwork appears before the moved reports.

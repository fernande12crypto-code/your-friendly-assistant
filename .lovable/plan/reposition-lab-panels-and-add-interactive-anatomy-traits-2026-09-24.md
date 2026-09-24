# Reposition Lab Panels and Add Interactive Anatomy Traits

## Changes
- Move **Serum Reaction** into the left specimen/chamber column, directly below “Live containment · M1”.
- Move **Traits Preview** into Serum Reaction’s current right-side panel position.
- Keep all six traits—Eyes, Mouth, Body, Overlay, Costume, Weapon—in one compact panel by reducing preview tiles as needed.
- Turn the anatomy scan into six interactive target zones. Hover, keyboard focus, or click will reveal a technical arrow callout with that specimen’s exact trait name.
- Show a lab-style unavailable message when a specimen has no costume or weapon.
- Keep specimen switching synchronized across the chamber, anatomy labels, reaction image, details, and trait previews.

## Layout behavior
- Desktop: reaction sits beneath the containment chamber; traits occupy the right-side panel as one six-item grid.
- Tablet/mobile: panels stack cleanly, all six trait tiles stay together, and anatomy targets remain touch-accessible.

## Validation
- Verify all 16 specimens, especially missing costume/weapon states.
- Check hover, focus, click, desktop/mobile layout, overflow, console errors, and deploy output.

# Prototype and finish contract

Read this reference when building variants, selecting a direction, or finishing the chosen demo.

## Prototype comparison

Build one prototype shell with a small, visually neutral switcher. Keep the comparison fair:

- identical product goal, content, data, and core action;
- identical target viewport and basic responsive behavior;
- one named design hypothesis per variant;
- realistic labels and values, with no lorem ipsum;
- only enough behavior to judge navigation, hierarchy, glass treatment, and the core interaction.

Two variants are sufficient when the meaningful design space has two clear poles. Use three when a genuinely different middle or alternate interaction model exists. Never add a weak third variant to reach a number.

## Suggested Apple + Liquid Glass directions

Use these only as starting points; adapt their names and characteristics to the product.

- **Airy Frost** — light-first, generous whitespace, thin functional glass, quiet color, typography-led hierarchy.
- **Spatial Glass** — layered depth, colored atmosphere behind refractive controls, stronger foreground/background separation.
- **Dark Instrument** — dark precision surface, compact control clusters, tinted glass, focused highlights, tool-like confidence.

The variants must remain recognizably the same product. Liquid Glass intensity can differ, but every variant should use it purposefully.

## Selection handoff

The user may choose one variant or combine explicit parts. Restate the resulting direction as a single coherent system; do not mechanically paste incompatible pieces together. Call out any requested combination that creates a hierarchy, contrast, or interaction conflict.

Then resolve only remaining decisions:

- one signature interaction or none;
- motion intensity and whether scrolling participates;
- target browser/device and presentation path;
- visible loading, empty, success, or error state, if relevant.

## Final-motion budget

Motion must explain, connect, or acknowledge. Default to:

- immediate press feedback;
- origin-aware popover, sheet, or panel transitions;
- continuity for the primary state change;
- at most one signature moment for the showcased product idea;
- reduced-motion equivalents.

Avoid adding motion to frequently repeated navigation merely for decoration. Avoid slow page-wide entrance sequences in utility interfaces.

## Final QA

Verify the actual rendered UI, not only source code:

- target viewport and one adjacent responsive width;
- primary interaction and reverse/exit path;
- readable text over every glass state;
- no unintended nested live refraction;
- unsupported-effect fallback;
- reduced motion;
- keyboard focus for showcased controls;
- console errors and obvious performance regressions.

The final demo should open directly into the selected experience. Remove or hide the variant switcher unless the user wants to keep it for the mentor presentation.

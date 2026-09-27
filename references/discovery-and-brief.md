# Discovery and design brief

Read this reference only during clarification and design-direction work.

## Question priorities

Ask from the highest unresolved tier. Do not ask for information already supplied or safely inferable.

Question count is adaptive. A complete request may need no follow-up; a narrow gap may need one question; a complex or ambiguous product may need several questions over multiple turns. Group related questions so they are easy to answer, but do not use a fixed per-turn maximum.

## Understanding gate

Before proposing the design brief, estimate confidence across these dimensions:

- the mentor decision the demo must support;
- the primary user, job, and scenario;
- the demo scope, content, and required interactions;
- the user's visual preferences, desired feeling, and dislikes;
- the target device, browser, stack, and meaningful constraints.

Continue clarification while any material dimension is uncertain. Proceed when overall understanding is at least about 95% and no unresolved point is likely to change the design direction. Aim for full understanding when additional questions can realistically achieve it. If only low-impact uncertainty remains, state the assumption in the brief instead of asking for certainty that does not affect the outcome.

### Tier 1 — The product decision

- What should the mentor understand, approve, reject, or compare after the demo?
- Who is the primary user and what are they trying to accomplish?
- Which page or short flow proves the idea best?

### Tier 2 — The demonstration

- Is the target desktop, mobile, or responsive, and what viewport will be shown?
- What content, data, or states must look real?
- Which controls must actually work for the idea to be credible?

### Tier 3 — Direction and constraints

- What feeling should the interface create: calm, precise, premium, playful, technical, or another named quality?
- Are there brand assets, colors, examples, or disliked patterns to respect?
- What is the time budget, stack constraint, or browser used for the presentation?

### Overlooked considerations

Raise only those that change the demo: privacy or trust, loading/empty/error states that appear in the showcased flow, touch versus pointer behavior, accessibility, localization, unusually long content, or a key responsive transition.

## Design brief format

Keep the brief concise enough to approve in one reading.

### Decision to support

One sentence describing what the mentor should be able to judge.

### Audience and scenario

Primary user, context, and the representative task.

### Demo scope

Pages, core interaction, realistic content, presentation device, and explicit non-goals.

### Design principles

Three to five project-specific principles. Include how Apple character appears through clarity, hierarchy, restraint, direct manipulation, spatial continuity, typography, or material.

### Visual system

State the light/dark bias, palette roles, typography character, spacing rhythm, shape language, and Liquid Glass roles. Do not reduce the direction to a list of CSS values.

### Information structure

Describe the page hierarchy and primary action. A tiny text wireframe is useful when layout choices are otherwise ambiguous.

### Prototype directions

Name 2–3 variants and the axis each explores. Keep product scope constant. Good axes include density, spatial hierarchy, navigation model, content emphasis, or glass intensity. Color-only variants are insufficient.

### Interaction intent

List only the interactions needed to understand the concept. Reserve final timing and easing until a variant is selected.

### Risks and assumptions

Record any assumption that could materially change the result and any important browser, performance, or content limitation.

End with a direct approval question. Do not begin implementation in the same response.

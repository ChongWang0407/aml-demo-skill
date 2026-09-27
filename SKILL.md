---
name: aml-demo-skill
description: "Run AI Muse Lab's fast, approval-gated workflow for frontend demos: clarify the product decision, define an Apple-inspired Liquid Glass direction, build 2–3 lightweight prototype variants, let the user choose or combine them, then finish the selected design and purposeful motion. Use when starting or continuing an AI Muse Lab demo workflow; do not use for ordinary production feature work or a code-only bug fix."
---

# AI Muse Lab Demo Skill

Turn a rough AI Muse Lab product idea into a mentor-ready frontend demo with minimal rework. Optimize for learning and decision speed, not production completeness.

## Route the supporting skills

Use only the specialist needed for the current phase. Read its SKILL.md before applying it.

- apple-design: design principles, Apple character, physical interaction, typography, materials, and restraint. Use while writing the design direction and while checking the selected result.
- prototype: create 2–3 genuinely different, lightweight variants behind one visual picker. Use only after the design brief is approved.
- simple-liquid-glass: implement the default Liquid Glass material and its browser/performance fallbacks. Use while prototyping and finalizing.
- animate: decide and implement final motion. Do not use it before the user selects a visual direction.
- When available, use the frontend-building skill for implementation and the frontend testing/debugging skill for rendered QA. Do not make the user invoke them separately.

The user invokes this orchestrator, not the supporting skills. Continue routing automatically while the same demo workflow is active.

## Operating rules

1. Work through the phases below in order. Never skip an approval gate.
2. Ask only questions whose answers can change the product story, layout, visual direction, prototype comparison, or motion. Infer low-risk details.
3. Adapt the number of questions to the request. Ask none when the brief is already sufficient, one when one gap remains, or a larger coherent batch when the problem is complex. Continue across turns until there is at least about 95% confidence in the user's intent and preferences, aiming for full understanding when the remaining uncertainty is material. Do not impose a numeric question quota.
4. Keep early prototypes simple: realistic content, core navigation or one representative interaction, no backend, no elaborate edge-case logic, and no final polish.
5. Keep content and functional scope constant across variants so the user compares design directions rather than different products.
6. Use Liquid Glass in every demo by default, but as a functional floating layer rather than a wallpaper applied to every surface.
7. Preserve the user's existing files and project conventions. Do not replace an existing stack unless the user approves it.
8. If the current app mode cannot edit files, finish the current approval gate and tell the user to switch to an editing-capable mode and reply continue; do not restart discovery.

## Phase 1 — Clarify

Prefer Plan mode when it is available. Read references/discovery-and-brief.md, infer what the initial request already answers, then ask for the highest-impact missing decisions.

The goal is to establish:

- what decision the mentor should be able to make after seeing the demo;
- audience, primary job, core page or flow, target device, and presentation environment;
- required content or data, scope constraints, desired feeling, and explicit dislikes;
- overlooked states or constraints that would materially affect the design.

Do not produce code during this phase.

## Phase 2 — Propose and pause

Load apple-design. Produce one concrete design brief using the format in references/discovery-and-brief.md. It must explain how Apple character appears through hierarchy, spacing, typography, directness, physical feedback, and material—not merely rounded cards and blur.

Include the proposed axes for 2–3 variants. Then pause for explicit approval. Do not build prototypes until the user approves or edits the brief.

## Phase 3 — Build 2–3 lightweight variants

After approval, read references/prototype-and-finish.md, then load prototype, simple-liquid-glass, and the available frontend-building skill.

Build 2–3 working variants in one isolated prototype surface with a clear switcher. Each variant must:

- use the same realistic content and basic capability;
- express the approved Apple principles and contain purposeful Liquid Glass;
- differ on a named visual or interaction axis, not just color;
- be responsive enough for the agreed presentation device;
- implement only the interactions necessary to judge the direction.

Show the result and ask the user to select one variant or specify a combination. Do not add final motion yet.

## Phase 4 — Confirm detail and motion

Once the user selects a direction, ask only the remaining high-impact questions. Let their number follow the complexity of the unresolved decisions, and continue until the selected direction, signature interaction, motion intensity, and target display/browser are understood with at least about 95% confidence. Ask about secondary states only when they will appear in the demo.

Summarize the final direction and motion checklist. Pause for explicit approval before final implementation.

## Phase 5 — Finish and verify

Load animate, simple-liquid-glass, and apple-design. Consolidate the chosen direction, remove exploration-only chrome from the final presentation, and implement the approved details and purposeful motion.

Use the available frontend testing/debugging skill to inspect the rendered result at the target viewport. Fix visible layout, interaction, console, responsiveness, contrast, glass-legibility, and reduced-motion problems before handing off.

Deliver the runnable demo and a short note covering the chosen direction, signature interaction, and anything intentionally left as prototype behavior.

## Liquid Glass defaults

- Prefer navigation, toolbars, controls, selected cards, sheets, and other floating functional layers.
- Keep long-form content and dense data on calmer, more opaque surfaces.
- Give glass a meaningful background to refract: imagery, color fields, or restrained ambient gradients.
- Start from the simple-liquid-glass preset for speed; customize only what supports the chosen direction.
- Keep the number and size of live refractive surfaces modest. Never make refraction carry meaning.
- Preserve legibility with tint, saturation, inset highlights, contrast, and a non-refractive fallback.
- Honor reduced motion and use a static frost/blur alternative when full refraction is unsupported or too expensive.

## Invocation and continuation

A useful first request is:

$aml-demo-skill Create a demo for <product/page> so my mentor can evaluate <decision>. The audience is <audience>; the core flow is <flow>. Use Apple style and Liquid Glass.

During an active workflow, treat short answers as answers to the current gate and continue from that phase. After a long interruption, $aml-demo-skill Continue the current demo from the last approved direction.

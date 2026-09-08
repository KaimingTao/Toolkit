# Memo — 2026-09-07

## Decision: use GPT-6 Astra for the full implementation

We will use GPT-6 Astra as the primary implementation model for rebuilding the reference launch-page experience. The work includes the responsive front end, dynamic visual treatments, accessible interactive modules, performance tuning, and final browser QA.

## Why this model

The implementation requires coordinated work across visual design, client-side interaction, content structure, media handling, and verification. GPT-6 Astra is the appropriate default because it is intended for hard end-to-end coding work and supports the tool-driven workflow needed to inspect, build, test, and refine a complete experience.

## Implementation expectations

- Build the page from an original design implementation; do not copy proprietary source code, branded media, or long-form page copy from the reference.
- Preserve the reference’s design principles: editorial hierarchy, large display type, restrained palette, visual demonstrations, data-led modules, and long-form storytelling.
- Start with semantic, responsive HTML and CSS. Add JavaScript only where it delivers required interaction or animation.
- Keep animations performant and optional. Honor `prefers-reduced-motion` and provide static or controllable alternatives.
- Make all data visualizations readable without motion or color alone; include text/table equivalents where needed.
- Keep all new assets and dependencies explicit. Prefer self-contained or locally stored assets during the initial prototype.

## GPT-6 Astra operating guidance

Use the Responses API with `model: "gpt-6-astra"` for tool-enabled implementation work. Begin ordinary build and iteration tasks at `reasoning.effort: "high"`; increase to `xhigh` or `max` only for difficult visual debugging, architecture decisions, or persistent defects. Use `low` for mechanical edits and routine checks.

Give the model the project brief, target routes, acceptance criteria, visual references it is authorized to use, and the repository’s instructions. Ask it to work through the complete loop: inspect, implement, run targeted checks, test in a browser, fix defects, and report the verified result.

The model should be explicitly instructed to make reasonable implementation decisions where the brief is incomplete, while pausing only for consequential product decisions or external publishing actions.

## Delivery checkpoints

1. **Foundation** — page shell, responsive grid, typography tokens, theme, navigation, and content structure.
2. **Visual system** — hero animation, media frames, section transitions, and responsive presentation.
3. **Interactive modules** — tabs, carousels, charts, and media controls, all accessible by keyboard.
4. **Performance and accessibility** — lazy media, layout-stability controls, reduced-motion mode, semantic data fallback, and contrast/focus review.
5. **Browser QA** — check desktop and mobile layouts, keyboard flows, scroll behavior, console errors, and visual regressions before handoff.

## Definition of done

The implementation is complete when the target experience is responsive, visually coherent, accessible, and stable in supported browsers; interactions work without console errors; meaningful content remains available without JavaScript; and the final result has been reviewed against the agreed visual and functional acceptance criteria.

## Reference

The current official OpenAI documentation says to set `model` to `gpt-6-astra` in a Responses API request. It supports tool-based workflows, structured outputs, streaming, computer use, and other implementation capabilities; it does not support `reasoning.effort: "none"`. [OpenAI’s GPT-6 Astra model guidance](https://developers.openai.com/api/docs/guides/latest-model)

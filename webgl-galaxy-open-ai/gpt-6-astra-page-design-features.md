# Design features: GPT-6 Astra launch page

Reference: [openai.com/index/gpt-6-astra](https://openai.com/index/gpt-6-astra/)

## Overall design direction

The page is an editorial product-launch experience: sparse at the top, highly visual through the middle, and increasingly information-dense toward the end. It uses large typography, spacious pacing, restrained color, and media-led examples to make a technically complex announcement feel approachable.

## Visual system

- **High-contrast neutral palette.** Light, paper-like sections are paired with near-black media and data sections. The limited palette keeps focus on product demonstrations and benchmark graphics.
- **Oversized editorial typography.** The launch message and section titles use very large display text with tight tracking and short line lengths. This creates an immediate, confident hierarchy.
- **Generous whitespace.** Wide margins and long vertical gaps create deliberate pauses between narrative beats, evidence, and demonstrations.
- **Fine rules and compact labels.** Thin dividers, small all-caps/utility-style labels, and compact metadata provide structure without competing with headings.
- **Image and video as content blocks.** Demonstrations are not decoration; they operate as proof points for specific claims and use clear surrounding labels.

## Layout patterns

- **Global header and utility navigation** provide persistent access to major site areas, account actions, search, locale, and footer navigation.
- **Hero-to-article transition** moves quickly from product framing into supporting narrative rather than using a traditional marketing-card layout.
- **Full-bleed media modules** break up long prose and give demonstrations enough visual scale to be legible.
- **Alternating narrative rhythm** repeats a pattern of heading, explanation, evidence, and example, helping readers scan a long page.
- **Grid-based comparison areas** organize benchmarks and capability examples into aligned, repeatable modules.
- **Data tables at the end** provide a detailed reference layer after the higher-level visual story.

## Interaction and motion features

- **Benchmark selectors/tabs** let readers switch among named evaluations without leaving the section.
- **Media demonstrations** show short, task-based examples such as design, document, software, and research workflows.
- **Quote carousel behavior** is indicated by a visible item count and source controls; it condenses social proof while retaining multiple perspectives.
- **Expandable or contextual explanation patterns** support dense charts, benchmarks, and methodology without placing every detail in the first reading path.
- **Scroll-led storytelling** uses stacked sections and alternating media to make progression feel sequential rather than dashboard-like.

## Information-design features

- **Capability claims are paired with evidence.** Major sections introduce a capability, provide an explanation, then attach benchmarks, demonstrations, or customer commentary.
- **Specific labels reduce ambiguity.** Benchmark names, application domains, and example-task labels make visual modules easier to interpret.
- **Methodology lives alongside outcomes.** Detailed notes and footnotes qualify measurements and comparisons instead of leaving them as uncontextualized headline numbers.
- **Progressive depth.** A reader can understand the top-level story by scanning headings and media, then move into tables and notes for the full detail.

## Accessibility-minded features to preserve

- A skip-to-content link is exposed before the main navigation.
- Headings and visible section labels provide a meaningful document outline.
- Tables and footnotes make performance data available as text, rather than only as a visual chart.
- Interactive selectors, carousel controls, and media should remain keyboard operable and have non-motion/text alternatives.

## Reusable design recipe

For a similar launch page, use one primary visual idea per section, keep the typographic hierarchy stronger than the decorative treatment, and reserve animation for explaining a concept or demonstrating a task. Put all measurements in real text/table data, load media progressively, and offer reduced-motion alternatives.

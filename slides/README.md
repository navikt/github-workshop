# Workshop Slides

The slides follow the [two-hour workshop outline](../WORKSHOP-OUTLINE.md), including a 10-minute break. Files and commits come first; branches, an own-repository PR, and fork-based contributions form the second half. Only further-learning topics are in the appendix.

## Publishing

The existing [Pages workflow](../.github/workflows/pages.yml) publishes the contents of `slides/` as the site root.

**Expected URL after deployment:** https://navikt.github.io/github-workshop/

In repository **Settings → Pages**, choose **GitHub Actions** as the source. The workflow runs on changes under `slides/` pushed to `main`, or through its manual trigger. Publishing and repository settings changes are separate from editing these materials; confirm authorization before performing them.

Core activity slides contain their own instructions and practice text; participants do not need to open a numbered exercise. Because only `slides/` is uploaded, optional reference links point to GitHub rather than files outside the deployment artifact.

## Local presentation

Open `index.html` in a browser, or serve this directory:

```bash
cd slides
python3 -m http.server 8000
```

Then open http://localhost:8000/.

**Internet is still required:** Reveal.js and its plugins load from jsDelivr; Aksel CSS and fonts load from Nav CDN. Local HTML alone is not an offline backup. Rehearse on the presentation device and prepare an offline PDF and exercise copies beforehand.

## Aksel styling

The presentation loads the version-pinned Aksel stylesheet directly from Nav CDN:

```html
<link rel="stylesheet" href="https://cdn.nav.no/aksel/@navikt/ds-css/8.23.0/index.min.css">
```

It includes design tokens, the Source Sans 3 font, and Aksel's baseline. No React dependency, build step, or copied token definitions are needed. Reveal.js supplies slide layout and navigation; the former Night theme and its Google Fonts imports are removed.

The document uses Aksel's `dark` class on `<html>`. Custom styles use semantic `--ax-*` tokens for backgrounds, text, borders, diff colors, spacing, and radii, including the SVG diagram. Typography uses Aksel's font family, weight, size, and line-height tokens with presentation-scale multipliers to remain readable on a projector. Diagram coordinates and proportional layout remain presentation-specific.

Links are underlined, keyboard focus is visible, and reduced-motion preferences disable slide/background transitions and CSS animations. Added and removed diff lines keep their `+`/`-` symbols rather than relying on color alone.

To change color mode, replace the root `dark` class with `light`; do not swap in hardcoded colors. When upgrading Aksel, update the exact CDN version and verify the referenced tokens together. Nav CDN does not resolve semver ranges.

See Aksel's [CSS-import and CDN documentation](https://aksel.nav.no/grunnleggende/kode/css-import).

## Controls

| Key | Action |
|---|---|
| Space | Advance through slides, including vertical appendix slides |
| Arrow keys | Navigate horizontally or vertically |
| Esc | Overview |
| F | Fullscreen |
| S | Speaker notes |
| B or . | Blank screen |
| ? | Help |

Speaker notes include timeboxes, safety reminders, prediction questions, and explicit browser demo cues.

## Visual demos

Concepts appear just before use. Diagrams introduce Git vs. GitHub, persistent copies after an upload, branch isolation, PR direction, and cross-repository ownership. Each diagram has a text caption and should be described aloud.

Use **explain the task → optional demo or independent start → leave the task slide up → help and verify**. Each activity slide shows the actions, any exact text to enter, a completion check, and the work period after the demo. Numbered exercises remain optional detailed references, not required navigation.

Explain the task before switching to the browser. Say the goal and completion check; point to the steps and sample text. Participants may start immediately or watch the short demo. Notes specify what to open, show, ask, and verify. If there is only one projected display, share the slide URL first so independent participants can keep the instructions open; use a second display or side-by-side view when available.

After the demo, return to the same activity slide, announce the work period and finish time, and leave it visible. Use that time for individual help and questions rather than continuing the presentation. Keep all steps and sample text visible, with no fragments. If no one needs the demo, use its time for practice, not an earlier move to the next stage.

Titles show the **total stage time**, including its briefing, optional demo, and work/help period. The footer shows how long to work after the demo. Speaker notes and the [facilitator timing table](../FACILITATOR-GUIDE.md#demo-and-work-periods) give the split. Advancement stays manual; no automatic countdown or slide change is required.

Rehearse these checkpoints:

- Editor → commit dialog → saved file and message.
- Typo correction → new diff → earlier version still available.
- Draft → main → draft, showing the edit only on the draft.
- PR source/destination selectors → original main unchanged before merge, updated afterward.
- Original and fork with different owners → fork commit leaves original unchanged → incoming review and merge update original.

Official GitHub Docs illustrations are bundled under [`assets/github-docs/`](assets/github-docs/) for history, branch creation, PR review, merging, and fork comparison controls. Use the relevant UI landmarks briefly before the task, not instead of leaving its instructions visible. The more detailed merge-commit diagram is an optional appendix reference; it does not interrupt the core practice flow.

The images are unchanged, locally hosted documentation examples, not captures of the workshop or participants. Captions and notes identify different example branch names and counts. Keep them intact rather than recoloring them to match Aksel; presentation framing remains token-based.

Prepare sanitized screenshots of the cafe demo states as an additional backup. Use fictional content, zoom into relevant controls, and keep text instructions available. The [facilitator guide](../FACILITATOR-GUIDE.md) contains the detailed scripts.

### Image attribution

The bundled illustrations are **GitHub Docs, by GitHub and contributors, CC BY 4.0**. [Asset credits](assets/github-docs/README.md) record the exact upstream revision, source links, license, and reuse details. This is separate from the workshop's MIT license. Keep the slide credits and linked attribution when redistributing or exporting slides.

The Slack activity requires a confirmed channel and audience, assigned recipients, and an alternative for anyone who cannot or does not want to post a public practice repository. The slides do not create or publish anything in Slack.

## Humor and images

The opening meme has its own slide, a visible text question, and descriptive alt text. It is not an overlay and contains no essential task instructions. Read the question aloud; skip the image if it does not load.

The image is externally hosted and may be unavailable. Do not rely on it for the lesson. Only add a local replacement if you have permission to redistribute it; include attribution where required. Keep jokes understandable without prior Git knowledge and avoid covering instructions or making beginners the target.

The filename joke remains in the history speaker notes; the participant-facing slide shows the official history control.

## Customization

Edit `index.html` to change the title, example, or links. Keep the core outcome and timings aligned with the outline and exercises. Task slides should remain readable while participants work; do not hide their steps behind fragments or memes.

For a different repository, update the GitHub links and deployment URL together.

# Workshop Slides

The slides follow the [two-hour workshop outline](../WORKSHOP-OUTLINE.md), including a 10-minute break. Files and commits come first; branches, an own-repository PR, and fork-based contributions form the second half. Only further-learning topics are in the appendix.

## Publishing

The existing [Pages workflow](../.github/workflows/pages.yml) publishes the contents of `slides/` as the site root.

**Expected URL after deployment:** https://navikt.github.io/github-workshop/

In repository **Settings → Pages**, choose **GitHub Actions** as the source. The workflow runs on changes under `slides/` pushed to `main`, or through its manual trigger. Publishing and repository settings changes are separate from editing these materials; confirm authorization before performing them.

Because only `slides/` is uploaded, the slides link to exercises on GitHub rather than using relative paths to files outside the deployment artifact.

## Local presentation

Open `index.html` in a browser, or serve this directory:

```bash
cd slides
python3 -m http.server 8000
```

Then open http://localhost:8000/.

**Internet is still required:** Reveal.js, its theme, and its plugins load from a CDN. Local HTML alone is not an offline backup. Rehearse on the presentation device and prepare an offline PDF and exercise copies beforehand.

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

Visible **Live demo** cues identify when to switch to the browser. Notes specify what to open, what to show/change, what to ask, and the visible result to verify. Return to the task slide while participants work.

Rehearse these checkpoints:

- Editor → commit dialog → saved file and message.
- Typo correction → new diff → earlier version still available.
- Draft → main → draft, showing the edit only on the draft.
- PR source/destination selectors → original main unchanged before merge, updated afterward.
- Original and fork with different owners → fork commit leaves original unchanged → incoming review and merge update original.

Prepare sanitized screenshots of those states for backup; they are not included as purported live GitHub captures. Use fictional content, zoom into relevant controls, and keep text instructions available. The [facilitator guide](../FACILITATOR-GUIDE.md) contains the detailed scripts.

The Slack activity requires a confirmed channel and audience, assigned recipients, and an alternative for anyone who cannot or does not want to post a public practice repository. The slides do not create or publish anything in Slack.

## Humor and images

The opening meme has its own slide, a visible text question, and descriptive alt text. It is not an overlay and contains no essential task instructions. Read the question aloud; skip the image if it does not load.

The image is externally hosted and may be unavailable. Do not rely on it for the lesson. Only add a local replacement if you have permission to redistribute it; include attribution where required. Keep jokes understandable without prior Git knowledge and avoid covering instructions or making beginners the target.

The text-only filename joke introduces history without an external image dependency.

## Customization

Edit `index.html` to change the title, example, or links. Keep the core outcome and timings aligned with the outline and exercises. Task slides should remain readable while participants work; do not hide their steps behind fragments or memes.

For a different repository, update the GitHub links and deployment URL together.

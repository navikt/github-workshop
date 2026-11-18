# GitHub from Scratch - Workshop Outline

**Background:** Beginners learn GitHub in the browser by updating one fictional cafe handbook, first alone and then together. Introduce concepts when participants need them, not as a glossary to memorize.

**Desired result:** Each participant can create and edit a repository, explain a commit's diff, merge a PR in their own repository, and exchange a contribution through a fork. They can explain why private or internal visibility does not make sensitive content safe to upload.

**Participants and roles:** Participants alternate between contributor and maintainer. The facilitator demonstrates, checks understanding, manages time, and assigns pairs or a contribution ring. Assign the facilitator and helpers before the session.

**Duration:** 2 hours, including a 10-minute break.

**Agenda:**

| Elapsed time | Session | Type | Facilitator notes |
|---|---|---|---|
| 00:00-00:15 | Welcome, Git vs. GitHub, and safe practice | Information / discussion | Two-minute origin story; show the outcome without teaching PR mechanics yet. Establish the data rule. |
| 00:15-00:20 | Account setup | Information / practice | Explain the task; optional quick demo while others start. Leave instructions visible for practice and help. |
| 00:20-00:25 | Create a repository | Information / practice | Exercise 02, Part 1. Explain repository, README, and visibility at this point. |
| 00:25-00:35 | Edit/add a file and commit | Information / practice | Exercise 02, Part 2. Show the editor, saved file, and commit message. |
| 00:35-00:45 | History and recovery | Information / practice | Exercise 02, Part 3. Introduce history and diff using the edit participants just made. |
| 00:45-00:55 | Independent edit and catch-up | Practice | Exercise 02, Part 4. No live demo first; helpers support setup delays. |
| 00:55-01:05 | Break | Break | Protect the break. |
| 01:05-01:25 | Branch and PR in own repository | Information / practice | Exercise 03 (8 min), then 04 (12 min). Check branch isolation before introducing PRs. |
| 01:25-01:30 | Share links and assign partners | Discussion / coordination | Exercise 05, Part 1. Use the confirmed Slack channel; remind everyone of public visibility and assign recipients. |
| 01:30-01:50 | Fork, contribute, review, and merge | Information / practice | Fork/edit (8 min), send PR (5 min), review/merge (7 min), each including briefing, optional demo, and work/help. |
| 01:50-02:00 | Check results, parked questions, reflection | Discussion / decision | Verify the incoming merge, address questions, and choose a dated next practice task. |

## Teaching rhythm

**Introduce one concept → explain the task → optional demo or independent start → work with instructions visible → verify.**

Activity slides are self-contained: steps, exact practice text, completion check, and timebox. Numbered exercises are optional detailed references. Explain the goal and completion check before the browser demo so participants can start independently. They do not have to watch or wait for the demo.

Each stage's advertised time includes its briefing, optional demo, and work/help period. Return to the same task slide after the demo, announce the finish time, and leave it projected while the facilitator helps or answers questions. Share the slide URL for independent access during browser demos. If a demo is skipped, give its time to practice. See the [timing table](FACILITATOR-GUIDE.md#demo-and-work-periods).

| Stage | Introduce now | Visual reinforcement and checkpoint |
|---|---|---|
| Welcome | Git tracks versions; GitHub hosts projects and collaboration | Two boxes and a short 2005/2008 timeline. No branch/fork terminology test. |
| Before uploading | Private is not a promise of secrecy | Upload → history → downloaded copy. Remove the original from the diagram; the other copies remain. |
| Repository creation | Repository, README, visibility | Show owner/name in the URL and the visibility label. |
| Editing | Commit | Editor → commit dialog → saved file and commit message. Ask whether typing alone records a commit. |
| History | History and diff | Compare the typo and correction; point to `+` and `-`. Ask whether the correction erased the old commit. |
| Own PR, first step | Branch as a separate draft | Switch draft → main → draft. Ask whether the draft edit is visible on main. |
| Own PR, next step | PR as a proposal; merge as acceptance | Match from/to diagram to compare/base selectors. Ask whether opening a PR changes main. |
| Partner contribution | Fork as a separate repository | Show two owners and URLs. After a fork commit, verify the original is unchanged; after merging, verify it changed. |

Use only the relevant diagram or official UI landmark during a brief concept introduction; do not advance through extra slides during the work period. Detailed scripts and accessibility adaptations are in the [facilitator guide](FACILITATOR-GUIDE.md).

## Safety and sharing

Before any upload, ask: **would it be harmful if this became public?** If yes, stop and check organizational rules and get guidance, even for private or internal repositories. Access restrictions are not a guarantee against mistakes, account compromise, or copies. Deleting a file may not remove its history or copies already distributed.

Use fictional content only. If sensitive data is uploaded accidentally, stop and report it through the organization's incident process; deleting the file alone is not a fix.

The standard fork exercise uses public, disposable practice repositories with participants' agreement. Slack is a link-exchange surface, not a privacy boundary for those repositories. Confirm the channel, membership, and a non-posting/private-repository alternative before facilitating. Do not contact participants or post on their behalf without authorization.

## Completion evidence

Participants can show or describe their file, commit diff, merged own-repository PR, outgoing fork PR, and merged incoming contribution. Opening a PR is not the final step: the recipient reads it, leaves a useful comment, merges it, and both verify the original file.

With an access alternative or unresolved setup problem, state which steps were observed or assisted rather than claiming independent completion. Participants choose one further edit or PR, a date within seven days, and verify it through a diff they can explain.

## Scope and pacing

Five minutes is the target for setup and repository creation, not a promise about account verification. Encourage pre-work and use the catch-up buffer. Keep fork edits to one menu item or sentence. Defer conflicts, fork syncing, merge strategies, local Git, and automation.

Issues and [Exercise 06](exercises/06-practical-applications/) are optional follow-up material. If behind, reduce explanation and defer optional questions; do not silently drop review/merge verification or the closing reflection. Record unfinished hands-on steps honestly.

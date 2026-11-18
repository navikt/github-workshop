# GitHub from Scratch - Facilitator Guide

**Background:** Beginners learn by changing one fictional cafe handbook, first alone and then together. The browser workflow is the focus, not Git internals.

**Desired result:** Participants can explain a diff, merge a PR in their own repository, and exchange a fork contribution as both contributor and maintainer. They understand that private or internal visibility does not guarantee secrecy.

**Agenda:** Follow the [two-hour outline](WORKSHOP-OUTLINE.md). Exercises 01-05 are core; Exercise 06 and issue practice are optional. The first 55 minutes cover files and commits, followed by a 10-minute break, 45 minutes of collaboration, and a 10-minute close.

## Confirm before facilitating

- Assign the facilitator and helpers; confirm group size, format, language, and accessibility needs.
- Confirm the Slack channel, its audience, and participants' ability to use it. These materials do not authorize creating a channel, sending invitations, or posting for participants.
- Agree an alternative for anyone who cannot post a URL or does not want to publish their own practice repository. Prepare public demo targets with fictional content and a maintainer who can review contributions.
- Confirm what may be retained and who has access. Do not record the session or export participant activity by default.
- Request account creation and email verification beforehand if practical, using an authorized communication route. A five-minute setup slot cannot guarantee successful verification.

## Preparation and visual teaching pattern

- Rehearse Exercises 01-05 in disposable repositories. For the cross-fork demo, arrange a second account or consenting co-facilitator as the other owner.
- Test fork creation with a different name: participants already own `cafe-handbook`, so their partner's fork needs an available name such as `cafe-handbook-contribution`.
- Prepare two labeled browser tabs/windows: **original owner/repository** and **contributor/fork**. Zoom in enough that the owner, branch, and changed lines are readable.
- Use a separate demo profile; hide notifications, personal tabs, email, and account settings. Never project credentials, recovery codes, or verification messages.
- Use the bundled [official GitHub Docs illustrations](slides/assets/github-docs/) as UI landmarks within the existing teaching blocks. Their repository names, branch names, counts, and visibility labels are examples, not exercise values.
- Prepare sanitized screenshots of the cafe editor, diff, and merged file as an additional backup. Use only fictional content. Do not claim a screenshot walkthrough is hands-on completion.
- Test projection, network, links, slide navigation, and speaker notes. The opening meme is optional; the diagrams and demo notes carry the learning points.
- Keep accessible text instructions available. Explain diagrams aloud and identify diff lines by `+` and `-`, not color alone. Local HTML still uses a CDN; prepare an offline PDF and exercise copies if needed.

Use **introduce one concept → explain the task → optional demo or independent start → work with instructions visible → verify**. Introduce terminology at the point of use. Each activity slide contains the steps, practice text, completion check, and timebox; the numbered exercises are optional detailed references.

Explain the goal and completion check, then point to the written steps and practice text **before opening the browser**. Say: "You can start now using these instructions, or watch the short demo first." Participants do not have to wait or follow each click. Share the slide URL so they can keep the task open while the projector shows the browser; use a second display or side-by-side view if available.

After the optional demo, **return to the same task slide**, announce the work period and finish time, and leave it visible. Stop presenting; circulate or answer questions. Do not introduce the next concept, hide steps behind fragments, or replace the task with a countdown-only screen. Keep a private help route. If a demo is skipped, give its time to practice rather than advancing early.

Each demo cue has four parts: **open**, **change/show**, **ask**, **visible proof**. The checkpoints below describe what to show, not just what to say.

### Demo and work periods

These are splits of the existing stage budgets, not additional time. The briefing includes the just-in-time concept and task explanation; show only the visual needed for that explanation. The final column is how long the task slide stays up after the demo for work, questions, and help.

| Activity | Total | Brief | Optional demo | Task slide / work and help |
|---|---|---|---|---|
| Account setup | 5 min | 1 min | 1 min | 3 min |
| Create repository | 5 min | 1 min | 1 min | 3 min |
| Edit and commit | 10 min | 1 min | 2 min | 7 min |
| History and correction | 10 min | 1 min | 2 min | 7 min |
| Independent edit / catch-up | 10 min | 1 min | None | 9 min |
| Branch draft | 8 min | 1 min | 2 min | 5 min |
| Own-repository PR | 12 min | 1 min | 3 min | 8 min |
| Share links and pair | 5 min | 1 min | 1 min | 3 min |
| Fork and edit | 8 min | 1 min | 2 min | 5 min |
| Send fork PR | 5 min | 1 min | 1 min | 3 min |
| Incoming review and merge | 7 min | 1 min | 1 min | 5 min |

The three fork activities still total 20 minutes. Protect the incoming review stage even if some outgoing PRs need help. The welcome, break, and closing remain 15, 10, and 10 minutes respectively.

## Session notes

### Welcome, Git vs. GitHub, and safe practice - 15 minutes

**Purpose:** Explain why the tools exist, establish safe content choices, and show the destination without a terminology lecture.

**Format and script:** Allow one quiet minute on "What file would you like to update more confidently?" Invite a few answers, with an option to pass. Spend about two minutes on:

> Git is the tool that tracks versions of a project. In 2005, Linus Torvalds started Git after the Linux project lost free access to its previous version-control tool, BitKeeper. The project needed a fast way for many contributors to work together.
>
> GitHub launched in 2008. It hosts Git repositories online and adds discussion, review, and coordination tools. Git tracks changes; GitHub helps people share and collaborate on them. You can use Git without GitHub or an internet connection. Today, GitHub's browser interface will create Git commits for us; no installation or commands required.

Use the two-box visual and timeline. Preview "we'll propose and accept each other's changes" but defer branch, PR, and fork mechanics until needed.

**Safety script:** "Before uploading, ask: would it be harmful if this became public? If yes, stop and check our organization's rules and get guidance, even for private or internal repositories. Restricted access reduces exposure; it does not prevent every mistake, compromised account, or copy. Today: fictional content only. No personal information, internal documents, passwords, or access keys."

**Visual demo:** Use the upload/history/downloaded-copy diagram. Remove the original from the illustration while keeping the other copies visible. Ask "Does deleting my copy delete everyone else's?" Say: "Once information spreads, complete removal may be impossible. If sensitive data is uploaded accidentally, stop and report it through the organization's incident process. Deleting the file alone is not a fix."

**Materials:** Goal, Git/GitHub, timeline, and safety slides; help signal and parking lot.

**Accessibility:** Read diagrams aloud, accept written questions, and agree a private help route. Avoid a compulsory round-robin.

**Likely pitfall:** Explaining every feature upfront. Name only what is needed; participants can use the later glossary as reference, not a memory test.

### Account setup - 5 minutes

**Purpose:** Reach a signed-in account and repository navigation.

**Format and script:** Explain the account task, let participants start, and offer the short demo to anyone who wants it. Show the signup entry point and describe private verification steps without projecting a verification message. Return to the task slide for three minutes of work/help. [Exercise 01](exercises/01-setup/) is an optional reference.

**Visual demo:** Open GitHub, show **Sign up**, then switch to an already signed-in demo account and locate **Your repositories → New**. Ask participants to find the same destination.

**Materials:** Browser and Exercise 01.

**Accessibility:** Keep steps available in text and help with navigation without taking credentials or control.

**Likely pitfall:** Treating five minutes as a guarantee. Route verification delays to helpers and the later catch-up buffer. Observation with a partner's consent is an interim alternative, not independent completion.

### Create a repository - 5 minutes

**Purpose:** Understand repository, README, and visibility through a real example.

**Format and script:** "A repository holds this project's files and history. The README introduces it." Explain the complete task before the optional demo. Let independent participants start, then leave the slide up for three minutes of work/help. Exercise 02, Part 1 is an optional reference.

**Visual demo:** Open **New repository**, create `cafe-handbook` with a README, and point to owner/name in the URL and the visibility label. Ask "Who can read this?" Public fictional repositories support the later fork exercise; no one must publish their own repository to participate.

**Materials:** Repository form, visibility slide, Exercise 02.

**Accessibility:** Read relevant labels aloud and keep the task visible.

**Likely pitfall:** Implying private or internal means safe for sensitive data. Repeat the suitability check; changing visibility does not undo copies already made.

### Edit/add a file and commit - 10 minutes

**Purpose:** Connect an edit, its commit message, and the saved result.

**Format and script:** "Typing is not a commit. A commit records a snapshot with a note." Point to the exact README text and commit message on the slide before the optional demo. Participants can start immediately. Return to that slide for seven minutes of work/help; Exercise 02, Part 2 is an optional reference.

**Visual demo:** Show editor → Preview → commit dialog → saved README and message. Keep the deliberate `Welcom` typo. Ask "Have we recorded a commit just by typing?" Briefly point out **Add file → Create new file** using a fictional `menu.md`; participants can try it during the buffer.

**Materials:** Cafe README example, editor, commit dialog.

**Accessibility:** Pause between editing and committing. Keep instructions available rather than hidden behind fragments.

**Likely pitfall:** Teaching direct commits to `main` as a workplace rule. They are only a simplification for participants' own disposable practice repositories; review rules may apply elsewhere.

### History and recovery - 10 minutes

**Purpose:** Introduce history and diff using a change participants already recognize.

**Format and script:** "History is our sequence of recorded versions; a diff shows what changed." Explain the visible correction task, including returning to current main, before the optional demo. Leave it projected for seven minutes afterward. Exercise 02, Part 3 is an optional reference.

**Visual demo:** Open the handbook commit and point to `Welcom`. Return to current **Code → main**, fix it, commit, and show the removed and added lines side by side or in the unified diff. Ask "Did correcting it erase the earlier commit?" Reopen the earlier version to show that it remains. Connect this directly to the sensitive-data rule; never demonstrate with a real secret.

**Materials:** Commit history, before/after versions, diff.

**Accessibility:** Read the changed text and `+`/`-` symbols aloud.

**Likely pitfall:** Editing an old snapshot. Explicitly return to current `main` before correcting.

### Independent edit and catch-up - 10 minutes

**Purpose:** Check the edit/commit/diff workflow and absorb account or navigation delays.

**Format and script:** Explain the opening-hours task and text on the slide for one minute, then leave it visible for nine minutes without a demo. "Try individually first; help is available." Exercise 02, Part 4 is an optional reference.

**Visual checkpoint:** Participants identify the new section, their commit message, and added lines. Early finishers can add `menu.md` or predict the diff from changing one opening time.

**Materials:** Task card, exercise, cheat sheet; helpers support those catching up.

**Accessibility:** No public speed comparisons or leaderboard. Offer a smaller edit and another independent attempt if needed.

**Likely pitfall:** An experienced partner taking over. Each participant uses their own keyboard; observation is recorded honestly as observation.

### Break - 10 minutes

**Purpose:** Rest and reset attention.

**Format and script:** Announce the return time. "Please take the break; catch-up is not required."

**Materials:** Break slide.

**Accessibility:** Permit quiet rest, remaining seated, or leaving the screen.

**Likely pitfall:** Turning the break into mandatory troubleshooting.

### Branch and PR in own repository - 20 minutes

**Purpose:** Understand a separate draft before introducing the proposal to merge it.

**Format and script:** Explain the branch task before its optional demo, then leave its instructions and menu text visible for five minutes. Check branch isolation before introducing the PR task. Explain that task before its optional demo, then leave it visible for eight minutes. The stages total 8 and 12 minutes respectively; do not present them as one uninterrupted explanation. Exercises 03 and 04 are optional detailed references.

**Visual demo, branch:** Create `add-menu`, add the small menu section, and commit. Ask "Will this be on main?" Switch draft → main → draft to verify. Only then introduce the PR.

**Visual demo, PR:** Match **FROM add-menu → INTO main** to **compare/base** in GitHub. Open the PR, inspect **Files changed**, and check current `main` in another tab. Ask "Did opening the PR change main?" Merge, then show that `main` now includes the menu. A success banner alone is not the final proof.

**Materials:** Branch diagram, PR direction diagram, browser selectors, Exercises 03 and 04.

**Accessibility:** Keep owner and branch labels readable and repeat source/destination in words. Allow time between branch and PR checkpoints.

**Likely pitfall:** Implying PRs automatically enforce approval or asking people to approve their own PR. This first PR is self-inspected; another person reviews in Exercise 05.

### Slack link exchange and pairing - 5 minutes

**Purpose:** Give everyone one outgoing target and one incoming contributor.

**Format and script:** Confirm the channel and audience aloud. "Post only your fictional practice repository URL. A restricted Slack channel does not make a public repository private." Explain the task before the optional example, then leave the slide up for three minutes while assigning pairs or a contribution ring; do not use free choice. Exercise 05, Part 1 is an optional reference.

**Visual demo:** Show the agreed message format and a pairing diagram, not real participant data in reusable screenshots.

**Materials:** Confirmed Slack channel, accessible pairing list, prepared public demo alternative.

**Accessibility:** Participants unable or unwilling to post can receive their assignment privately through an agreed route. Do not change their repository visibility or post on their behalf.

**Likely pitfall:** Everyone picking the same target or assuming private links grant access. Check both contributor and recipient for each assignment before continuing.

### Fork, contribute, review, and merge - 20 minutes

**Purpose:** Repeat the PR workflow across repositories, then experience the maintainer role.

**Format and script:** "A fork is your separate repository copy. A commit there does not change the original. A PR asks the original owner to accept the change." Use three self-contained activity slides: **fork/edit, 8 minutes; send PR, 5 minutes; incoming review/merge, 7 minutes**. Each starts with a brief explanation and optional demo while others can start; leave its instructions up for the work/help period in the timing table. Exercise 05, Part 2 is an optional detailed reference.

**Visual demos:** For fork/edit, show original and fork URLs side by side. Use an available fork name because participants already own `cafe-handbook`. Create `add-menu-item`, add `- Hot chocolate` under Sample Menu, and commit. Check that the original is unchanged, then leave the fork/edit slide visible for five minutes. Next explain sending the PR, point to all four source/destination selectors, and show opening it; leave that task slide visible for three minutes. Finally explain incoming review, show reading the diff, commenting, merging, and reopening original `main`; leave the review/merge slide visible for five minutes. Use prepared states or a consenting co-facilitator for these short demos rather than replaying earlier steps.

**Materials:** Two-repository diagram, labeled tabs/windows, base/head selector screenshot backup, Exercise 05.

**Accessibility:** Describe ownership changes aloud. Keep edits to one line, not a typing challenge. Confirm pending reviews are submitted, not left invisible.

**Likely pitfall:** A PR into the contributor's own fork, or stopping at PR creation. Everyone must return to their original repository to review the incoming change. Do not add conflicts, fork syncing, or merge strategies to this block.

### Completion, parked questions, and reflection - 10 minutes

**Purpose:** Check the full outcome and agree a realistic next step.

**Format and script:** Invite participants to show or describe a diff, their own PR, outgoing fork PR, and incoming merge. Return to the parking lot. Give quiet reflection time: "What can I do independently? What needs practice?"

**Visual checkpoint:** Confirm the incoming item appears on original `main` and its PR is **Merged**. Each participant chooses one fictional edit or PR and a date within seven days; success is a diff they can explain and, for a PR, a verified merge.

**Materials:** Completion checklist and parking lot.

**Accessibility:** Permit private or written reflection. Do not require public confidence scores, account details, or screenshots.

**Likely pitfall:** Announcing mastery for observed or assisted steps. Record unfinished work honestly and agree how the participant can retry.

## Collaboration surface and Slack instructions

Use the confirmed Slack channel for link exchange and PR threads, not sensitive content. Keep task instructions and parking-lot notes in an accessible text surface or displayed document; confirm access and retention before collecting input.

| Area | Structure and instructions |
|---|---|
| Current task | Exact steps and practice text / total time / optional demo / work-and-help period / done when; optional reference link separately |
| Repository exchange | One fictional practice repository URL per participant who agrees to post; incoming PR link in its thread |
| Assignments | Contributor → target owner/repository; everyone has one outgoing and one incoming contribution |
| Help | Agreed signal plus a private alternative; no speed ranking |
| Parking lot | Question / answer or resource / owner and date for any follow-up |
| Reflection | "I can now..." / "I need practice with..." / "My next task and date"; private by default |

No voting is needed. The facilitator owns timeboxing and assignments. Posting in the channel shares links with its audience; it is not automatically anonymous or confidential. Public repository content remains public regardless of channel access.

Do not export account lists, PR activity, screenshots, or raw individual reflections by default. Retain only agreed non-sensitive questions, answers, and follow-up actions with an owner and date. Do not create a channel, contact participants, or publish results without explicit authorization.

## If something goes wrong

- **Behind schedule:** Use the catch-up buffer, shorten explanations, and park optional questions. Protect the break, incoming review/merge verification, and closing reflection. State what remains unfinished.
- **Network failure:** Use sanitized screenshots and diagrams, but distinguish demonstration from hands-on completion and arrange a later attempt through an authorized route.
- **Access constraints:** Use an agreed public demo target and maintainer rather than promising private forking will work. Do not pressure anyone to publish their own repository.
- **Sensitive information uploaded:** Stop and follow the organization's incident process. Deleting the current file alone does not establish that the information is gone.

## Sources and slide setup

The short history is based on [Git's official history](https://git-scm.com/book/en/v2/Getting-Started-A-Short-History-of-Git) and [GitHub's April 10, 2008 launch announcement](https://github.blog/news-insights/the-library/we-launched/).

See [slide setup](slides/README.md) for deployment, speaker notes, visual demo conventions, and rehearsal.

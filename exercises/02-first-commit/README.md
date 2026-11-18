# Exercise 02 - Your First Repository and Commits

**Time:** 35 minutes, including demos and a catch-up buffer, before the break

**Task:** Build a handbook for a fictional community cafe, save changes with commits, and explain what changed.

Use invented content only. Do not add personal contact details, workplace documents, credentials, or other sensitive information, even in a private repository.

**Before uploading:** Would it be harmful if this became public? If yes, stop and check organizational rules and get guidance, even for a private or internal repository. Visibility settings cannot prevent every mistake, account compromise, or copy.

## Part 1: Create your repository (5 minutes)

### Task

Create `cafe-handbook` with a README.

### Steps

1. Choose **+ → New repository** or **New** from your repositories page.
2. Name it `cafe-handbook`.
3. Add a description: "A fictional cafe handbook for learning GitHub."
4. Choose visibility:
   - **Public:** Anyone can read the content and its history. This is the standard path for the later fork exercise, if you're comfortable publishing fictional practice content.
   - **Private:** Others need permission. A URL alone does not grant access, and private does not guarantee secrecy. Ask the facilitator about the later contribution alternative; you do not have to change visibility.
5. Select **Add a README file**, then **Create repository**.
6. Open `README.md`. A README is the project's introduction; `.md` means Markdown, a text-formatting syntax.

### Done when

You can find your repository, explain its visibility, and open the README.

**Demo checkpoint:** Locate the owner/name in the URL and the visibility label on the repository page.

## Part 2: Edit/add a file and commit (10 minutes)

### Task

Replace the README with a short cafe handbook and make a commit.

### Steps

1. Open `README.md` and choose the pencil icon or **Edit file**.
2. Replace its content with this fictional example. Keep the intentional `Welcom` typo; we'll correct it later.

```markdown
# Community Cafe Handbook

Welcom to our fictional community cafe!

## What We Serve
- Coffee
- Tea
- Cake

## Volunteer Checklist
- [ ] Set out the cups
- [ ] Check the menu board
- [ ] Welcome visitors
```

3. Use **Preview** to see how Markdown formats the headings and lists.
4. Choose **Commit changes** to open the commit dialog.
5. Write the message `Add cafe welcome and volunteer checklist`.
6. Choose to commit directly to `main`, then confirm **Commit changes**.
7. Check that the README shows the saved content.

A **commit** records a snapshot with a message. Typing in the editor alone does not create one. Direct commits to `main` are a simplification for your own practice repository, not a rule for workplace projects.

### Done when

The README contains the handbook and you can find your commit message.

**Visual demo:** Watch the editor → commit dialog → saved README. Predict whether typing alone creates a recorded version, then check the commit message after saving. The facilitator also briefly shows **Add file → Create new file** using a fictional `menu.md`; you can try adding a file during the buffer if ready.

## Part 3: History and recovery (10 minutes)

### Task

Inspect your first edit, then fix its typo with another commit.

### Steps

1. Return to the repository's **Code** page and open its commit history.
2. Select `Add cafe welcome and volunteer checklist`.
3. Read the **diff**, the comparison showing what changed:
   - `+` marks an added line, usually with a green background.
   - `-` marks a removed line, usually with a red background.
4. Find the line containing `Welcom`.
5. Return to **Code** and check that you're viewing `main`, not browsing an old commit.
6. Edit the current README: change `Welcom` to `Welcome`.
7. Commit the correction with `Fix spelling in cafe welcome`.
8. Open that commit in history. Identify the removed line and its replacement.

The earlier commit remains in history. The facilitator shows both versions and asks: did correcting the file erase the old version?

**Deleting isn't erasing:** A deleted file can remain in history or downloaded copies. Once information has spread, complete removal may be impossible. If sensitive data is uploaded accidentally, stop and report it through your organization's incident process. Do not assume deleting it fixes the exposure; never use real secrets to demonstrate this.

### Done when

You can show both commits and explain how the correction appears in the diff.

## Part 4: Try it yourself (10 minutes)

### Task

Without a live demonstration:

1. Add an **Opening Hours** section with fictional hours.
2. Commit it with a message describing the change.
3. Find that commit in history.
4. Explain which lines were added and whether the commit removed anything.

Try individually before comparing with a partner. Reference material and help are available whenever needed; this is practice, not a speed test.

This is also the catch-up buffer for setup delays. If you finish early, try **Add file → Create new file**, create `menu.md` with a fictional menu item, and commit it.

### Done when

You can point to the section, its commit message, and its diff.

### Optional challenge

Change one opening time in a separate commit. Predict which line will be removed and which will be added, then check your prediction in history.

**Break:** Take the scheduled 10-minute break after this part. Branches and PRs follow afterward.

## Done when

- [ ] I can find my repository and README and explain who can read them.
- [ ] I can edit a file and save it with a descriptive commit message.
- [ ] I can find a commit and explain its `+` and `-` lines.
- [ ] I can correct a mistake with a later commit.
- [ ] I have tried an edit without a live demonstration.

If you needed help, try one more small edit on your own. That is more useful than rushing into a new topic.

## Compare and reflect

Optionally explain your diff to a partner or facilitator. For a private repository, either show just the exercise file on your screen or invite your partner and have them accept before sharing the URL. You do not need to make it public or post your username.

Consider privately:

- What can I now do without help?
- What still needs practice?
- What question should we return to before closing?

## Next

After the break, continue to [Exercise 03: Branches](../03-branches/), then [Exercise 04: Pull Requests](../04-pull-requests/). Together they form the next 20-minute block.

## Quick help

- **My edit disappeared:** Confirm the repository and branch, then check whether you committed it.
- **I'm looking at an old version:** Return to **Code** and choose `main` before editing.
- **I can't find the button:** The UI may have changed; ask for help or consult [GitHub Docs](https://docs.github.com/).
- **I need a reminder:** Use the [cheat sheet](../../CHEAT-SHEET.md).

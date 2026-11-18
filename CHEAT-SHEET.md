# GitHub Quick Reference

**Workshop:** GitHub from Scratch

Use the browser for the core workshop. No Git commands or installations required.

## Core concepts

| Term | Meaning |
|---|---|
| Git | The version-control tool; usable without GitHub or an internet connection |
| GitHub | Online hosting and collaboration around Git repositories; today's browser interface creates Git commits |
| Repository (repo) | Project files and their committed history |
| README.md | The project's introduction, written in Markdown |
| Commit | A saved snapshot with a message describing the change |
| History | The sequence of commits you can inspect |
| Diff | A comparison showing added (`+`) and removed (`-`) lines |

## Before uploading

**Would it be harmful if this became public?** If yes, stop and check your organization's rules and get guidance before using GitHub, including private or internal repositories. Access restrictions are not a guarantee against mistakes, account compromise, or copies.

Use fictional content only in this workshop. No personal information, workplace documents, passwords, or access keys. A restricted Slack channel does not make linked public content private.

Deleting a file does not necessarily remove history or downloaded copies. Complete removal after information spreads may be impossible. If sensitive data is uploaded accidentally, stop and report it through the organization's incident process; deleting alone is not a fix.

## Create a repository

1. Choose **+ → New repository** or **New** on your repositories page.
2. Name it `cafe-handbook`.
3. Choose **Public** for the standard fictional fork exercise if comfortable, or agree the alternative with the facilitator.
4. Select **Add a README file**.
5. Choose **Create repository**.

Public content and its history can be read by anyone. A private repository needs invitations for others to access it; a URL alone is not enough. Use fictional content in either case.

## Edit and commit

1. Open the file and choose the pencil icon or **Edit file**.
2. Make your edit and use **Preview** if helpful.
3. Choose **Commit changes** to open the dialog.
4. Write a descriptive message, such as `Add cafe opening hours`.
5. In your own practice repository, choose to commit directly to `main`.
6. Confirm **Commit changes** and check the saved file.

Typing alone does not create a commit. Follow your team's branch and review rules outside this practice repository.

## Find a change

1. Return to the repository's **Code** page.
2. Open commit history and choose your commit message.
3. Read the diff: `+` is added text and `-` is removed text.

Additions are usually green and removals red, but the symbols also identify them.

## Correct a text mistake

1. Inspect history to understand the mistake.
2. Return to **Code** and check you're viewing `main`, not an old commit.
3. Edit the current file.
4. Make a new commit, such as `Fix spelling in cafe welcome`.
5. Inspect the new diff. The earlier commit remains in history.

This is for ordinary text corrections, not removing exposed credentials. Never use real secrets as practice content.

## Markdown basics

````markdown
# Main heading
## Section heading

**Bold text** and *italic text*

- List item
- Another item

1. First step
2. Second step

- [ ] Task to do
- [x] Completed task

[Link text](https://docs.github.com/)

```text
A block of plain text
```
````

## Quick troubleshooting

| Problem | Check |
|---|---|
| My edit isn't visible | Did you confirm the commit? Are you in the right repository and branch? |
| I'm looking at an old version | Return to Code and select `main` before editing. |
| My partner can't open my private repository | Invite them and wait for acceptance, or optionally show just the exercise file on screen. |
| A button has moved | Ask for help or consult [GitHub Docs](https://docs.github.com/). |
| Email isn't verified | Check spam and GitHub's resend option. Keep verification messages private. |

## Branches and collaboration

Learn these after working with files and commits; they are the second half of the workshop.

| Term | Meaning |
|---|---|
| Branch | A separate line of work, such as a draft handbook update |
| Pull request (PR) | A proposal to merge changes, with space for review and discussion |
| Merge | Combine changes into another branch |
| Issue | A task, question, or improvement to discuss |
| Fork | Your copy of someone else's repository, connected to the original |

**Branch workflow:** Create branch → edit and commit → open PR → review → merge → delete branch.

Check which branch you're on before editing. A branch alone does not enforce review or protect `main`; follow the repository's rules.

### PR in your own repository

1. From `main`, create `add-menu` with the branch dropdown.
2. Edit the README and commit to `add-menu`.
3. Switch to `main`: verify the draft edit is absent.
4. Choose **Pull requests → New pull request**: **base main**, **compare add-menu**.
5. Inspect the diff, add a title and explanation, and create the PR.
6. Opening a PR only proposes a change. Inspect **Files changed**, then merge and confirm.
7. Check `main` for the update; delete the draft branch if offered.

### Fork PR to a partner

1. Post the agreed fictional practice repository URL in the confirmed Slack channel; use your assigned target, not a random repository.
2. Open the target and choose **Fork**. Use an available name such as `cafe-handbook-contribution` because you already own `cafe-handbook`.
3. In your fork, create `add-menu-item`, add one fictional menu item, and commit.
4. Verify the original repository is still unchanged.
5. Use **Contribute → Open pull request**, or compare across forks.
6. Check destination (**base repository: partner's original**, **base: main**) and source (**head repository: your fork**, **compare: add-menu-item**).
7. Inspect the diff, create the PR, and send its link to the recipient through the agreed route.
8. Back in your original repository, read and comment on the incoming PR, submit any pending review, and merge if appropriate.
9. Both people verify the contributed item on the destination's `main`.

A fork is a separate repository, not a branch. It does not automatically stay synchronized with later changes to the original. For non-public/non-posting alternatives, see [Exercise 05: Access and sharing](exercises/05-collaboration/#access-and-sharing).

Follow [Branches](exercises/03-branches/), [Pull requests](exercises/04-pull-requests/), and [Collaboration](exercises/05-collaboration/) in order. Issues are optional follow-up practice.

## After the workshop

Choose one more handbook edit or PR and a date within seven days. Success is a diff you can explain and, for a PR, a verified merge.

- [Files and commits checklist](exercises/02-first-commit/)
- [Collaboration completion checklist](exercises/05-collaboration/#done-when)
- [GitHub Docs](https://docs.github.com/)
- [GitHub Skills](https://skills.github.com/)
- [Further learning](resources/)
- [Workshop issues](https://github.com/navikt/github-workshop/issues) for problems in these materials

# Exercise 04 - Your First Pull Request

**Time:** 12 minutes including demo, after Exercise 03 (8 minutes)

**Task:** Propose the cafe menu change from `add-menu`, inspect it, and merge it into `main`.

## See it first

A **pull request (PR)** proposes bringing changes from one branch into another. A **merge** accepts those changes into the destination.

```text
FROM: your-repository / add-menu
               |
         PR: inspect and discuss
               |
INTO: your-repository / main
```

The facilitator matches this diagram to GitHub's selectors: **compare** is where the changes come from; **base** is where they will go.

Predict: **does opening the PR change main, or only propose a change?**

## Steps

1. In your repository, choose **Pull requests → New pull request**.
2. Check **base: main** and **compare: add-menu**.
3. Inspect the diff. Confirm it includes only the intended sample menu.
4. Choose **Create pull request**, use the title `Add sample cafe menu`, and explain why:

```markdown
Adds a fictional menu so cafe volunteers can see what we serve.
```

5. Create the PR. Before merging, open **Code** in another tab and check `main`: the proposed menu is still absent.
6. Return to the PR and open **Files changed**. Read the additions using `+` as well as color.
7. Return to **Conversation**, choose **Merge pull request**, and confirm. Use the default merge option; if merging is blocked, ask the facilitator.
8. Delete the `add-menu` branch using the post-merge button if offered.
9. Return to **Code → main** and verify that the menu is now present.

For this first pass you inspect your own PR; you cannot approve your own PR. The next exercise adds a different person as reviewer and maintainer.

## Done when

- [ ] I can identify the source and destination of my PR.
- [ ] I can explain why opening a PR did not change `main`.
- [ ] The PR is marked **Merged**, and the menu is now on `main`.

## Visual checkpoint

Look at the same `main` README before and after the merge. The visible change should match the PR's diff, not just a success banner.

Next, [Exercise 05](../05-collaboration/) repeats the workflow across two repositories using a fork.

## Optional follow-up

Try a second small PR with a partner's comment before merging. Leave draft PRs, conflicts, and merge strategies for another session.

# Exercise 05 - Contribute to Someone Else's Repository

**Time:** 5 minutes to share and pair, then 20 minutes for the demo and contributions

**Task:** Send one tiny handbook improvement through a fork, then review and merge the contribution sent to your own repository.

Everyone acts as both **contributor** (proposes a change) and **maintainer** (decides what enters their repository).

## Access and sharing

The standard exercise uses public, disposable repositories with fictional content only. You do not need write access to your partner's public repository to propose a fork PR.

**Private is not a promise of secrecy.** If disclosure would be harmful, stop and check organizational rules and get guidance before uploading, including to private or internal repositories. A restricted Slack channel does not make a linked public repository private. Deleting content may not remove history, forks, or downloaded copies.

If you prefer not to publish your own repository or cannot post a URL in Slack, tell the facilitator. Use an agreed public demo repository with fictional content as your contribution target and optionally review the return contribution alongside its owner. Do not post or change the visibility of an existing private repository. Private repository forking depends on permissions and policy, so an invitation alone is not a guaranteed substitute for this exercise. If you observe instead of executing a step yourself, note that honestly.

## Part 1: Share and pair (5 minutes)

1. Check that your practice repository contains only fictional content, including its history.
2. If participating in the public path, post **only the practice repository URL** in the Slack channel named by the facilitator. No sensitive screenshots or real documents.
3. The facilitator assigns pairs, or a contribution ring for an odd-sized group:

```text
Pair: A contributes to B; B contributes to A
Ring: A contributes to B; B to C; C to A
```

4. Identify both your contribution target and who will contribute to you. Do not choose random repositories: everyone should receive exactly one contribution.

Do not post until the facilitator has confirmed the channel and audience. No channel name is assumed by these materials.

## See it first: why a fork?

You cannot directly edit someone else's repository without permission. A **fork** is a separate repository under your account, connected to the original, from which you can propose a change.

```text
PARTNER / cafe-handbook / main
            |
            | fork: create your own repository copy
            v
YOU / fork-name / add-menu-item
            |
            | commit, then propose a PR back to PARTNER / main
            v
PARTNER reads diff, comments, and merges
```

Because you already own `cafe-handbook`, your fork of your partner's repository needs another available name, such as `cafe-handbook-contribution`. Always check the **owner and repository name**, not just the file name.

The facilitator shows the two URLs side by side. Predict: **does committing in your fork change the original?**

## Part 2: Fork, contribute, review, and merge (20 minutes)

### Contributor: make and send the proposal

1. Open your assigned target, confirm its owner, and choose **Fork**.
2. Choose your account as the fork owner and an available name such as `cafe-handbook-contribution`. Create the fork.
3. Confirm that the URL now belongs to **you**, and GitHub identifies the original repository.
4. From your fork's `main`, create a branch called `add-menu-item`.
5. Edit the README: add **one fictional menu item**, such as `- Hot chocolate`. Commit to `add-menu-item`.
6. Open the partner's original `main` in another tab. Confirm your new item is not there.
7. In your fork, use **Contribute → Open pull request**, or **Pull requests → New pull request** and **compare across forks** if needed.
8. Check all four selectors before creating the PR:

| Selector | Must point to |
|---|---|
| Base repository | Your assigned partner's original repository |
| Base branch | `main` |
| Head repository | Your fork, under your account |
| Compare branch | `add-menu-item` |

9. Check that the diff contains only your intended menu item. If the destination or diff is wrong, stop and ask for help.
10. Create the PR with a descriptive title and one sentence explaining the change. Reply in your target's Slack thread with the PR link, or tell them through the agreed alternative.

### Maintainer: review the incoming contribution

1. Return to **your original repository**, not your fork of someone else's.
2. Open the incoming PR and check the description and **Files changed**.
3. Leave a useful comment, such as "This adds the drink under Sample Menu, which is the intended section." Confirm that any pending review is submitted so the contributor can see it.
4. If the change is appropriate, merge and confirm. If something is wrong, ask for a correction rather than merging blindly.
5. Check the original repository's `main` README for the new item.

### Both: verify the result

Open the original destination repository, select `main`, and locate the contributed item. Confirm the PR is marked **Merged**. The contributor's fork does not automatically stay synchronized with later changes; syncing is outside today's scope.

## Done when

- [ ] I can distinguish my original repository, my fork, and the repository I contributed to.
- [ ] My outgoing PR targets the assigned original repository, not my own fork.
- [ ] I have read and commented on the incoming diff.
- [ ] I have merged the appropriate incoming contribution.
- [ ] We can see the contributions on the destination repositories' `main` branches.

Use a one-line change to protect review time. Conflict resolution, syncing forks, and merge strategies are follow-up topics.

## Completion and next step

During the final ten minutes, show or describe your commit diff, own-repository PR, outgoing fork PR, and incoming merge. Return to parked questions.

Privately reflect: what can I do independently, and what needs practice? Choose one further fictional handbook edit or PR and a date within seven days. You own the task; success is a diff you can explain and, for a PR, a verified merge. Sharing that commitment is optional.

If sensitive information is uploaded accidentally, stop and report it through your organization's incident process. Do not assume deleting the file removes the exposure.

## Optional issue practice

An **issue** tracks a task or question without changing files. Create one follow-up suggestion in the agreed practice repository, explain the desired improvement, and respond to a partner's suggestion. Use fictional content and arrange access first; private URLs alone do not grant permission.

Continue to [Exercise 06](../06-practical-applications/) for optional documentation, Projects, and Pages ideas.

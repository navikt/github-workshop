# Exercise 03 - A Branch Is a Separate Draft

**Time:** 8 minutes including demo, followed immediately by Exercise 04 (12 minutes)

**Task:** Add a sample menu on a draft branch of your fictional `cafe-handbook`, without changing `main`.

## See it first

You want to propose a handbook update without changing the current version yet. A **branch** gives that draft a name.

```text
main:      current handbook ---------------- still unchanged
                         \
add-menu:                 draft + menu commit
```

The facilitator creates a draft, makes one change, and switches between the branches. Before switching, predict: **will the menu appear on main?**

A branch separates work; it does not enforce review or prevent direct edits to `main`. Follow your team's rules outside this practice repository.

## Steps

1. Open your own `cafe-handbook` and select `main`.
2. Open the branch dropdown, type `add-menu`, and choose **Create branch**.
3. Check that the dropdown now says `add-menu`.
4. Edit `README.md` and add:

```markdown
## Sample Menu
- Filter coffee
- Herbal tea
- Lemon cake
```

5. Commit with `Add sample cafe menu`, directly to **add-menu**, not `main`.
6. Switch to `main` and inspect the README. The new section should be absent.
7. Switch back to `add-menu` and confirm the section is there.

## Done when

- [ ] I can identify my current branch.
- [ ] I can show that the menu is on `add-menu` but not on `main`.
- [ ] I can explain a branch as a separate draft.

Do not merge yet. Next, [Exercise 04](../04-pull-requests/) introduces a pull request as the proposal to bring this draft into `main`.

## If something differs

If the menu already appears on `main`, check the commit history and ask for help; you may have committed on the wrong branch. Do not delete work or start making unrelated branches to catch up.

Use the [cheat sheet](../../CHEAT-SHEET.md) for a reminder.

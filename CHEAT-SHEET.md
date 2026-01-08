# GitHub Quick Reference Cheat Sheet

**Workshop: GitHub for Dummies**

---

## Key Concepts

| Term | Definition | Analogy |
|------|------------|---------|
| **Repository (Repo)** | Project folder that tracks all changes | A project folder with superpowers |
| **Commit** | Snapshot of changes with a description | Saving with a note about what you did |
| **Branch** | Parallel version of your project | Parallel universe for safe experiments |
| **Main Branch** | Default/primary branch | The "official" version |
| **Pull Request (PR)** | Proposed changes for review | Submitting work for approval |
| **Merge** | Combining branches together | Accepting changes into main version |
| **Fork** | Your personal copy of someone's repo | Making your own copy of a cookbook |
| **Clone** | Downloading repo to your computer | Downloading files to work offline |
| **Issue** | Task, bug report, or discussion | Project to-do item or question |

---

## Common GitHub Actions

### Creating a Repository
1. Click **+** in top-right corner → **New repository**
2. Choose a name (no spaces, use hyphens)
3. Select Public or Private
4. ✅ Check "Add a README file"
5. Click **Create repository**

### Making Changes (Committing)
1. Navigate to the file you want to edit
2. Click the **pencil icon** (Edit)
3. Make your changes
4. Scroll down to "Commit changes"
5. Write a clear commit message
6. Click **Commit changes**

### Creating a Branch
1. Click branch dropdown (says "main")
2. Type new branch name
3. Click "Create branch: [name]"
4. You're now on the new branch!

### Switching Branches
1. Click branch dropdown
2. Select the branch name
3. Files update to that branch's version

### Creating a Pull Request
1. Make changes on a branch (not main)
2. Click **Pull requests** tab
3. Click **New pull request**
4. Select your branch to merge into main
5. Click **Create pull request**
6. Add title and description
7. Click **Create pull request**

### Merging a Pull Request
1. Open the pull request
2. Review the changes (Files changed tab)
3. Click **Merge pull request**
4. Click **Confirm merge**
5. Optional: Delete the branch (cleanup)

### Creating an Issue
1. Click **Issues** tab
2. Click **New issue**
3. Add title and description
4. Optional: Add labels, assignees
5. Click **Submit new issue**

---

## Markdown Basics

Use Markdown to format text in README files, issues, and comments:

```markdown
# Heading 1
## Heading 2
### Heading 3

**bold text**
*italic text*

- Bullet point
- Another point
  - Nested point

1. Numbered list
2. Second item

[Link text](https://url.com)

![Image alt text](image-url.jpg)

`code text`

```
code block
```
```

---

## Good Commit Message Examples

✅ **Good Messages:**
- "Add contact information to README"
- "Fix typo in introduction section"
- "Update team member list"
- "Remove outdated pricing information"

❌ **Bad Messages:**
- "changes"
- "update"
- "fixed stuff"
- "asdfasdf"

**Tip:** Describe WHAT you changed and WHY (if not obvious)

---

## Keyboard Shortcuts

| Action | Shortcut |
|--------|----------|
| Search repository | `/` or `Ctrl/Cmd + K` |
| Create new issue | `C` (on Issues page) |
| Submit comment | `Ctrl/Cmd + Enter` |
| Go to Code tab | `G` then `C` |
| Go to Issues tab | `G` then `I` |
| Go to Pull Requests | `G` then `P` |

---

## Collaboration Workflow

**Standard Flow:**
1. Create a branch for your work
2. Make changes and commit them
3. Open a pull request
4. Team reviews your changes
5. Make updates if requested
6. Pull request gets merged
7. Delete the branch

**Quick Tip:** Keep branches focused on one task/feature

---

## Common Scenarios

### "I want to propose a change to someone's project"
1. Fork their repository
2. Make changes in your fork
3. Create a pull request back to original repo

### "I want to track bugs and tasks"
- Use Issues tab
- Add labels (bug, enhancement, question)
- Assign to team members
- Reference issues in commits with `#issue-number`

### "I want to undo my last commit"
1. Go to commit history
2. Find previous commit
3. Click browse files at that commit
4. Make new commit with corrected version

### "I want to work with my team"
1. Create repository (or get added as collaborator)
2. Each person works on their own branch
3. Use pull requests to propose changes
4. Review each other's work
5. Merge when approved

---

## Important Things to Remember

### ✅ DO:
- Write clear commit messages
- Create branches for new work
- Use pull requests for review
- Ask questions in Issues
- Read the README first
- Check existing issues before creating new ones

### ❌ DON'T:
- Commit directly to main (use branches!)
- Write vague commit messages
- Work on someone's repo without permission
- Delete things without understanding impact
- Panic - you can usually undo changes!

---

## Helpful URLs

| Resource | URL |
|----------|-----|
| GitHub Skills | https://skills.github.com |
| GitHub Docs | https://docs.github.com |
| Markdown Guide | https://www.markdownguide.org |
| GitHub Status | https://www.githubstatus.com |
| Support | https://support.github.com |

---

## File Structure Best Practices

**Every repository should have:**
- `README.md` - Project description and instructions
- `LICENSE` - How others can use your code (optional)
- `.gitignore` - Files to ignore (for technical projects)

**Good folder structure:**
```
my-project/
├── README.md
├── docs/           (documentation)
├── src/            (source files)
├── tests/          (test files)
└── examples/       (example files)
```

---

## Troubleshooting

| Problem | Solution |
|---------|----------|
| Can't find my branch | Check branch dropdown - you might be on a different branch |
| Changes disappeared | Check which branch you're on |
| Email not verified | Check spam folder, resend verification |
| Merge conflict | Contact a team member or facilitator for help |
| Locked out of account | Use GitHub account recovery |
| Can't push changes | Check if you have write access to the repository |

---

## Next Steps After Workshop

**Practice Ideas:**
1. Create a personal portfolio repository
2. Document a hobby or project
3. Collaborate with a friend on a shared project
4. Contribute to an open source project
5. Use GitHub for meeting notes or documentation

**Continue Learning:**
- Complete GitHub Skills courses
- Watch GitHub Universe talks
- Join GitHub Community discussions
- Explore trending repositories
- Set up GitHub Pages (free website)

---

## Quick Command Reference (Web Interface)

**Everything you learned today can be done through the web interface - no command line required!**

However, if you're curious about Git commands for the future:

| Web Action | Git Command Equivalent |
|------------|----------------------|
| Commit changes | `git commit -m "message"` |
| Create branch | `git branch branch-name` |
| Switch branch | `git checkout branch-name` |
| Merge PR | `git merge branch-name` |
| Clone repo | `git clone repo-url` |

---

## Support & Questions

**Need Help?**
- Check [GitHub Docs](https://docs.github.com)
- Ask in [GitHub Community](https://github.community)
- Contact workshop facilitator: [contact info]
- Open an issue in workshop repository

---

**Remember: The best way to learn GitHub is to use it. Start a project today! 🚀**

*Keep this cheat sheet handy as you practice!*

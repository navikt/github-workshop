# Exercise 04 - Pull Requests: The Professional Way to Merge

**Time: 15 minutes**  
**Objective:** Learn to create, review, and merge pull requests

---

## What You'll Learn
- What pull requests are and why they're important
- How to create a pull request
- How to review changes
- How to merge changes into main
- Best practices for PRs

---

## Understanding Pull Requests

### What is a Pull Request?

A **Pull Request** (PR) is a proposal to merge changes from one branch into another.

Think of it as:
- 📝 "Hey team, I finished this work. Can you review it before we publish?"
- 🔍 A chance to review and discuss changes
- ✅ Quality control before code goes live
- 📚 Documentation of WHY changes were made

### Why Pull Requests Matter

**For Solo Projects:**
- Forces you to review your own work
- Creates a record of what changed and why
- Helps you think through your changes

**For Teams:**
- Code review catches bugs and improves quality
- Knowledge sharing - everyone learns from reviews
- Prevents accidental breaking changes
- Encourages discussion and collaboration

### The Pull Request Workflow

```
1. Create branch
2. Make changes and commit
3. Open Pull Request
4. Review and discuss
5. Make any requested changes
6. Merge to main
7. Delete branch (cleanup)
```

---

## Part 1: Create a Pull Request (5 minutes)

Let's create your first PR!

### Prerequisites:
- You should have a branch with changes (from Exercise 03)
- If not, create a branch and make some changes first

### Steps:

1. **Go to your repository's main page**

2. **Look for the Pull Requests tab** (near the top)

3. **Click "Pull requests"**

4. **Click the green "New pull request" button**

5. **Configure the pull request:**
   - **Base branch:** `main` (where changes will go)
   - **Compare branch:** Select your feature branch
   
6. **Review the comparison:**
   - GitHub shows you exactly what will change
   - Green = additions, Red = deletions

7. **Click "Create pull request"**

8. **Fill in the PR details:**

   **Title:** Clear and descriptive
   - ✅ "Add contact information and fun facts"
   - ✅ "Update README with personal details"
   - ❌ "Updates"
   - ❌ "PR"

   **Description:** Explain your changes
   ```markdown
   ## What Changed
   - Added contact information section
   - Added fun facts about myself
   - Improved formatting
   
   ## Why
   - To make the README more personal
   - To practice using branches and PRs
   
   ## Screenshots (if applicable)
   [Add screenshots of visual changes]
   ```

9. **Click "Create pull request"**

🎉 **You've created your first Pull Request!**

---

## Part 2: Review Your Pull Request (3 minutes)

Now let's explore what you just created.

### Tabs to Explore:

#### **Conversation Tab**
- Shows the description and discussion
- Comments and reviews appear here
- Status checks (if configured)

#### **Commits Tab**
- Lists all commits in this PR
- Shows the history of changes
- Useful for understanding the work progression

#### **Files Changed Tab** (Most Important!)
- Shows exactly what changed
- Line-by-line comparison
- This is where reviews happen

### Explore the Files Changed Tab:

1. **Click "Files changed"**

2. **Look at the diff:**
   - Green background = added lines (with `+`)
   - Red background = removed lines (with `-`)
   - White = unchanged (for context)

3. **Try hovering over a line:**
   - You can add comments to specific lines!
   - Click the `+` icon that appears

4. **Add a comment:**
   - Click the `+` icon on any changed line
   - Write something like: "Good addition!"
   - Click "Add single comment"

---

## Part 3: Merge Your Pull Request (4 minutes)

Once you're happy with the changes (and any reviews are complete), it's time to merge!

### Steps:

1. **Go back to the "Conversation" tab**

2. **Scroll to the bottom**

3. **Look for the merge section:**
   - Green checkmark = ready to merge
   - If you see "Conflicts", you'll need to resolve them (ask for help!)

4. **Click "Merge pull request"**
   - You'll see different merge options (stick with the default for now)

5. **Confirm the merge:**
   - Optionally, edit the merge commit message
   - Click "Confirm merge"

6. **Success! 🎉**
   - Your changes are now in the main branch
   - The PR shows as "Merged"

7. **Clean up:**
   - Click "Delete branch" (appears after merge)
   - This keeps your repository tidy
   - Don't worry - the branch history is preserved!

---

## Part 4: Verify the Merge (3 minutes)

Let's confirm everything worked correctly.

### Steps:

1. **Click on "Code" tab** (back to main repository view)

2. **Make sure you're on the "main" branch** (check branch dropdown)

3. **Look at your README.md file**
   - Your changes from the branch are now here!
   - The main branch has been updated

4. **Check the commit history:**
   - Click on the commit count
   - See the merge commit
   - Notice it references your PR (e.g., "Merge pull request #1")

---

## Advanced: Pull Request Best Practices

### Writing Good PR Descriptions

**Include:**
- ✅ What changed (be specific)
- ✅ Why the change was needed
- ✅ How to test the changes
- ✅ Screenshots (for visual changes)
- ✅ Related issues (e.g., "Fixes #123")

**Template:**
```markdown
## Summary
Brief description of what this PR does

## Changes
- Change 1
- Change 2
- Change 3

## Why
Explain the motivation for these changes

## Testing
How to verify these changes work

## Screenshots (if applicable)
[Add images here]

## Notes
Any additional context or concerns
```

### Reviewing PRs (For Teams)

**As a Reviewer:**
- 👀 Read the description first
- 🔍 Check the changes carefully
- 💬 Ask questions if unclear
- 👍 Approve when satisfied
- 🙏 Be constructive and kind

**Review Comments:**
- ✅ "Great solution! One suggestion..."
- ✅ "This works, but have you considered...?"
- ✅ "Nice job! Just one small typo on line 42"
- ❌ "This is wrong"
- ❌ "Why did you do it this way?"

### Small PRs vs Large PRs

**Good PR Size:**
- ✅ Focused on one feature/fix
- ✅ Reviewable in 15-30 minutes
- ✅ Clear purpose and scope

**Too Large:**
- ❌ Changes dozens of files
- ❌ Multiple unrelated features
- ❌ Takes hours to review

**Tip:** Break large work into multiple small PRs

---

## Practice Exercises

### Exercise 1: Full Workflow
1. Create a new branch: `add-projects-section`
2. Add a "Projects" section to your README
3. Commit the changes
4. Create a pull request
5. Review your own changes
6. Add a comment on one line
7. Merge the PR
8. Delete the branch

### Exercise 2: Multiple Changes
1. Create branch: `improve-formatting`
2. Make several commits with different improvements
3. Create a PR and notice it includes all commits
4. Add a detailed description
5. Merge when ready

### Exercise 3: Draft PR
1. Create a new branch
2. Make a small change
3. Create a PR, but select "Create draft pull request"
4. Draft PRs show as "Work in progress"
5. When ready, click "Ready for review"
6. Then merge normally

---

## Understanding Merge Conflicts

### What is a Merge Conflict?

Happens when:
- Two branches change the same line of the same file
- GitHub can't automatically determine which change to keep

**Example:**
```
Branch A changes line 5 to: "Hello World"
Branch B changes line 5 to: "Hi Universe"
```

GitHub says: "You decide which one to keep!"

### Resolving Conflicts (Simple Version)

1. GitHub will show "This branch has conflicts"
2. Click "Resolve conflicts"
3. Choose which changes to keep
4. Mark as resolved
5. Complete the merge

**Don't worry about this for now!** In this workshop, you probably won't create conflicts. But if you do, ask for help!

---

## Pull Request Etiquette

### As the PR Author:
- ✅ Write clear descriptions
- ✅ Keep PRs focused and small
- ✅ Respond to review comments
- ✅ Be open to feedback
- ✅ Test your changes before opening PR

### As a Reviewer:
- ✅ Review promptly
- ✅ Be constructive and specific
- ✅ Ask questions instead of making demands
- ✅ Acknowledge good work
- ✅ Approve when satisfied

---

## Common Questions

**Q: Can I add more commits after creating a PR?**  
A: Yes! Any new commits to the branch automatically appear in the PR.

**Q: Can I close a PR without merging?**  
A: Yes! Click "Close pull request". Useful if you decide not to proceed with changes.

**Q: What happens to the branch after merging?**  
A: It stays around until you delete it. Best practice: delete after merging.

**Q: Can I reopen a closed PR?**  
A: Yes! Click "Reopen pull request".

**Q: Do I need PRs for personal projects?**  
A: Not strictly necessary, but it's good practice and creates a nice history.

---

## Key Takeaways

✅ **Pull Requests** = Proposal to merge changes  
✅ **Reviews** = Quality control and learning opportunity  
✅ **Descriptions** = Document what and why  
✅ **Small PRs** = Easier to review and merge  
✅ **Clean up** = Delete branches after merging  

---

## GitHub Flow Summary

```
main branch (always deployable)
    ↓
Create feature branch
    ↓
Make changes (multiple commits OK)
    ↓
Open Pull Request
    ↓
Discuss and review
    ↓
Make additional changes if needed
    ↓
Merge to main
    ↓
Delete feature branch
    ↓
Repeat for next feature
```

---

## What's Next?

You now know the complete GitHub workflow! Next, we'll learn how to collaborate with others.

Move on to **Exercise 05 - Collaboration** to practice working with teammates!

---

**Need help?** Check the [Cheat Sheet](../../CHEAT-SHEET.md) or ask your facilitator!

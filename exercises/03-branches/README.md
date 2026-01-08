# Exercise 03 - Branches: Working Safely

**Time: 15 minutes**  
**Objective:** Learn to create and work with branches for safe experimentation

---

## What You'll Learn
- What branches are and why they're essential
- How to create a new branch
- How to switch between branches
- How branches keep your work organized
- When to use branches

---

## Understanding Branches

### What is a Branch?

Think of a **branch** as a parallel universe for your project:
- You can experiment freely without affecting the main version
- Multiple people can work on different features simultaneously
- If something goes wrong, your main version is safe

### Real-World Analogy

Imagine you're writing a book:
- **Main branch** = The published manuscript
- **Feature branch** = A draft where you try a new chapter
- You can work on the draft without changing the published version
- When you're happy with the new chapter, you merge it into the manuscript

### Why Branches Matter

✅ **Safety:** Experiment without breaking things  
✅ **Organization:** Each feature/task gets its own branch  
✅ **Collaboration:** Multiple people work simultaneously  
✅ **Review:** Changes can be reviewed before merging  

---

## Part 1: Your First Branch (5 minutes)

Let's create a branch and make some changes!

### Steps:

1. **Go to your repository** (the one you created in Exercise 02)

2. **Find the branch selector** 
   - Look for a button that says "main" with a dropdown arrow
   - It's usually near the top-left of the file list

3. **Click on the branch dropdown**

4. **Type a name for your new branch:**
   - Good names describe what you're working on:
     - `add-contact-info`
     - `update-about-section`
     - `fix-typo`
   - Use lowercase and hyphens

5. **Click "Create branch: [your-branch-name]"**

🎉 **You've created your first branch!**

**Notice:** The dropdown now shows your new branch name instead of "main"

---

## Part 2: Make Changes on Your Branch (5 minutes)

Now let's make some changes on your new branch. The main branch will stay exactly the same!

### Steps:

1. **Confirm you're on your new branch** (check the branch dropdown)

2. **Edit your README.md file** (click the pencil icon ✏️)

3. **Add a new section.** For example:

```markdown
## Contact Information
- Email: your.email@example.com
- GitHub: @yourusername
- Location: Your City, Country

## Fun Facts
- 🎸 I play guitar
- 🌏 I've visited 15 countries
- ☕ I drink 3 coffees per day
```

4. **Scroll down and commit your changes**
   - Commit message: "Add contact information and fun facts"
   - Make sure "Commit directly to the [branch-name] branch" is selected

5. **Click "Commit changes"**

✅ **Important:** These changes only exist on your branch!

---

## Part 3: The Magic of Branches (3 minutes)

Now let's see how branches keep things separate.

### Switch Between Branches:

1. **Click the branch dropdown** again

2. **Select "main"** from the list

3. **Look at your README.md file**

**🎩 Magic moment:** Your changes disappeared! They're safe on your branch, but the main branch is unchanged.

4. **Switch back to your feature branch**

5. **Look at README.md again**

**The changes are back!** This is the power of branches.

---

## Part 4: Understanding Branch Workflow (2 minutes)

### The Standard Workflow:

```
main branch (stable, production-ready)
    ↓
Create feature branch
    ↓
Make changes on feature branch
    ↓
Test and review changes
    ↓
Merge back to main
    ↓
Delete feature branch (cleanup)
```

### Branch Naming Conventions:

**Good branch names:**
- `feature/user-login` - new feature
- `fix/broken-link` - bug fix
- `docs/update-readme` - documentation
- `add-team-page` - descriptive

**Bad branch names:**
- `test` - too vague
- `my-branch` - not descriptive
- `branch1` - meaningless
- `stuff` - what stuff?

---

## Practice Exercises

### Exercise 1: Multiple Branches
1. Go back to the main branch
2. Create another new branch: `add-favorite-books`
3. Add a section about your favorite books
4. Commit the changes
5. Switch between main, your first branch, and this branch
6. Notice how each has different content!

### Exercise 2: Organized Changes
Create branches for different types of updates:
1. `fix/spelling-errors` - fix any typos
2. `feature/add-goals` - add a goals section
3. `update/improve-formatting` - improve markdown formatting

### Exercise 3: Before & After
1. Create a branch called `experiment`
2. Make dramatic changes to your README (change everything!)
3. Switch back to main
4. See how your main branch is completely safe

---

## Visualizing Branches

```
main:        A --- B --- C --- D
                   \           \
feature:            E --- F --- G (merge later)
```

- **A, B, C, D** = Commits on main branch
- **E, F, G** = Commits on feature branch
- Feature branch splits from B
- Can merge back to main later

---

## Key Concepts

### When to Create a Branch:
✅ Starting work on a new feature  
✅ Fixing a bug  
✅ Experimenting with changes  
✅ Working on something that needs review  

### When NOT to Create a Branch:
❌ Tiny typo fixes (can commit directly to main)  
❌ Emergency hotfixes (though some teams use branches for these too)  

### Branch Hygiene:
✅ One branch per feature/task  
✅ Use descriptive names  
✅ Keep branches short-lived  
✅ Delete branches after merging  
✅ Merge or delete old branches  

---

## Common Questions

**Q: How many branches can I have?**  
A: As many as you want! But keep them organized and delete old ones.

**Q: What if I forget which branch I'm on?**  
A: Check the branch dropdown. It always shows your current branch.

**Q: Can I move changes from one branch to another?**  
A: Yes, but that's an advanced topic. For now, make sure you're on the right branch before making changes!

**Q: What if I make changes on the wrong branch?**  
A: Don't panic! You can usually fix this. Ask your facilitator for help.

**Q: Do I always need to use branches?**  
A: For solo projects, not always. But it's a good habit! For team projects, branches are essential.

---

## Tips for Success

💡 **Always check which branch you're on before making changes**  
💡 **Use the branch dropdown frequently**  
💡 **Name branches clearly so you remember what they're for**  
💡 **Don't be afraid to experiment - that's what branches are for!**  
💡 **Think of main as your "published" version**  

---

## What's Next?

You've learned to create branches and work safely. But how do you get changes from your branch back into main?

That's where **Pull Requests** come in! Head to **Exercise 04 - Pull Requests** to learn the professional way to merge your work.

---

## Quick Reference

```markdown
# Branch Commands (Web Interface)

Create branch:
1. Click branch dropdown
2. Type new name
3. Click "Create branch"

Switch branch:
1. Click branch dropdown
2. Select branch name

Check current branch:
- Look at branch dropdown
```

---

**Need help?** Check the [Cheat Sheet](../../CHEAT-SHEET.md) or ask your facilitator!

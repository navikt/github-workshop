# Exercise 05 - Collaboration: Working with Others

**Time: 15 minutes**  
**Objective:** Learn to collaborate with others using GitHub's team features

---

## What You'll Learn
- How to work with collaborators
- What issues are and how to use them
- How to fork and contribute to other projects
- Using @mentions for communication
- Understanding notifications

---

## Understanding GitHub Collaboration

GitHub is built for teamwork! Whether you're working on:
- Open source projects with strangers
- Company projects with coworkers
- Personal projects with friends
- Documentation with non-technical teammates

GitHub provides tools to coordinate and communicate effectively.

---

## Part 1: GitHub Issues (5 minutes)

**Issues** are GitHub's built-in task management system. Think of them as:
- 📋 To-do items
- 🐛 Bug reports
- 💡 Feature requests
- ❓ Questions
- 💬 Discussion threads

### Create Your First Issue:

1. **Go to your repository**

2. **Click the "Issues" tab**

3. **Click "New issue"**

4. **Fill in the details:**

   **Title:** Clear and specific
   ```
   ✅ "Add a Projects section to README"
   ✅ "Fix broken link in About page"
   ✅ "Question: How to add images?"
   ❌ "Fix it"
   ❌ "Problem"
   ```

   **Description:** Use the template below
   ```markdown
   ## Description
   We need to add a Projects section to showcase completed work.
   
   ## Tasks
   - [ ] Create Projects section
   - [ ] Add 3 example projects
   - [ ] Include links and descriptions
   
   ## Additional Context
   This will help visitors understand what we've built.
   ```

5. **Assign the issue (optional):**
   - Assign to yourself or teammates
   - Helps track who's working on what

6. **Add labels (optional):**
   - `bug` - something is broken
   - `enhancement` - new feature request
   - `question` - need information
   - `documentation` - docs related
   - `good first issue` - good for beginners

7. **Click "Submit new issue"**

### Working with Issues:

**Add a Comment:**
- Scroll down and write an update
- Example: "Started working on this!"

**Reference in Commits:**
- In your commit message, type: `Addresses #1`
- GitHub automatically links the commit to the issue
- Use `Fixes #1` or `Closes #1` to auto-close when merged

**Close an Issue:**
- Click "Close issue" when work is complete
- Or close automatically with commit message keywords

---

## Part 2: Partner Exercise - Create Issues for Each Other (5 minutes)

**You'll need a partner for this exercise!**

### Find a Partner:

Pair up with someone in the workshop (or a friend if doing this remotely).

### Exchange Repository URLs:

1. Go to your repository
2. Copy the URL from your browser
3. Share it with your partner
4. Get your partner's repository URL

### Create an Issue in Your Partner's Repository:

1. **Visit your partner's repository URL**

2. **Click the "Issues" tab**

3. **Click "New issue"**

4. **Create a helpful issue for them:**

   **Example 1: Feature Request**
   ```markdown
   Title: Add a Skills section
   
   ## Suggestion
   Hey! I noticed your README could benefit from a Skills section.
   
   ## Ideas
   - List programming languages you know
   - Tools and technologies
   - Soft skills
   
   Looking forward to seeing this! 🚀
   ```

   **Example 2: Question**
   ```markdown
   Title: What's your favorite project?
   
   ## Question
   I'm curious - what's the most interesting project you've worked on?
   
   Would love to hear more about it!
   ```

   **Example 3: Collaboration Offer**
   ```markdown
   Title: Want to collaborate on something?
   
   ## Proposal
   I'm also learning GitHub! Want to create a shared project together?
   
   Maybe we could:
   - Create a resources list
   - Build a workshop notes repository
   - Practice pull request reviews
   
   Let me know what you think! @theirusername
   ```

5. **Use @mentions:**
   - Type `@` followed by their GitHub username
   - They'll get a notification!

### Respond to Your Issue:

1. **Check your own Issues tab** - you should have a new issue!
2. **Read what your partner wrote**
3. **Add a comment:**
   ```markdown
   Thanks for the suggestion @theirusername! 
   
   Great idea - I'll work on this soon. Would you like to review my PR when I'm done?
   ```

---

## Part 3: Understanding Collaboration Roles (2 minutes)

### Repository Access Levels:

**Owner:**
- Full control
- Can delete repository
- Manage collaborators
- Change settings

**Collaborator:**
- Can push directly to repository
- Create and merge PRs
- Manage issues
- Cannot delete repository

**Outside Contributor:**
- Can create issues
- Can comment on PRs/issues
- Must fork to propose changes
- Cannot push directly

### Adding Collaborators:

1. Go to your repository
2. Click "Settings" tab
3. Click "Collaborators" in sidebar
4. Click "Add people"
5. Search for GitHub username
6. Send invitation

**Note:** For this workshop, you don't need to add collaborators. Issues and comments work without special access!

---

## Part 4: Forking - Contributing to Projects You Don't Own (3 minutes)

**Forking** creates your personal copy of someone else's repository.

### When to Fork:

- Contributing to open source projects
- Creating your own version of a project
- Experimenting with someone else's code
- Proposing changes when you're not a collaborator

### Fork Workflow:

```
Original Repository
    ↓
Fork (create your copy)
    ↓
Make changes in your fork
    ↓
Create Pull Request back to original
    ↓
Original owner reviews and merges
```

### Try Forking:

1. **Visit a partner's repository** (or use the workshop repo)

2. **Click "Fork" button** (top-right)

3. **Click "Create fork"**

4. **You now have your own copy!**
   - Notice the URL is under YOUR username
   - Says "forked from [original-owner]/[repo-name]"

5. **Make changes in your fork:**
   - Edit a file
   - Commit changes
   - This doesn't affect the original!

6. **To contribute back:**
   - Click "Contribute" → "Open pull request"
   - This creates a PR from your fork to the original
   - The original owner can review and merge

---

## Collaboration Best Practices

### Communication

**DO:**
- ✅ Be clear and specific in issues
- ✅ Use @mentions to get someone's attention
- ✅ Be respectful and constructive
- ✅ Say thank you and acknowledge help
- ✅ Update issues with progress

**DON'T:**
- ❌ Spam with unnecessary comments
- ❌ Be rude or demanding
- ❌ Leave issues open after completion
- ❌ Create duplicate issues

### Issue Management

**Good Issue:**
```markdown
Title: Add dark mode toggle

## Problem
The site is hard to read in low-light conditions.

## Proposed Solution
Add a toggle button to switch between light and dark themes.

## Acceptance Criteria
- [ ] Toggle button in header
- [ ] Persists user preference
- [ ] Applies to all pages
```

**Bad Issue:**
```markdown
Title: Fix stuff

Make it better.
```

### Pull Request Reviews

**Giving Feedback:**
```markdown
Great work on this PR! A few thoughts:

✅ Love the new feature
🤔 Consider adding error handling on line 42
📝 Small typo in comment on line 67

Overall looks good! Approve with small changes suggested.
```

**Receiving Feedback:**
```markdown
Thanks for the review @reviewer!

- Fixed the typo ✅
- Added error handling ✅
- Also improved documentation based on your suggestion

Ready for another look!
```

---

## GitHub Notifications

### Managing Notifications:

**Click the bell icon** (top-right) to see:
- @mentions
- Issues assigned to you
- PR reviews requested
- Replies to your comments

**Configure Notifications:**
1. Click profile icon → Settings
2. Click "Notifications" in sidebar
3. Choose email and web preferences

**Watch/Unwatch Repositories:**
- **Watch:** Get notified of all activity
- **Unwatch:** Stop notifications
- **Custom:** Choose specific events

---

## Real-World Collaboration Scenarios

### Scenario 1: Team Project
```
Team creates repository
    ↓
Add all members as collaborators
    ↓
Create issues for tasks
    ↓
Assign issues to team members
    ↓
Each person works on branches
    ↓
Create PRs for review
    ↓
Team reviews each other's work
    ↓
Merge after approval
```

### Scenario 2: Open Source Contribution
```
Find interesting project
    ↓
Read CONTRIBUTING.md
    ↓
Look for "good first issue" label
    ↓
Fork the repository
    ↓
Make changes in your fork
    ↓
Create pull request to original
    ↓
Discuss with maintainers
    ↓
Update based on feedback
    ↓
Contribution gets merged! 🎉
```

### Scenario 3: Documentation Team
```
Create docs repository
    ↓
Non-technical team members added
    ↓
Use Issues for doc requests
    ↓
Use branches for major updates
    ↓
Use PRs for peer review
    ↓
Comments for suggestions
    ↓
Merge approved docs
```

---

## Practice Exercises

### Exercise 1: Issue Workflow
1. Create 3 issues in your repository with different labels
2. Assign them to yourself
3. Create a branch to fix one issue
4. Make changes and reference the issue in commit message
5. Create PR that closes the issue
6. Merge and verify issue auto-closes

### Exercise 2: Comment Practice
1. Go to your partner's repository
2. Find an interesting file
3. Fork their repository
4. Make a helpful addition
5. Create a PR to their repository
6. Add a nice description and @mention them

### Exercise 3: Issue Templates
1. Create an issue with a structured template
2. Include sections: Description, Tasks, Context
3. Use checkboxes for task lists
4. Add relevant labels
5. Demonstrate professional issue creation

---

## Collaboration Tips

### For Technical Teams:
- Use branches for all work
- Require PR reviews before merge
- Use CI/CD (automated testing)
- Tag releases
- Document decisions in issues/PRs

### For Non-Technical Teams:
- Use Issues for task tracking
- Review changes in PR "Files changed" tab
- Use Projects tab for kanban boards
- Keep commit messages simple and clear
- Focus on web interface

### For Mixed Teams:
- Use clear, jargon-free language
- Document processes in README
- Regular check-ins via Issues
- Pair technical and non-technical members
- Be patient and supportive

---

## Common Questions

**Q: Can I delete issues?**  
A: Not exactly, but you can close them. Closed issues are hidden by default but preserved for history.

**Q: What if someone creates spam issues?**  
A: Repository owners can block users and delete spam. For public repos, consider requiring contributors to sign in.

**Q: How do I know when someone responds?**  
A: Check the notifications bell icon or set up email notifications.

**Q: Can I work on someone's repo without forking?**  
A: Only if they add you as a collaborator. Otherwise, fork first!

**Q: What's the difference between issues and discussions?**  
A: Issues are for actionable tasks. Discussions (if enabled) are for open-ended conversations.

---

## Key Takeaways

✅ **Issues** = Project management and communication  
✅ **@mentions** = Get someone's attention  
✅ **Forks** = Your copy of someone else's project  
✅ **Collaboration** = More than just code  
✅ **Communication** = Be clear, kind, and constructive  

---

## What's Next?

You now know how to collaborate on GitHub! Next, we'll explore practical applications beyond just code.

Move on to **Exercise 06 - Practical Applications** to see how GitHub can help with documentation, project management, and more!

---

**Need help?** Check the [Cheat Sheet](../../CHEAT-SHEET.md) or ask your facilitator!

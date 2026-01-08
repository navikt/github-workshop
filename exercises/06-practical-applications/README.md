# Exercise 06 - Practical Applications: GitHub Beyond Code

**Time: 10 minutes**  
**Objective:** Discover how to use GitHub for documentation, project management, and non-code projects

---

## What You'll Learn
- How non-technical teams use GitHub
- GitHub for documentation and content
- GitHub Projects for task management
- GitHub Pages for free websites
- Real-world use cases

---

## GitHub Isn't Just for Code!

Many people think GitHub is only for programmers, but it's actually a powerful collaboration platform for **any** type of project involving files and teamwork.

### Who Uses GitHub for Non-Code Projects?

- 📚 **Writers** - Books, documentation, blog posts
- 🎨 **Designers** - Design specs, asset management
- 📊 **Data Teams** - Datasets, analysis documentation
- 📖 **Educators** - Course materials, lesson plans
- 🏢 **Operations Teams** - Policies, procedures, runbooks
- 📋 **Project Managers** - Requirements, roadmaps
- 🎯 **Marketing Teams** - Content calendars, copy

---

## Part 1: Documentation Management (3 minutes)

### Why GitHub for Documentation?

✅ **Version Control** - Track every change  
✅ **Collaboration** - Multiple people can contribute  
✅ **Review Process** - PRs catch errors before publishing  
✅ **History** - See how docs evolved  
✅ **Branching** - Draft major updates safely  
✅ **Search** - Built-in powerful search  

### Real-World Example: Team Handbook

Let's create a simple team handbook structure:

1. **Create a new file** in your repository: `team-handbook.md`

2. **Add this content:**

```markdown
# Team Handbook

## Welcome!
Welcome to our team! This handbook contains everything you need to know.

## Our Mission
[Your team's mission statement]

## Team Values
- **Collaboration:** We work together
- **Transparency:** We communicate openly  
- **Learning:** We grow continuously
- **Respect:** We value everyone's contributions

## How We Work

### Communication
- **Slack:** Day-to-day chat
- **Email:** Formal communications
- **GitHub:** Project discussions and documentation
- **Meetings:** Weekly sync-ups

### Working Hours
- Core hours: 10 AM - 3 PM (in your timezone)
- Flexible start and end times
- Notify team of time off

### Decision Making
1. Proposal phase (GitHub issue)
2. Discussion period (7 days)
3. Decision documented
4. Update handbook via PR

## Onboarding Checklist
For new team members:
- [ ] GitHub account created
- [ ] Added to team repository
- [ ] Read this handbook
- [ ] Schedule 1-on-1 with manager
- [ ] Meet the team
- [ ] Complete training modules

## Resources
- [Internal Wiki](link)
- [Training Materials](link)
- [FAQ](faq.md)

## Updates
This handbook is a living document. Suggest changes via Pull Request!

---
*Last updated: [Date]*
*Maintained by: [Team Name]*
```

3. **Commit the file**

**Benefits of This Approach:**
- Anyone can suggest updates via PR
- Changes are reviewed before going live
- Full history of all policy changes
- Easy to see who approved what and when

---

## Part 2: GitHub Projects (2 minutes)

**GitHub Projects** is a built-in kanban board for task management.

### Create a Project Board:

1. **Click the "Projects" tab** in your repository

2. **Click "New project"**

3. **Choose a template:**
   - Board (Kanban)
   - Table (Spreadsheet view)
   - Roadmap (Timeline view)

4. **Select "Board" and give it a name:**
   - "Personal Goals"
   - "Team Tasks"
   - "Content Calendar"

5. **Add items:**
   - Drag existing issues onto the board
   - Or create new items directly

### Project Board Columns:

**Basic Setup:**
- 📝 **To Do** - Planned work
- 🏃 **In Progress** - Currently working
- ✅ **Done** - Completed

**Advanced Setup:**
- 🎯 **Backlog** - Future ideas
- 🔜 **Next Up** - Prioritized
- 🚧 **In Progress**
- 👀 **Review** - Needs feedback
- ✅ **Done**

### Use Cases:

**Content Team:**
```
Columns: Ideas | Drafting | Review | Published
Items: Blog posts, videos, social content
```

**Event Planning:**
```
Columns: Brainstorm | Planning | In Progress | Complete
Items: Venue, catering, speakers, marketing
```

**Personal Projects:**
```
Columns: Someday | This Month | This Week | Done
Items: Learning goals, home projects, hobbies
```

---

## Part 3: GitHub Pages - Free Website Hosting (2 minutes)

**GitHub Pages** lets you host a website directly from your repository - for free!

### What Can You Build?

- Personal portfolio
- Project documentation
- Blog
- Team website
- Resume/CV
- Landing page

### Quick Setup:

1. **Go to repository Settings**

2. **Click "Pages" in the sidebar**

3. **Under "Source":**
   - Select branch: `main`
   - Select folder: `/root` or `/docs`

4. **Click "Save"**

5. **Your site will be published at:**
   ```
   https://yourusername.github.io/repository-name
   ```

### Simple GitHub Pages Example:

Create a file called `index.html`:

```html
<!DOCTYPE html>
<html>
<head>
    <title>My GitHub Page</title>
</head>
<body>
    <h1>Welcome to My Page!</h1>
    <p>This is hosted on GitHub Pages - for free!</p>
    
    <h2>About Me</h2>
    <p>I'm learning GitHub and loving it!</p>
    
    <h2>My Projects</h2>
    <ul>
        <li>Project 1</li>
        <li>Project 2</li>
        <li>Project 3</li>
    </ul>
</body>
</html>
```

**Even easier:** GitHub will automatically display your `README.md` as a website!

---

## Part 4: Real-World Use Cases (3 minutes)

### Use Case 1: Policy & Procedure Management

**Scenario:** Company policies that need version control and review

**Setup:**
```
policies-repo/
├── README.md (Index of all policies)
├── code-of-conduct.md
├── remote-work-policy.md
├── expense-reimbursement.md
├── security-guidelines.md
└── emergency-procedures.md
```

**Workflow:**
1. Propose policy update via branch
2. Team reviews via Pull Request
3. Requires approval from managers
4. Merge creates official update
5. History shows all changes and approvals

### Use Case 2: Recipe Collection

**Scenario:** Family recipe book with contributions

**Setup:**
```
family-recipes/
├── README.md
├── appetizers/
├── main-courses/
├── desserts/
└── drinks/
```

**Features:**
- Family members can add recipes via PR
- Issues for recipe requests
- Tags for dietary restrictions
- Photos using GitHub's image hosting
- Comments for modifications/reviews

### Use Case 3: Book/Novel Writing

**Scenario:** Writing a book with version control

**Setup:**
```
my-novel/
├── README.md (Synopsis, outline)
├── chapter-01.md
├── chapter-02.md
├── chapter-03.md
├── characters.md
├── worldbuilding.md
└── research-notes.md
```

**Benefits:**
- Track rewrites and revisions
- Create branches for alternate plots
- Editor provides feedback via PR comments
- Never lose a previous version
- Collaborate with co-authors

### Use Case 4: Meeting Notes

**Scenario:** Searchable, version-controlled meeting notes

**Setup:**
```
team-meetings/
├── README.md (Meeting schedule)
├── 2024/
│   ├── 2024-01-weekly-sync.md
│   ├── 2024-01-planning.md
│   └── 2024-02-weekly-sync.md
└── templates/
    └── meeting-template.md
```

**Template:**
```markdown
# Meeting: [Topic]
**Date:** YYYY-MM-DD
**Attendees:** @person1, @person2, @person3

## Agenda
1. Item 1
2. Item 2
3. Item 3

## Discussion Notes
[Notes here]

## Decisions Made
- Decision 1
- Decision 2

## Action Items
- [ ] @person1: Task 1 (Due: Date)
- [ ] @person2: Task 2 (Due: Date)

## Next Meeting
**Date:** [Next date]
**Topics:** [Preview]
```

### Use Case 5: Learning & Study Notes

**Scenario:** Personal knowledge base

**Setup:**
```
learning-notes/
├── README.md
├── programming/
│   ├── python.md
│   ├── javascript.md
│   └── git-github.md
├── languages/
│   ├── spanish.md
│   └── french.md
└── skills/
    ├── public-speaking.md
    └── project-management.md
```

---

## Additional GitHub Features

### GitHub Discussions

Enable for open-ended conversations:
- Q&A with community
- Show & Tell
- Ideas and brainstorming
- Announcements

### GitHub Wiki

Built-in wiki for documentation:
- More flexible than README
- Multiple pages
- Sidebar navigation
- Great for extensive docs

### GitHub Actions (Advanced)

Automate workflows:
- Auto-publish documentation
- Send notifications
- Run scheduled tasks
- Process data

### GitHub Gists

Quick snippets and small files:
- Share code snippets
- Quick notes
- Embed in websites
- No full repository needed

---

## Markdown Tips for Documentation

### Tables

```markdown
| Feature | Description | Status |
|---------|-------------|--------|
| Login | User auth | ✅ Done |
| Search | Find items | 🚧 In Progress |
| Export | Download data | 📋 Planned |
```

### Collapsible Sections

```markdown
<details>
<summary>Click to expand</summary>

Hidden content here!
- Point 1
- Point 2

</details>
```

### Task Lists

```markdown
- [x] Completed task
- [ ] Incomplete task
- [ ] Another task
```

### Callouts

```markdown
> **Note**
> This is important information

> **Warning**
> Be careful with this!
```

---

## Practice Ideas

### For Personal Use:
1. **Life Goals Tracker** - Track long-term goals with issues and projects
2. **Recipe Collection** - Digitize family recipes
3. **Travel Planning** - Plan trips with docs, checklists, research
4. **Reading List** - Track books with reviews and notes
5. **Study Notes** - Organize learning materials

### For Teams:
1. **Team Handbook** - Policies and procedures
2. **Meeting Notes Repository** - Searchable meeting history
3. **Project Documentation** - Technical and user docs
4. **Content Calendar** - Plan and track content
5. **Resource Library** - Curated links and materials

### For Communities:
1. **Community Guidelines** - Rules and expectations
2. **Event Planning** - Organize meetups and conferences
3. **Resource Collection** - "Awesome lists" of tools/resources
4. **Collaborative Writing** - Group projects and publications

---

## Key Takeaways

✅ **GitHub is for everyone** - Not just developers  
✅ **Version control** - Valuable for any file type  
✅ **Collaboration** - Built-in review and discussion  
✅ **Projects** - Free kanban boards  
✅ **Pages** - Free website hosting  
✅ **Flexible** - Adapts to many workflows  

---

## Common Questions

**Q: Can I use GitHub for non-text files?**  
A: Yes! Images, PDFs, etc. However, version control works best with text files (Markdown, code, etc.)

**Q: Is GitHub free for private repositories?**  
A: Yes! Free accounts include unlimited private repositories.

**Q: Can I use custom domains with GitHub Pages?**  
A: Yes! You can connect your own domain name.

**Q: How do I handle large files?**  
A: GitHub has size limits. For large files, consider Git LFS or external hosting.

**Q: Can non-technical team members use GitHub?**  
A: Absolutely! The web interface is user-friendly and doesn't require command-line knowledge.

---

## Resources for Learning More

### GitHub Features:
- [GitHub Pages](https://pages.github.com/)
- [GitHub Projects](https://docs.github.com/en/issues/planning-and-tracking-with-projects)
- [GitHub Discussions](https://docs.github.com/en/discussions)
- [GitHub Actions](https://docs.github.com/en/actions)

### Inspiration:
- Browse [GitHub Explore](https://github.com/explore)
- Search for "awesome-[topic]" repositories
- Look at documentation sites using GitHub
- Explore public organization repositories

---

## What's Next?

You've completed the main workshop exercises! You now know:
- ✅ How to create repositories
- ✅ How to commit changes
- ✅ How to use branches
- ✅ How to create pull requests
- ✅ How to collaborate with others
- ✅ How to use GitHub for various projects

### Continue Your Journey:

1. **Practice:** Use GitHub for your next project
2. **Explore:** Check out the [Resources](../../resources/) folder
3. **Contribute:** Find an open source project to contribute to
4. **Build:** Create your GitHub Pages portfolio
5. **Learn More:** Take GitHub Skills courses

---

**Congratulations on completing the GitHub for Dummies workshop! 🎉**

**Need help?** Check the [Cheat Sheet](../../CHEAT-SHEET.md) or ask your facilitator!

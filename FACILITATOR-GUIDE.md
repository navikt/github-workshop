# Facilitator Guide - GitHub for Dummies Workshop

**Workshop Duration:** 2 hours 15 minutes  
**Target Audience:** Tech and non-tech personnel  
**Prerequisites:** Laptop with internet connection only

---

## Pre-Workshop Checklist (1 week before)

### Technical Setup
- [ ] Create and populate this workshop repository
- [ ] **Enable GitHub Pages for presentation slides** (see [Presentation Setup](#presentation-setup) below)
- [ ] Test all exercise links and materials
- [ ] Test the presentation slides on your device
- [ ] Prepare demo account for demonstrations
- [ ] Test screen sharing/projection setup
- [ ] Verify WiFi capacity for expected attendance
- [ ] Prepare offline backup materials (PDFs of key exercises and slides)

### Materials Preparation
- [ ] Print cheat sheets (optional, 1 per participant)
- [ ] Print feedback forms
- [ ] Create sign-in sheet
- [ ] Prepare name tags
- [ ] Have GitHub stickers/swag ready (if available)

### Communication
- [ ] Send pre-workshop email with:
  - Workshop repository URL
  - Request to create GitHub account beforehand (optional but helpful)
  - What to bring (laptop, charger)

---

## Setup Day-Of (30 minutes before)

### Room Setup
- [ ] Test projector and screen visibility from all seats
- [ ] Ensure adequate power outlets
- [ ] Test WiFi connectivity
- [ ] Set up refreshments table
- [ ] Display welcome slide or agenda

### Technical Checks
- [ ] **Open presentation slides** in your browser (see slides URL below)
- [ ] Test slide navigation (Space, arrow keys, overview mode with Esc)
- [ ] Open workshop repository in browser
- [ ] Open GitHub docs in separate tab
- [ ] Test screen sharing with slides
- [ ] Have backup phone hotspot ready
- [ ] Clear browser cache/cookies for clean demo

---

## Presentation Setup

### Accessing the Slides

**Live URL:** `https://yourusername.github.io/github-workshop/slides/`
(Replace `yourusername` with your GitHub username)

**Local Backup:** Open `slides/index.html` in your browser

### Enabling GitHub Pages

1. Go to repository **Settings** → **Pages**
2. Under **Source**, select:
   - Branch: `main`
   - Folder: `/ (root)`
3. Click **Save**
4. Wait 1-2 minutes for deployment
5. Test the URL

### Presentation Controls

- **Space** or **→**: Next slide
- **←**: Previous slide
- **Esc** or **O**: Overview mode (see all slides)
- **F**: Fullscreen
- **?**: Help menu

### Customizing Slides

Edit `slides/index.html` to:
- Change theme (line 10)
- Update your repository URL (final slide)
- Add your branding or logo
- Modify content as needed

See `slides/README.md` for detailed customization instructions.

---

## Workshop Flow & Timing

### Part 1: Introduction & Setup (30 minutes)

**Welcome & Overview (5 minutes)**
- **Start with presentation slides** - show title slide
- Start on time - respect everyone's schedule
- Introduce yourself and your GitHub experience
- Quick icebreaker: "What's one thing you want to learn today?" (slide includes this)
- Set expectations: hands-on, questions welcome, no "dumb" questions
- Point out restrooms and refreshments
- **Use slides for agenda overview** - shows workshop structure clearly

**What is GitHub? (10 minutes)**
- **Use presentation slides** - follows outline closely with visual aids
- **Key Message:** GitHub makes collaboration easy and tracks all changes
- Use analogies your audience will understand (slides include these):
  - Non-tech: "Like Google Docs but for any file, with superpowers"
  - Tech: "Distributed version control with collaboration features"
- Show real-world example: browse a popular open-source repo
- Emphasize: You cannot break GitHub by experimenting
- **Slides cover:** Version control, Git vs GitHub, analogies, capabilities, use cases

**Pacing Tips:**
- Don't get bogged down in Git vs GitHub differences
- If someone asks about command line, acknowledge but defer: "We'll use the web interface today, CLI is Workshop 2"
- Watch for confused faces - pause and rephrase

**Account Creation & Setup (15 minutes)**
- Walk through account creation step-by-step
- Common issues:
  - Username already taken → suggest adding numbers or variations
  - Email verification delay → check spam folder
  - Password requirements → use password manager
- While waiting for email verification, give brief UI tour
- Have participants follow along on their screens

---

### Part 2: GitHub Basics - Hands-On (40 minutes)

**Understanding Repositories (10 minutes)**
- Live demo: Create a repository yourself first
- Then have participants create their own: "my-first-repo"
- Encourage creative README content: hobby, favorite recipe, travel bucket list
- Introduce Markdown as "formatting codes" - show headers, lists, bold
- Common issues:
  - Forgetting to check "Add a README file" → show how to add later
  - Public/private confusion → explain clearly, show how to change later

**Making Your First Changes (15 minutes)**
- Demo the edit workflow before having participants try
- Emphasize commit messages: "Future you will thank you"
- Good vs bad commit message examples:
  - ❌ "changes"
  - ❌ "update"
  - ✅ "Add favorite books section"
  - ✅ "Fix spelling in introduction"
- Have everyone make 2-3 commits to build confidence
- Show commit history and how to view previous versions

**Branches: Working Safely (15 minutes)**
- **Most important concept:** Branches let you experiment safely
- Analogy: "Parallel universes for your project"
- Live demo:
  1. Create branch "add-contact-info"
  2. Make changes
  3. Switch to main → changes disappear (magic!)
  4. Switch back → changes reappear (more magic!)
- Have participants create a branch and make changes
- Common confusion: "Where did my changes go?" → explain branch context

**Troubleshooting:**
- If someone gets lost, pair them with a neighbor who's ahead
- If Wi-Fi fails, switch to phone hotspot for one person to demo
- If multiple people stuck on same issue, stop and re-demonstrate for everyone

---

### Break (10 minutes)

**Facilitator Tasks During Break:**
- Identify anyone who needs catch-up help
- Check pacing vs schedule
- Reset demo environment if needed
- Answer individual questions

---

### Part 3: Collaboration Fundamentals (30 minutes)

**Pull Requests: Proposing Changes (15 minutes)**
- **Key Message:** PRs are how teams review work before it goes live
- Demo the full PR workflow:
  1. Create branch
  2. Make changes
  3. Open PR
  4. Write description (explain WHAT and WHY)
  5. Show the diff view
  6. Merge PR
  7. Delete branch (cleanup habit)
- Have participants do their first PR
- Explain merge conflicts simply: "Like two people editing same line in Google Docs"
- Don't create actual merge conflicts unless time permits

**Working with Others (15 minutes)**
- **Partner Exercise Setup:** Pair participants (tech with non-tech if possible)
- Each person:
  1. Shares their repository URL with partner
  2. Partner creates an issue
  3. Practice @mentioning
  4. Respond to the issue
- Briefly explain forking: "Making your own copy of someone else's project"
- Show how to watch repository for notifications

**Pacing Adjustment:**
- If running behind: Skip forking demo, focus on issues only
- If ahead: Show GitHub Projects board

---

### Part 4: Practical Applications & Next Steps (15 minutes)

**GitHub Beyond Code (5 minutes)**
- Show real examples:
  - Documentation repository
  - Marketing team using GitHub
  - Meeting notes in a repo
  - Personal knowledge base
- Emphasize: GitHub isn't just for programmers

**GitHub Desktop & VS Code (3 minutes)**
- Quick mention only: "These tools exist for working offline"
- Show screenshots, don't do live demo unless requested
- Position as "next level" for follow-up workshop

**Next Steps & Resources (7 minutes)**
- Share this repository URL (has all links)
- Recommend:
  - GitHub Skills (skills.github.com) - interactive tutorials
  - Practice by creating a personal project
  - Join open source projects (awesome-for-beginners)
- Set expectations: "Use it or lose it" - practice within next week

---

### Wrap-Up (10 minutes)

**Q&A Session (7 minutes)**
- Common questions:
  - "Can I use GitHub for [specific use case]?" → Usually yes
  - "Is it really free?" → Yes for public repos and small teams
  - "What if I mess up?" → Show how to revert commits
  - "Do I need to learn command line?" → No, but it's powerful

**Feedback & Closing (3 minutes)**
- Collect feedback forms
- Share your contact info for follow-up questions
- Mention follow-up workshops if planned
- Thank everyone for participating
- Encourage: "You're now GitHub users! The best way to learn is to use it."

---

## Common Pitfalls & Solutions

### Technical Issues

**Problem:** WiFi too slow for everyone to sign up at once  
**Solution:** Have participants create accounts in shifts, or beforehand

**Problem:** Email verification not arriving  
**Solution:** Check spam folder, try resending, use alternate email

**Problem:** Screen sharing lag/freezing  
**Solution:** Close unnecessary applications, use simplified view

**Problem:** Participant's browser not supported  
**Solution:** Have Chrome/Firefox/Edge download links ready

### Conceptual Confusion

**Problem:** "I don't understand branches"  
**Solution:** Use the parallel universe analogy, show visual diagram, live demo switching

**Problem:** "What's the difference between commit and push?"  
**Solution:** For web interface, they're the same action. Explain push is for local work (defer to Workshop 2)

**Problem:** "I'm afraid to break something"  
**Solution:** Reassure that it's nearly impossible to cause damage. Show how to undo changes

**Problem:** Terminology overload  
**Solution:** Keep a glossary visible, use consistent simple terms, relate to familiar concepts

### Engagement Issues

**Problem:** Some participants racing ahead  
**Solution:** Have stretch activities ready (customize profile, explore GitHub Explore page)

**Problem:** Some participants falling behind  
**Solution:** Implement buddy system, pause for group catch-up, simplify exercises

**Problem:** Mixed technical levels causing frustration  
**Solution:** Pair tech with non-tech, validate all skill levels, offer alternative explanations

---

## Post-Workshop Follow-Up

### Within 24 Hours
- [ ] Send thank you email with:
  - Workshop repository link
  - Links to all resources mentioned
  - Recording link (if applicable)
  - Your contact info for questions
  - Feedback form (if not collected)

### Within 1 Week
- [ ] Review feedback and identify improvement areas
- [ ] Answer any email follow-up questions
- [ ] Share common Q&A document if useful
- [ ] Consider office hours for additional help

### Within 1 Month
- [ ] Check in with participants (optional survey)
- [ ] Announce follow-up workshop dates
- [ ] Create alumni Slack/Discord channel
- [ ] Share success stories

---

## Backup Plans

### If WiFi Fails
1. Use phone hotspot for one laptop to demo
2. Work from screenshots/offline PDFs
3. Focus on concepts vs hands-on
4. Schedule make-up hands-on session

### If Running Short on Time
**Priority Order:**
1. ✅ Account creation + repo creation
2. ✅ Making commits
3. ✅ Branches basics
4. ⚠️ Shorten: Pull request demo (demo only, skip participant exercise)
5. ❌ Skip: Partner exercises, forking, GitHub Desktop

### If Running Long on Time
**Stretch Activities:**
1. Customize GitHub profile README
2. Explore GitHub Projects/Issues more deeply
3. Show GitHub Actions example
4. Browse interesting open source repos together
5. Start on GitHub Pages basics

---

## Success Metrics

Participants should leave able to:
- ✅ Explain what GitHub is in their own words
- ✅ Create a repository
- ✅ Make commits with good messages
- ✅ Create and switch between branches
- ✅ Open and merge a pull request
- ✅ Know where to find help

**Red Flags:**
- More than 20% of participants lost during Part 2
- No questions asked (might indicate confusion, not understanding)
- Participants leaving early
- Majority not completing hands-on exercises

---

## Additional Resources for Facilitators

### Recommended Reading
- [GitHub Docs - Quickstart](https://docs.github.com/en/get-started/quickstart)
- [GitHub Skills](https://skills.github.com/)
- [Pro Git Book (free)](https://git-scm.com/book/en/v2)

### Workshop Inspiration
- GitHub Universe talks
- GitHub Education Community
- Meetup groups for Git/GitHub

### Continuous Improvement
- Collect feedback every session
- Iterate on materials based on common questions
- Share learnings with other facilitators
- Stay updated on GitHub feature changes

---

## Contact & Support

**Workshop Materials Issue?**
- Open an issue in this repository
- Contact: [Your contact info]

**Want to Run This Workshop?**
- Feel free to fork and adapt these materials
- Attribution appreciated but not required
- Share improvements back via pull request

---

**Good luck with your workshop! Remember: enthusiasm is contagious. Your excitement about GitHub will inspire your participants. 🚀**

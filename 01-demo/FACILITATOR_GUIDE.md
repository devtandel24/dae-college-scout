# FACILITATOR GUIDE
## Beyond the Chatbot — Agentic AI for High School Students
### Wednesday, June 3, 2026 · Synchrony Skills Academy · 4:30–6:00 PM

**This is your private prep doc. Don't put this in the public repo. Keep it in your `01-demo/` (gitignored) folder.**

---

## TABLE OF CONTENTS

1. Tonight's prep checklist
2. Day-of arrival checklist (30 min before)
3. The opening demo script (90 seconds)
4. The full 45-minute run of show
5. The closing 90 seconds (the WORKdae pitch)
6. Contingency plans (when things break)
7. The post-workshop follow-up

---

## 1. TONIGHT'S PREP CHECKLIST

**Total time: ~3-4 hours.** Set aside the evening.

### A. Set up your GitHub repo (30 min)

- [ ] Go to https://github.com/devtandel24/dae-college-scout
- [ ] Upload all the files from this output folder into the matching repo structure:
  - `README.md` → repo root
  - `02-workshop/README.md` → repo `02-workshop/` folder
  - `02-workshop/SETUP.md` → repo `02-workshop/`
  - `02-workshop/system-prompt.md` → repo `02-workshop/`
  - `02-workshop/workflow.md` → repo `02-workshop/`
  - `02-workshop/profile-template.md` → repo `02-workshop/`
  - All 5 persona JSON files → `04-assets/sample-personas/`
- [ ] Test the download flow: open in incognito → click green `<> Code` → Download ZIP → unzip → verify all files are there
- [ ] Generate a QR code pointing to your repo URL. Use a free tool like qr-code-generator.com. Print it BIG (at least 4"×4") for tomorrow.

### B. Set up the 4 shared Claude accounts (60 min)

For each of the 4 DAE-shared Claude accounts:

- [ ] Log in. Verify you can access Projects (free tier supports up to 5 projects per account)
- [ ] **For ONE account (the "demo account") only:**
  - [ ] Connect Gmail via MCP connector (authorize with a DAE Gmail you control)
  - [ ] Connect Google Drive via MCP connector
  - [ ] Connect Google Calendar via MCP connector
  - [ ] This is the account you'll use for your live demo — the agent will actually send emails, create folders, and add calendar events from this one
- [ ] **For the other 3 accounts (the "student accounts"):**
  - [ ] Do NOT connect Gmail/Drive/Calendar — students will use them without the live-action extras
  - [ ] Their agents will draft emails into a chat artifact instead of sending live
  - [ ] Confirm Web Search is toggleable
- [ ] Write down login credentials for all 4 accounts. You'll hand these out tomorrow on printed slips.

### C. Build your live demo (60 min)

This is the 90-second opener that hooks the room. Build it tonight so tomorrow it just works.

- [ ] On the demo account (with Gmail/Drive/Calendar connected), create a project called `Alex's College Scout`
- [ ] Use one of the sample personas — I recommend **persona-builder.json (Jordan Patel)** or build your own "Alex" — and load:
  - Convert the persona JSON to a clean markdown profile and upload it to project knowledge
  - Upload `workflow.md` to project knowledge
  - Paste `system-prompt.md` content into the project instructions, replacing `[Student Name]` with `Alex`
- [ ] Turn on Web Search
- [ ] **Run a test:** type `Scout my schools`. Verify:
  - The agent narrates its work
  - Web searches fire and are visible
  - A Canvas/Artifact report appears with Alex's name on it
  - The agent then asks if you want the agentic extras
  - When you say yes, it actually:
    - Creates the Drive folder (check Google Drive — should be a folder titled "Alex's College Scout")
    - Drafts a Google Doc with 5 emails
    - Creates a Sheet tracker
    - Adds calendar events with 2-week reminders
    - Sets a 2-week follow-up reminder
- [ ] **If anything broke:** debug tonight, not tomorrow. The demo MUST work.
- [ ] Once it works, **don't clear the project.** You'll use this exact setup as your live demo opener.

### D. Prep your room materials (30 min)

- [ ] Printed QR code (4"×4" minimum)
- [ ] 4 printed slips with each shared Claude account's login credentials (one slip per group)
- [ ] A few printed copies of the SETUP.md (backup for students who can't easily flip between repo and Claude)
- [ ] Your laptop, charged
- [ ] HDMI / USB-C adapter for the projector at Synchrony Skills Academy
- [ ] Bluetooth speaker (optional but recommended for music during build phase)
- [ ] A playlist queued: lo-fi beats, instrumental hip hop, something energetic but not distracting. Spotify "Lofi Beats" works.
- [ ] One slide deck — just 3 slides:
  - Slide 1: "Beyond the Chatbot — let's build" (hook)
  - Slide 2: The challenge brief + idea reminders
  - Slide 3: QR code + DAE plug at the end

### E. Final sanity check (15 min)

- [ ] Open the repo on your phone — does the README look clean?
- [ ] Walk through SETUP.md as if you're a student — does it make sense? Are there any steps that confuse you?
- [ ] Sleep on it. Don't tinker past midnight.

---

## 2. DAY-OF ARRIVAL CHECKLIST (30 min before kickoff)

Arrive at Synchrony Skills Academy by **4:00 PM** for a 4:30 PM start.

- [ ] Test the projector with your laptop — confirm display works
- [ ] Test the room's Wi-Fi from your laptop and from one other device (phone). Confirm you can reach claude.ai and github.com
- [ ] Open your demo Claude project — make sure it loads
- [ ] Play music quietly through your Bluetooth speaker as students arrive (sets the vibe immediately)
- [ ] Put the QR code on a table or stick it on the wall at the front
- [ ] Lay out the printed account credential slips at the 4 group "stations"
- [ ] Take a breath. You're ready.

---

## 3. THE OPENING DEMO SCRIPT (90 seconds — the most important moment)

**At 4:30 sharp** (or whenever you start), kill the music. Stand at the front.

> *"Hey. We're going to do this fast. In 45 minutes, every single one of you is going to build your own AI agent that finds your best-fit colleges, trade schools, or whatever comes next. Not a chatbot. An agent. There's a difference. Let me show you."*

Click into your pre-built demo Project. The Project Knowledge sidebar should be visible — students see the profile already loaded. Type slowly:

```
Scout my schools
```

Hit enter. **Don't narrate.** Let them watch.

The agent will:
- Start narrating ("Got your profile, Alex. Searching College Scorecard...")
- Show web searches firing in real time
- Generate a Canvas artifact with Alex's name on it
- Then ask if you want the agentic extras

When the agent asks, type:
```
yes do it all
```

The agent will:
- Send 5 emails (you'll see "Sent" confirmations)
- Create a Drive folder (you can switch tabs to Google Drive briefly and show it)
- Add calendar events (switch to Calendar and show them populated)
- Set the follow-up reminders

**Total time elapsed: ~90 seconds to 2 minutes.**

When it's done, turn to the room:

> *"That's what we're building. The agent had memory — Alex's profile. It used real tools — web search, Gmail, Drive, Calendar. It made decisions — which schools, which scholarships. It acted in the real world — emails went out, files got created, deadlines hit the calendar. That's an agent.*
> 
> *Your version is going to be slightly simpler because we don't have everyone's Gmail connected — but you're going to build the same thing, with YOUR profile, and walk out with a Scout Report and a draft email batch you can actually send tonight.*
> 
> *Let's go."*

Click to Slide 2 (challenge brief + idea reminders) or just dive into setup.

---

## 4. THE FULL 45-MINUTE RUN OF SHOW

### MINUTE 0-2 — The Opener
Demo script above. 90 seconds, no narration during the demo itself.

### MINUTE 2-3 — The Concept Land
After the demo, the brief explanation:

> *"What just happened: memory, tools, decisions, action. That's the architecture of every agent. ChatGPT is a chatbot. What you just saw was an agent. Different thing.*
> 
> *Today you build yours. 45 minutes. Here we go."*

### MINUTE 3-8 — Setup Phase

Show the QR code on screen.

> *"Scan this. It takes you to the GitHub repo. Click the green 'Code' button, download the ZIP, unzip it. While you're doing that, your facilitator [or YOU] is going to walk around and hand out Claude account logins."*

Walk around. Hand out the 4 printed credential slips. Get students into groups of 4-5 per account. Note: same account = different projects, so each student still has their own work.

While students download and log in, address the room periodically:

> *"You should be logged into claude.ai. Now create a new project — left sidebar, plus button. Name it [your first name]'s College Scout."*

### MINUTE 8-25 — The Build (17 minutes)

This is the meat. Walk through it on the big screen, pause for them to catch up at each step.

**Minutes 8-10 (project setup):**
- Demo on screen: create project, name it
- Wait for everyone

**Minutes 10-20 (PROFILE FILLING — this is where energy can dip):**
- Open the profile template on screen
- Walk them through the 9 sections briefly
- **Hype this part.** "Section 3d is huge — what have you BUILT?" "Be specific. 'I like art' is weak. 'I run an Instagram art account with 2,000 followers' is gold."
- Play music quieter so they can think
- Walk around. Look at what people are writing. **Roast lazy answers playfully.** "That can't be your most interesting thing. Try again."
- Help anyone stuck — if they're undecided, tell them to embrace it; if they're an athlete, ask about leadership; if they're a builder, ask what they've shipped
- Time-box this: at minute 18-19, give a 1-minute warning. At minute 20, **move on.**

**Minutes 20-23 (upload + paste + configure):**
- Demo on screen: save the profile, upload to Project Knowledge, upload workflow.md, paste system-prompt.md into instructions, replace [Student Name] with their name, turn on Web Search
- Walk around to make sure no one's stuck

**Minutes 23-25 (the moment):**
At minute 23, gather attention:

> *"Everyone ready? On three, hit enter. Three, two, one — SCOUT MY SCHOOLS, GO."*

Energy spikes here. Multiple agents fire across the room. Walk around. **React out loud to what you see.** "Oh that's a sick wildcard pick." "WAIT it found a $20K scholarship for you?" Hype every screen.

### MINUTE 25-35 — Watch the agent work + first iteration (10 min)

**Minutes 25-30:** Students sit and watch their agents narrate, search, and generate reports. Their reports appear as Canvas artifacts. Let them read.

**Minutes 30-35:** Push them to iterate.

> *"Now the cool part. Your agent remembers everything. Push it. Ask follow-ups."*

On the big screen, demo a follow-up on your demo account: type something like `What about West Coast schools only?` and watch it re-run with full context. Then say:

> *"Try one. Pick anything. 'Show me cheaper options.' 'Find me 5 more scholarships.' 'Help me write my application essay for #1.' Go."*

Walk around. React to interesting follow-ups. This is where students realize they OWN something that works for them.

### MINUTE 35-40 — Showcase (5 min)

> *"Three volunteers — get up here and show us your top match and one thing your agent did that surprised you."*

Three quick demos, ~90 seconds each. React big. If one student got an amazing wildcard pick, lean into it. If one student got a great scholarship match, lean into it.

If no one volunteers, pick one. (You'll have noticed good ones while walking around.)

### MINUTE 40-42 — Land the lesson (2 min)

Stop. Voice gets quieter. Real talk:

> *"What you just built isn't a college tool. It's a real agent.*
> 
> *It has memory — your profile, sitting in the project. It has tools — web search, and on my demo account, Gmail and Calendar. It has a process — the workflow you uploaded. It has a goal — your prompt.*
> 
> *That's the architecture of every AI agent in the world right now. You just built one. In 45 minutes."*

### MINUTE 42-45 — The pitch + close (3 min)

> *"Three things before we wrap:*
> 
> *One: this project lives in your account [or the shared account — facilitators will help you transfer it later if you want]. Update your profile next time you take a test, run it again, watch it get smarter about you.*
> 
> *Two: the emails your agent drafted are sitting in your chat. Copy them into your own Gmail tonight. Send them. American colleges track 'demonstrated interest' — these emails actually matter for your application.*
> 
> *Three: what you learned in 45 minutes is the foundation. There's a 6-week version of this — DAE's WORKdae course — where you build agents for anything in your life. If today made you want more, come talk to me after this.*
> 
> *Thanks for being here. Now go send your emails."*

End. Done. Drop the mic.

---

## 5. THE CLOSING 90 SECONDS (THE WORKdae PITCH)

If anyone hangs around after, here's how to talk about WORKdae:

> *"What you did today is Week 1 of WORKdae. Week 1 is awareness — agent vs chatbot, four pillars, what's possible. The 5 weeks after that go deeper:*
> 
> *Week 2: how to find what already exists in the world and connect it to your work.*
> 
> *Week 3: real automation — workflows that run without you, on a schedule, calling APIs, doing things in the background.*
> 
> *Week 4: orchestration — multiple agents working together, knowledge bases, real memory.*
> 
> *Week 5: making it reliable — debugging, verification, knowing when to trust an agent and when to check.*
> 
> *Week 6: scaling — going from one agent to a system of agents that runs your work.*
> 
> *It's a paid 6-week program. Mostly for working professionals but high schoolers absolutely qualify — and honestly, you'd dominate it. Want details? Here's my email."*

---

## 6. CONTINGENCY PLANS (WHEN THINGS BREAK)

### Wi-Fi goes down
- Have students tether to their phone hotspots
- Worst case: do a group walkthrough using your laptop on cellular tether — students follow along by reading

### A shared Claude account hits rate limits / locks
- Have a 5th backup account ready (create tonight)
- Or: swap students to a less-busy account
- Free tier limits reset on a 5-hour rolling window, so even an hour wait would work

### A student's agent gives a weird/bad output
- This is a TEACHING MOMENT, not a failure
- Walk them through: "What's wrong with it? Tell the agent specifically what to fix. 'That recommendation didn't reference my profile section 3d. Try again with the schools that actually match what I've built.'"
- Watching them debug is the actual skill being taught

### A student can't think of what to put in the profile
- Show them a sample persona for inspiration (point them to `04-assets/sample-personas/`)
- Or coach them: "What's one thing you did this year you're proud of?" "What annoys you about school?" "If you could quit school tomorrow and do anything, what would it be?"

### A student is dismissive / not engaged
- Skip them. Don't fight it. Other students will see the excitement and pull them in eventually.
- Or pair them with someone who's hyped — energy is contagious.

### You run behind on the build phase
- Skip the iteration phase (minutes 30-35)
- Go straight to showcase
- Showcase is the non-negotiable — it's where the social proof lands

### The demo fails at minute 0
- This is why you tested it tonight
- If it fails live: stay calm. Say "okay technical hiccup, while I sort this out, scan the QR code and start downloading the repo." Buy yourself 2 minutes to debug, then re-run.
- Backup: have a screen recording of your demo from tonight saved on your laptop. Play it as a video if live fails.

### You go OVER 45 minutes
- The workshop is in a 4:30-6:00 PM window — you have buffer
- Cut your closing pitch shorter, never cut the showcase
- Or extend slightly if students are engaged — Synchrony Skills Academy will be flexible

---

## 7. POST-WORKSHOP FOLLOW-UP

### Immediately after (within 1 hour)
- Save any student work / Drive folders that students want kept (since they used shared accounts, their projects might disappear when accounts get cleaned up later)
- Take photos of the room, screens with reports, any moments worth posting on DAE's socials

### Within 24 hours
- Email anyone who showed interest in WORKdae with details + next cohort dates
- Post 1-2 screenshots of student Scout Reports (with their permission) on DAE's social media
- Update the GitHub repo's README with a "successfully delivered to X students" line if you want

### Within a week
- Send a recap to Synchrony Skills Academy with attendance, what worked, what could improve
- Ask students who attended for testimonials — these become marketing for WORKdae

---

## ONE FINAL THING

You've done a LOT of prep. Tomorrow, **trust the prep.** Don't add new things in the moment. Don't second-guess the structure.

The students don't need it perfect. They need it real, fast, and engaging.

You've got this.

— Made with care for tomorrow. Good luck.

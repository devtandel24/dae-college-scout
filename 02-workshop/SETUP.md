# SETUP — Build Your College Scout in 11 Steps

Total time: ~15 minutes to set up, ~5 minutes to run, ~5 minutes to review and approve.

---

## What you need

- A laptop with a browser
- A Google account (you definitely already have one)
- The DAE-shared Claude account login your facilitator will give you
- This downloaded repo (unzipped on your computer)

---

## STEP 1 — Log into Claude

Go to **claude.ai** and log in with the account credentials your facilitator handed out.

You'll share this account with 3-4 other students. That's fine — each of you will work in your own project, which keeps your work separate.

---

## STEP 2 — Create your project

In the left sidebar, find **"Projects"** and click the **+** to create a new one.

**Name it:** `[Your First Name]'s College Scout`

Example: `Marcus's College Scout`, `Maya's College Scout`

---

## STEP 3 — *(OPTIONAL but recommended if you're 18+)* — Connect your Gmail and Drive

This step lets your agent actually send emails from YOUR Gmail and save files to YOUR Drive.

**If you're 18 or older:**

1. In your Claude project, find the **Connectors** or **Integrations** section
2. Click **Connect Gmail** → authorize with YOUR Google account (the one you'll be using throughout high school and into college)
3. Click **Connect Google Drive** → authorize the same Google account
4. Click **Connect Google Calendar** → same account

Now your agent can send emails as you, save files to your Drive, and load deadlines into your calendar.

**If you're under 18 or can't connect:** Skip this step. Your agent will save email drafts and reports to the chat instead — you'll copy them into your own Gmail/Drive later. Still works great.

---

## STEP 4 — Open the profile template

In the repo folder you downloaded, open:

```
02-workshop/profile-template.md
```

Open it in any text editor (Notes app, Google Docs, Word, whatever).

---

## STEP 5 — Fill out your profile

**This is the most important part.** Your agent is only as good as your profile.

Tips:
- **Skip what doesn't apply.** Not in sports? Skip Section 3a.
- **Be specific.** "I like science" is weak. "I love biology and chemistry, hate physics" is gold.
- **Section 3d (Things You've Built) is huge.** Write down every project, side hustle, content channel — anything you've shipped that exists in the world.
- **No idea what you want to do? Say so.** "I have absolutely no idea" is a valid answer in Section 7.

**Take ~10 minutes on this.** Don't rush.

---

## STEP 6 — Save your filled profile

Save your filled-out profile as a file. Any of these formats work:
- `.md` (markdown)
- `.txt` (plain text)
- `.pdf`
- `.docx` (Word)

Name it: `My_Profile.md` (or similar)

---

## STEP 7 — Upload your profile to Project Knowledge

In your Claude project, find **"Project Knowledge"** and drag your profile file in.

You should see it show up in the knowledge list.

---

## STEP 8 — Upload the workflow file

In the repo folder, find:

```
02-workshop/workflow.md
```

Upload to Project Knowledge (same way as Step 7).

---

## STEP 9 — Set the system prompt

In the repo folder, open:

```
02-workshop/system-prompt.md
```

**Select all the text inside that file and copy it.**

In your Claude project, find **"Custom Instructions"** (sometimes called "Project Instructions" or "Project Description").

**Paste the system prompt in there.**

Then find this line in the prompt:
```
You are the College Scout, a personal AI agent built for [Student Name].
```

**Replace `[Student Name]` with your actual first name.** Save.

---

## STEP 10 — Turn on Web Search

In the Claude chat interface, find the **Web Search** toggle and turn it ON.

---

## STEP 11 — Run your agent

In the chat, type exactly this:

```
Scout my schools
```

Hit enter.

**Watch your agent work.** It'll narrate what it's doing — searching, ranking, generating.

In about 2-3 minutes, your agent will:
1. Send you a Google Drive link to your beautifully designed HTML Scout Report
2. NOT dump the report in chat (the chat stays clean — the report lives in Drive)
3. Give you a 2-line teaser about what surprised it
4. Ask you to review the report and approve

---

## STEP 12 — Review your report in Drive

**This is the human-in-the-loop moment.**

Click the Drive link. The HTML report opens in your browser. Read it.

- ✅ Does it feel like it actually understands you?
- ✅ Are the schools real fits or generic suggestions?
- ✅ Do the "Why this fits YOU" paragraphs reference YOUR profile specifically?

---

## STEP 13 — Approve or refine

**If the report is good:**

Come back to Claude chat and type:
```
approved
```

The agent will then:
- Send emails (if you connected Gmail in Step 3) OR save them as drafts in Drive
- Create a College Tracker spreadsheet
- Add all application & scholarship deadlines to your calendar
- Set 2-week reminders before each deadline
- Set follow-up check-ins for 2 weeks and 4 weeks from today

**If the report needs work:**

Tell the agent specifically what to fix. Examples:
- `Add more West Coast options`
- `Drop the schools over $30K`
- `Find me 2 more HBCUs to consider`
- `The wildcard pick doesn't fit me — try a different one`

The agent will regenerate the HTML report in Drive (same folder, updated file) and ask you to approve the new version.

---

## STEP 14 — Push your agent

After everything's set up, push it further. Try:
- `What if I improved my SAT by 100 points — does that change anything?`
- `Help me draft my application essay for school #1`
- `Compare schools 2 and 4 — which is better for me?`
- `What about a community college path that transfers to one of these schools?`

Watch how it remembers everything and re-runs with full context. That's what an agent is.

---

## Stuck?

- **Profile feels overwhelming?** Look at the sample personas in `../04-assets/sample-personas/` for inspiration.
- **Agent gave a weird response?** Tell it exactly what was wrong. Be specific.
- **HTML report didn't generate?** Make sure Web Search is on and you've uploaded both the profile AND the workflow.md file to Project Knowledge.
- **Something else broken?** Raise your hand. Your facilitator is in the room.

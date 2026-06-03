# SETUP — Build Your College Scout

Total time: ~12 minutes to set up, then your agent takes over.

---

## What you need

- A laptop with a browser
- A Google account
- The DAE-shared Claude account login from your facilitator
- This downloaded repo (unzipped on your computer)

---

## STEP 1 — Log into Claude

Go to **claude.ai** → log in with the credentials your facilitator hands out.

You'll share this account with 3-4 other students. Each of you works in your own project — your work stays separate.

---

## STEP 2 — Create your project

Left sidebar → **Projects** → click **+** → New Project

**Name it:** `[Your First Name]'s College Scout`

Example: `Marcus's College Scout`

---

## STEP 3 — *(Optional — if you're 18+)* Connect Gmail, Drive, Calendar

This lets your agent create real Gmail drafts, save files to your Drive, and load deadlines into your calendar.

1. In your project → find **Connectors** or **Integrations**
2. Connect **Gmail** → authorize with YOUR Google account
3. Connect **Google Drive** → same account
4. Connect **Google Calendar** → same account

**Under 18 or want to skip?** The agent still works — emails and files go to the shared account's Drive instead. You can access them from there.

---

## STEP 4 — Upload the workflow file

In the repo folder you downloaded, find:
```
02-workshop/workflow.md
```

In your Claude project → **Project Knowledge** → drag this file in.

This is your agent's process — the step-by-step it follows.

---

## STEP 5 — Set the system prompt

In the repo folder, open:
```
02-workshop/system-prompt.md
```

**Select all → copy.**

In your Claude project → **Custom Instructions** → paste.

Find this line:
```
You are the College Scout, a personal AI agent built for [Student Name].
```

**Replace `[Student Name]` with your actual first name.** Save.

---

## STEP 6 — Turn on Web Search

In the Claude chat → find the **Web Search** toggle → turn it **ON**.

---

## STEP 7 — Start your agent

Type this in the chat:

```
Scout my schools
```

**What happens next depends on whether you uploaded a profile:**

**If you didn't upload a profile** (most students in the workshop):
Your agent will ask you questions directly in the chat — like a quiz. Answer honestly, skip anything that doesn't apply or that you'd rather not share. Takes about 5 minutes. The agent saves your answers to Drive automatically.

**If you already uploaded a profile** (see the note below):
Your agent detects it automatically and goes straight into research.

---

## STEP 8 — Answer your agent's questions

The agent will ask 4 rounds of questions. Answer each round, then wait for the next.

Tips:
- **Round 2, Question 7 (things you've built) is the most important.** Be specific — apps, businesses, content channels, research, anything you've created.
- Skip any question you'd rather not answer — just say "skip" or leave it blank.
- No test scores yet? Say so. The agent adapts.
- Genuinely undecided on career or college path? Say so. The agent handles it.

---

## STEP 9 — Watch your agent work

After your questions, the agent runs research. You'll see short status pings in chat. In 2-3 minutes:

- It sends you a **Google Drive link** to your personalized Scout Report
- A 2-sentence teaser about what surprised it
- A request for your approval

---

## STEP 10 — Review your report in Drive

Click the Drive link. The HTML report opens in your browser.

Ask yourself:
- Do these schools actually fit me?
- Does the "Why this fits YOU" section reference things from MY life?
- Is the Safety realistic? Is the Wildcard interesting?

---

## STEP 11 — Approve or refine

**If it's good:**
```
approved
```

The agent then:
1. Writes 5 personalized "Why This School" statements → saves to Drive
2. Creates 5 Gmail drafts with statement links → appear in your Gmail Drafts folder
3. Builds your College Tracker spreadsheet → saves to Drive
4. Loads all deadlines into Google Calendar with 2-week reminders
5. Sets follow-up check-ins for 2, 4, and 6 weeks from today

**If something's off:**
Tell it specifically what to fix — "more West Coast options," "drop schools over $30K," "the wildcard doesn't fit me." It regenerates and asks you to approve again.

---

## STEP 12 — Push your agent further

After setup, try:
- `Show me more schools in the same direction`
- `Show me schools like [School Name]`
- `What if I get a 1400 on my SAT?`
- `I don't like these — find me different ones`
- `Tell me more about [school]`
- `I want to explore trade school options instead`

The agent remembers everything. It doesn't need you to re-explain yourself.

---

## A note about the profile template

There's a detailed profile template in `02-workshop/profile-template.md`. You don't need it for the workshop — your agent asks questions directly in the chat.

The template is for when you come back later and want to give your agent more detail — specific clubs, service history, identity background for scholarship searches, location preferences, and more. The more you fill in, the more precise your results.

To use it later: fill it out, save it as a file, and upload it to your Project Knowledge. Your agent will detect it automatically next time and skip the questions.

---

## Stuck?

- **Agent not asking questions?** Make sure the system prompt is pasted into Custom Instructions and includes your first name.
- **Web search results look off?** Make sure Web Search toggle is ON.
- **Drive link not working?** Make sure workflow.md is in Project Knowledge.
- **Gmail drafts not appearing?** Check if Gmail connector was authorized in Step 3. If not, look for the emails in your Drive folder instead.
- **Anything else?** Raise your hand — your facilitator is in the room.

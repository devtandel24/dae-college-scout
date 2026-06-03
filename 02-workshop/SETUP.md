# SETUP — Build Your College Scout in 10 Steps

Total time: ~15 minutes to set up, ~5 minutes to run.

---

## What you need

- A laptop with a browser
- A Google account (you definitely already have one)
- The DAE-shared Claude account login your facilitator will give you
- This downloaded repo (you should already have it unzipped — if not, scroll up and grab it)

---

## STEP 1 — Log into Claude

Go to **claude.ai** and log in with the account credentials your facilitator handed out.

You'll share this account with 3-4 other students. That's fine — your work goes into your own project, which keeps it separate.

---

## STEP 2 — Create your project

In the left sidebar, find **"Projects"** and click the **+** to create a new one.

**Name it:** `[Your First Name]'s College Scout`

Example: `Marcus's College Scout`, `Maya's College Scout`

This is your private workspace. Everything you build lives here.

---

## STEP 3 — Open the profile template

In the repo folder you downloaded, open:

```
02-workshop/profile-template.md
```

Open it in any text editor (Notes app, Google Docs, Word, whatever).

---

## STEP 4 — Fill out your profile

**This is the most important part.** Your agent is only as good as your profile.

The profile has 9 sections. Fill them out **honestly**. The agent is private to you — be real.

Tips:
- **Skip what doesn't apply.** Not in sports? Skip Section 3a. Not in performing arts? Skip 3b.
- **Be specific.** "I like science" is weak. "I love biology and chemistry, hate physics" is gold.
- **Section 3d (Things You've Built) is huge.** If you code, run a side hustle, make videos, do art — write it all down. This is what makes your agent's recommendations specific.
- **No idea what you want to do? Say so.** "I have absolutely no idea" is a valid answer in Section 7 and 8. The agent will help you figure it out.

**Take ~10 minutes on this.** Don't rush.

---

## STEP 5 — Save your filled profile

Save your filled-out profile as a file. Any of these formats work:
- `.md` (markdown)
- `.txt` (plain text)
- `.pdf`
- `.docx` (Word)

Name it: `My_Profile.md` (or whatever extension)

---

## STEP 6 — Upload your profile to Project Knowledge

In your Claude project, find **"Project Knowledge"** (it's a section in the project sidebar).

Click **+ Add Knowledge** or drag your `My_Profile.md` file into it.

You should see your profile show up in the knowledge list.

**This is the agent's memory of you. It will read this every time you ask it to do anything.**

---

## STEP 7 — Upload the workflow file

In the repo folder, find:

```
02-workshop/workflow.md
```

Upload this file to your Project Knowledge too. (Same way as Step 6.)

**This is the agent's process — the step-by-step it follows when you ask it to scout.**

---

## STEP 8 — Set the system prompt

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

**This is the agent's personality, rules, and identity.**

---

## STEP 9 — Turn on Web Search

In the Claude chat interface, look for the **Web Search** toggle (usually a button below or beside the message box).

**Turn it ON.**

Your agent needs to be able to search the web to find real schools and scholarships.

---

## STEP 10 — Run your agent

In the chat, type exactly this:

```
Scout my schools
```

Hit enter.

**Watch your agent work.** You'll see it narrate what it's doing — searching, ranking, generating.

In about 1-2 minutes, your Scout Report will appear as a Canvas/Artifact on the right side of the screen.

---

## After the report drops

The agent will ask you if you want it to:
- Draft personalized emails to your top 5 schools
- Create a Google Drive folder with everything organized
- Add deadlines to your Google Calendar
- Set follow-up reminders

**Say yes** (or pick which ones).

If your facilitator has connected Gmail / Drive / Calendar to the account, the agent will do these things live. If not, the agent will create everything as files in the chat that you can save.

---

## Then — push your agent

Try follow-up questions like:
- `What about West Coast schools only?`
- `Show me cheaper options`
- `Find me 5 more scholarships specifically for [your specific thing]`
- `What would my application look like for my #1 school?`
- `Compare schools 1 and 3 — which is better for me?`

Watch how it remembers everything and re-runs with full context.

**That's what an agent is.** Memory. Tools. Process. Goal.

You just built one.

---

## Stuck?

- **Profile feels overwhelming?** Look at the sample personas in `../04-assets/sample-personas/` for inspiration. Don't copy them — use them as examples.
- **Agent gave a weird response?** Tell it specifically what was wrong. "That recommendation didn't reference my profile — try again with the schools that actually match my Section 3d projects."
- **Something broken?** Raise your hand. Your facilitator is in the room.

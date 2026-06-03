# College Scout Workflow

This is the step-by-step process the agent follows when triggered.

When the student says "Scout my schools" (or any trigger phrase from the system prompt), execute these steps in order. Narrate as you work.

---

## STEP 1 — LOAD PROFILE

Read the student's profile from Project Knowledge.

Confirm you have data on all 9 sections. If any are missing or unclear, ask the student to clarify before proceeding.

**Say:** "Got your profile, [Name]. Let me find your matches."

Add a one-line summary of who you think they are, based on the profile. Example: "Here's what I'm working with: strong builder profile, 3.6 GPA, real CS credentials, wants to leave the East Coast, needs merit aid."

---

## STEP 2 — GENERATE SEARCH STRATEGY

Based on the profile, generate 5-7 specific search queries.

Branch based on Section 7 (pathway choice). See system prompt for branching logic by pathway.

**Say:** "Running these searches: [briefly list them]"

---

## STEP 3 — RUN WEB SEARCHES

Execute each query. Read top results. Prioritize authoritative sources.

**Narrate:** "Found 14 candidates from College Scorecard..." "Cross-referencing program offerings..." "Checking scholarship databases now..."

---

## STEP 4 — CROSS-REFERENCE PROFILE

For each candidate, evaluate against:
- Academic fit (stats in range? reach/match/safety?)
- Vibe fit (matches their dream Friday night from Section 6?)
- Location fit (matches their distance preference?)
- Size fit (matches their size preference?)
- Cost fit (affordable given Section 5? scholarships available?)
- Program fit (has the major from Section 8?)
- Special considerations (HBCU/MSI? Religious? Disability services? Direct-admit?)

Drop any candidate that doesn't pass at least 4 of these.

---

## STEP 5 — FIND SCHOLARSHIPS

Find at least 3 real, currently-open scholarships this student qualifies for. Include name, amount, deadline (current cycle), link, and why this student specifically qualifies.

---

## STEP 6 — RANK

Pick top 4 best-fit + 1 wildcard.

Top 4: highest combined score across all fit dimensions.

Wildcard: something surprising but defensible — HBCU/MSI they didn't know about, honors program at a state school, direct-admit program, school in an unexpected region, community college pathway with strong transfer.

---

## STEP 7 — WRITE PERSONALIZED REASONING

For each of the 5 schools, write 3-4 sentences answering: "Why does this fit YOU?"

Hard rule: Must reference at least 2 specific things from this student's profile. If you can't, find a different school.

---

## STEP 8 — GENERATE THE HTML REPORT AND UPLOAD TO DRIVE

**This is the most important step. Read carefully.**

### 8a. Create the Drive folder

Create a Google Drive folder titled: `[Student First Name]'s College Scout`

### 8b. Generate the HTML report

Generate a complete, standalone HTML file with these sections in this order. The HTML must be visually rich, modern, and look like a real designed product — not a default-styled webpage.

#### Required sections:

**1. Hero header**
- Large, bold display heading with `[Student First Name]'s College Scout Report`
- Subtitle with date generated and one-line summary of the student
- Visually distinct — use a gradient, accent color, or hero image background

**2. Quick Snapshot card**
- 3-4 lines about who this student is, in the agent's honest voice
- Visually distinct card with accent color
- Example tone: "Marcus is a senior varsity basketball captain holding a 3.4 GPA. Needs significant financial aid. Wants to play in college without sacrificing real academics. Looking at D3 academic schools where he won't be the only Black kid in the room."

**3. Your Top 4 Matches**
- Section heading clearly distinct from snapshot
- Each school as its own card with:
  - School name + location (large)
  - Type tags (Public/Private, 4-year, religious affiliation if relevant) — visual chips
  - Annual cost grid: Sticker price | Net cost after typical aid | Cost for in-state if applicable
  - Acceptance rate, median test scores, student-to-faculty ratio (small stat grid)
  - Application deadline (regular + EA/ED) — visually prominent
  - **"Why this fits YOU" pull-quote** in larger accent color, personalized to this student
  - "One thing to verify before applying" callout

**4. Your Wildcard**
- Visually distinct — different background color or border treatment
- "🃏 Your Wildcard" heading with the school name
- Same card content as Top 4 PLUS an extra paragraph: "Why this surprised me as a fit for you"

**5. Comparison table**
- All 5 schools side-by-side
- Columns: School | Location | Cost (net) | Accept Rate | Best Fit For You | Deadline
- Use color or icons to highlight strengths

**6. Scholarships You Personally Qualify For**
- Section with at least 3 scholarship cards
- Each with: scholarship name, sponsoring org, amount (visually prominent), deadline (with urgency indicator if soon), link, "why you qualify" sentence

**7. What I'd Do Next (Next 7 Days)**
- 3 numbered action items, tailored to grade level and pathway
- Each with specific dates or names

**8. Reality Check**
- Honest assessment in a different visual treatment
- Reach/match/safety breakdown of the 4 picks
- One real strength to lean into
- One gap to address
- One thing not to worry about

**9. Footer**
- "Built by your College Scout · Generated [date]"
- Small DAE attribution

#### Technical requirements:

- **Standalone HTML** — all CSS inline in `<style>` tags, no external dependencies (except optionally Google Fonts via `<link>`)
- **Mobile responsive** — use flexbox/grid, max-width containers, media queries for under 768px
- **Modern CSS** — use gradients, soft shadows (`box-shadow: 0 4px 20px rgba(0,0,0,0.08)`), rounded corners (`border-radius: 16px`), generous whitespace (`padding: 32px+`)
- **Typography** — use Google Fonts import (e.g., `Inter` for body, `Outfit` or `Space Grotesk` for headings), or system font stack
- **Color palette** — pick a sophisticated palette, NOT default blue. Examples that work:
  - Warm: deep terracotta + cream + forest accent
  - Cool: midnight navy + soft coral + pale gold
  - Modern: charcoal + electric lime + off-white
  - Bold: deep purple + bright orange + cream
- **No clip art, no stock images.** Use emoji as visual anchors sparingly (🎓 🃏 ✨ 📍)
- **File name:** `[Student First Name]_College_Scout_Report.html`

### 8c. Upload to Drive

Upload the HTML file to the Drive folder created in 8a. Get the shareable link.

### 8d. Verify it opens correctly

If possible, fetch the file back to confirm it uploaded properly.

---

## STEP 9 — DELIVER LINK + APPROVAL ASK (the chat response)

**Keep this chat response short.** Do NOT include the report content in chat.

Send a message like:

> "Your report is ready, [Name]. **[Drive link]**
>
> Open the link — the HTML renders right in your browser. Quick spoiler: your wildcard is **[School Name]** and I think it might be the most interesting pick because [one specific reason]. Also worth flagging: [one specific scholarship finding or unexpected match].
>
> Read it. When you're ready, come back here and say **'approved'** to kick off the next steps — emails, calendar, tracker. Or tell me what to fix if anything's off."

**Stop. Wait for the student.**

---

## STEP 10 — APPROVAL GATE

The student must come back and explicitly approve before you do anything else.

**If approved** ("approved" / "yes" / "thumbs up" / "go" / "let's do it"):
→ Proceed to Step 11

**If feedback** ("change X" / "redo Y" / "more West Coast options" / etc.):
→ Adjust criteria, re-run Steps 4-9 (skip the search if it's a ranking adjustment, re-search if it's a criteria change)
→ Regenerate the HTML report, replace it in Drive (same folder), get the new link
→ Send the new link with a note about what changed: "Updated based on your feedback — added more West Coast options, swapped out [School X] for [School Y]. New link: [link]. Say 'approved' when ready."

**If unclear**:
→ Ask one clarifying question. Don't proceed.

---

## STEP 11 — EXECUTE AGENTIC ACTIONS (only after approval)

### 11a. Check Gmail connector

Try to access the Gmail connector.

**If Gmail is connected and authorized for sending:**

Say to the student:
> "Quick confirm: I'm about to send 5 emails FROM **[connected gmail address]** to the admissions offices at your top 5 schools. Each email is personalized, ~4-5 sentences, requesting an info packet and showing interest. Confirm by saying **'send them'** to send live. Or say **'just draft them'** and I'll save the drafts to your Drive folder for you to send from your own Gmail later."

Wait for response.

- "send them" → Send all 5 emails via Gmail connector. Confirm each send.
- "just draft them" → Save as a Google Doc in the Drive folder (see 11b format)
- Anything else → Ask for clarity

**If Gmail is NOT connected (or send fails):**

Say:
> "I can't send emails directly — Gmail isn't authorized on this account for sending. I'll do the next-best thing: save 5 pre-drafted personalized emails to your Drive folder. Open Gmail, copy each one, paste, hit send. Takes you 3 minutes total."

Save as draft doc (see 11b).

### 11b. Format the email drafts doc (if drafting)

Create a Google Doc in the Drive folder titled `Emails to Send to My Top 5 Schools`.

At the top, in bold:
> *Instructions: Below are 5 personalized emails to your top 5 schools. Open your own Gmail, copy each email, paste into a new message, send. Total time: ~3 minutes. Responses come back to YOUR inbox.*

For each school:
- **To:** [official admissions email — researched and verified]
- **Subject:** Prospective Student — [Student Name] — Class of [Year]
- **Body:** 4-5 sentence email referencing:
  - Why they're interested in THIS school specifically (from the personalized reasoning)
  - One thing about them that's relevant (from profile)
  - A specific question or request (info packet, virtual tour link, contact with current student in their major, campus visit options)
  - Sign-off with their name, school, graduation year

Separator between each email.

### 11c. Create the College Tracker spreadsheet

Create a Google Sheet in the Drive folder titled `[Student First Name]'s College Tracker`.

Columns:
| School | Status | App Deadline | Decision Date | Financial Aid Deadline | App Fee | Notes |

Status options dropdown: Interested / Researching / Application Started / Submitted / Accepted / Waitlisted / Rejected

Pre-fill all 5 rows with researched deadlines, fees, and a starting note for each.

### 11d. Load Google Calendar

For each of the 5 schools:
- `[School Name] Application Due` on deadline date — include link to school's application page in description
- `[School Name] Decision Date` on decision date
- `[School Name] Financial Aid Deadline` on FA deadline

For each scholarship:
- `[Scholarship Name] Deadline` on deadline date

**Set 2-week-prior reminder for each event.**

### 11e. Set follow-up reminders

- 2 weeks from today: `Check in with College Scout — any school responses?`
- 4 weeks from today: `College Scout follow-up #2 — anything need attention?`

### 11f. Send final confirmation in chat

Short and clean:

> "Done. Here's what's live:
>
> 📁 **Drive folder:** [link] — your HTML report, your tracker, your emails (sent or drafted)
> ✉️ **Gmail:** [5 emails sent FROM your-gmail@gmail.com / 5 emails drafted in your folder]
> 📅 **Calendar:** all deadlines loaded, reminders set 2 weeks before each
> 🔔 **Follow-ups:** I'll nudge you on [date 2 weeks out] and [date 4 weeks out]
>
> Come back here anytime — your profile and everything we built is saved. Update me when you hear from schools, or when something changes."

---

## STEP 12 — HANDLE FOLLOW-UPS (post-workshop)

If the student returns later with questions, use the same project memory:

- "What about [different criteria]?" → Re-run from Step 2 with adjusted criteria, regenerate HTML report
- "Tell me more about [school]" → Deep dive via web search, save as new doc in Drive folder
- "Help me write my essay for [school]" → Draft starting essay based on profile + school values
- "What if my SAT goes up to X?" → Re-evaluate matches with new score
- "School X responded — what do I do?" → Help draft response, update tracker

Always reference original profile. Never ask them to re-explain themselves.

---

## END OF WORKFLOW

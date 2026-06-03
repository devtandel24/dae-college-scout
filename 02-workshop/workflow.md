# College Scout Workflow

This is the step-by-step process the agent follows when triggered.

When the student says "Scout my schools" (or any trigger phrase from the system prompt), execute these steps in order. Narrate as you work.

---

## STEP 1 — LOAD PROFILE

Read the student's profile from Project Knowledge.

Confirm you have data on:
- Section 1: Name, grade, school, GPA, test scores
- Section 2: Academic rigor, subject preferences
- Section 3: Activities (sports, arts, **things they've built**, clubs, work, service)
- Section 4: Identity background (handle gently)
- Section 5: Financial reality
- Section 6: Vibe & location preferences
- Section 7: **Pathway choice** ← this determines everything that follows
- Section 8: Career direction
- Section 9: Real talk (what they want a school to know, worries)

If any section is missing or unclear, ask the student to clarify before proceeding.

**Say:** "Got your profile, [Name]. Let me find your matches."

---

## STEP 2 — GENERATE SEARCH STRATEGY

Based on the profile, generate 5-7 specific search queries.

**For 4-year college pathway:** Mix queries like:
- "Colleges with strong [their intended major or interest] under [their budget] in [their region]"
- "[Honors programs at state schools] for [their GPA range]"
- "Direct admit programs for [their intended major]"
- "[Their sport] recruiting opportunities at [appropriate division] schools"
- "Scholarships for [their specific demographic + activity]"

**For trade school pathway:**
- "[Their trade interest] apprenticeship programs in [their state]"
- "Accredited trade schools for [trade] near [their city]"
- "Union apprenticeships [trade] [state]"
- "Trade school cost vs job placement rate [trade]"

**For military pathway:**
- Service academy admissions requirements
- ROTC scholarship programs [their state/intended major]
- Military enlistment paths for [their interest]
- MOS/job specialties matching [their skills]

**For gap year pathway:**
- AmeriCorps programs matching [their interests]
- Structured gap year programs [domestic/international]
- City Year, NOLS, Outward Bound

**For "no idea" pathway:**
- Run multiple searches across at least 3 different pathways
- Use their profile signals (academic strength, interests, projects) to guess what might resonate
- Return 1-2 options per pathway with reasoning

**Say:** "Running these searches: [briefly list them]"

---

## STEP 3 — RUN WEB SEARCHES

Execute each query. Read top results carefully.

Priority order for sources:
1. **.gov sites** — College Scorecard, CareerOneStop, military, AmeriCorps
2. **College Board's BigFuture**
3. **Official school admissions pages**
4. **Niche.com** (for student-rated experience data)
5. **Fastweb, Scholarships.com, Bold.org, Going Merry, RaiseMe** (scholarships)

**Narrate as you go:**
- "Found 14 candidates from College Scorecard..."
- "Cross-referencing with their actual program offerings..."
- "Checking scholarship databases for ones you'd qualify for..."

---

## STEP 4 — CROSS-REFERENCE PROFILE

For each candidate, evaluate against:

- **Academic fit:** Are this student's stats in range? Reach/match/safety?
- **Vibe fit:** Does it match their dream Friday night from Section 6?
- **Location fit:** Does it match their distance preference?
- **Size fit:** Does it match their preferred student body size?
- **Cost fit:** Is it affordable given Section 5? Are scholarships available?
- **Program fit:** Does it have the major(s) from Section 8?
- **Special considerations:** Do they need HBCU/MSI? Religious affiliation? Disability services? Specific direct-admit program?

Drop any candidate that doesn't pass at least 4 of these.

---

## STEP 5 — FIND SCHOLARSHIPS

Search specifically for scholarships THIS student qualifies for based on profile.

Categories to check:
- **Need-based:** FAFSA eligibility, Pell Grant, state grants
- **Merit-based:** GPA, test score, course rigor
- **Identity-based:** First-gen, underrepresented background, specific heritage, LGBTQ+, military family, religious affiliation
- **Activity-based:** Specific sport, art, service, leadership
- **Geographic:** State residency, community foundations, local rotary clubs
- **Field-specific:** Intended major, intended industry

Find **at least 3 real, currently-open scholarships**. Include:
- Scholarship name
- Amount
- Deadline (must be current cycle)
- Link to apply
- Why this student qualifies specifically

---

## STEP 6 — RANK

Pick **top 4 best-fit + 1 wildcard**.

**Top 4:** Highest combined score across academic/vibe/location/cost/program fit.

**Wildcard:** Something they probably haven't considered but that fits surprisingly well. Examples:
- An HBCU/MSI they didn't know about
- An honors program at a state school
- A direct-admit program
- A small liberal arts college with unusual strength in their field
- A school in a region they haven't considered
- A community college pathway with strong transfer to their dream 4-year

Don't make the wildcard weird. Make it interesting and defensible.

---

## STEP 7 — WRITE PERSONALIZED REASONING

For each of the 5 schools/programs, write 3-4 sentences answering: **"Why does this fit YOU?"**

**Hard rule:** Must reference at least 2 specific things from this student's profile.

Good examples:
- "Given that you've built three apps and run an Etsy shop on the side, [School]'s entrepreneurship-meets-CS pathway is rare — they let you take CS courses without locking in CS as a major, which fits the way you described wanting to keep options open."
- "You said you want a real winter and city energy but cost matters — [School] is in [city] with in-state tuition at $X, and they have one of the strongest [your intended major] programs in the country with a 94% placement rate."

If you can't find 2 personalization hooks, the school doesn't make the list. Find a different one.

---

## STEP 8 — GENERATE THE REPORT

Create a Canvas/Artifact titled `[Student Name]'s College Scout Report`.

### Required sections (in this order):

**1. Quick Snapshot** (3 lines)  
A summary of this student in the agent's honest voice. Example: "Marcus is a senior who's been varsity basketball captain for two years, holds a 3.4 GPA, and wants to keep playing in college without sacrificing academics. Family budget is real — needs aid. Wants to study business or sports management."

**2. Your Top 4 Matches**  
For each:
- School name + location
- Type (Public/Private, 4-year/2-year, religious affiliation if relevant)
- Annual cost (in-state if applicable, out-of-state, and net cost after typical aid)
- Acceptance rate
- Application deadline (regular + early action/decision if available)
- Key stats (median SAT/ACT if relevant, student-to-faculty ratio)
- **"Why this fits YOU"** paragraph (3-4 sentences, personalized)
- One thing to verify before applying

**3. Your Wildcard**  
The surprise pick. Same format as Top 4, plus an extra paragraph explaining why it's interesting and worth a serious look.

**4. Scholarships You Personally Qualify For**  
At least 3 scholarships with:
- Name + sponsoring org
- Amount
- Deadline
- Link
- Why you specifically qualify

**5. What I'd Do Next** (3 specific actions for the next 7 days)  
Tailored to their grade level and pathway. Examples:
- "Take the SAT by [date] — your profile says you haven't yet, and 3 of these schools are still test-required"
- "Email [Teacher Name] about a rec letter — your AP English grade suggests they could write you a strong one"
- "Apply to [Scholarship] by [date] — deadline is in 12 days"

**6. Reality Check**  
Honest assessment:
- Reach/match/safety breakdown of your 4 picks
- Anything in their profile that's a real strength they should lean into
- Anything that's a gap they should address
- One thing they shouldn't worry about even though their profile suggests they might

Make it visually clean. The student should want to screenshot this.

---

## STEP 9 — OFFER THE AGENTIC EXTRAS

After the report, ask:

> "Want me to actually do something with this? I can:
> 
> ✅ Draft personalized emails to each of these 5 schools requesting info packets and showing interest (you'll send them from your own Gmail — takes you 3 minutes after this)
> 
> ✅ Create a Google Drive folder with your full Scout Report and a tracker spreadsheet
> 
> ✅ Add application deadlines to your Google Calendar with reminders 2 weeks before each one
> 
> ✅ Set a follow-up reminder for 2 weeks from today (and 4 weeks) to check if schools responded
> 
> Say 'yes do it all' or pick which ones."

**Wait for their approval.** This is the human-in-the-loop checkpoint.

---

## STEP 10 — EXECUTE THE AGENTIC ACTIONS

Once the student approves, execute the actions they approved.

### A. Create the Drive folder

Folder name: `[Student Name]'s College Scout`

Inside:
- **Scout Report** (the full report as a PDF or Google Doc)
- **Emails to Send to My Top 5 Schools** (Google Doc — see format below)
- **College Tracker** (Google Sheet — see columns below)

### B. The emails Google Doc format

At the top, instructions in bold:
> *"Below are 5 pre-drafted emails to your top schools. Open your own Gmail, copy each one, paste into a new message, hit send. Takes ~3 minutes. Responses will come back to your inbox."*

For each of the 5 schools:
- **School:** [Name]
- **Send to:** [official admissions email — research and verify]
- **Subject line:** Prospective Student — [Their Name] — Class of [Year]
- **Email body:** Personalized 4-5 sentence email referencing:
  - Why they're interested in THIS school specifically (from the Scout Report reasoning)
  - One thing about them that's relevant (from their profile)
  - A specific question (info packet, virtual tour, contact with current student in their major)
  - Sign-off with their name, school, grad year

### C. The College Tracker spreadsheet

Columns:
| School | Status | App Deadline | Decision Date | Financial Aid Deadline | Application Fee | Notes |
|---|---|---|---|---|---|---|

Status options: Interested / Researching / Application Started / Submitted / Accepted / Waitlisted / Rejected

Pre-fill rows for all 5 schools with deadlines and fees you researched.

### D. Add to Google Calendar

For each of the 5 schools:
- Event: "[School Name] Application Due" on the deadline date, with the school's application page URL in the description
- Event: "[School Name] Decision Date" on the decision date
- Event: "[School Name] Financial Aid Deadline" on the aid deadline

For each scholarship:
- Event: "[Scholarship Name] Deadline" on the deadline date

**Set a reminder 2 weeks before each event.**

### E. Set follow-up reminders

- Event 2 weeks from today: "Check in with College Scout — any school responses?"
- Event 4 weeks from today: "College Scout follow-up #2 — anything need attention?"

### F. Confirm with the student

Say something like:

> "Done. Your Drive folder is live: [link if available]. Your calendar has all the deadlines loaded with reminders 2 weeks before each one. I've set check-ins for 2 weeks and 4 weeks from today.
> 
> When you're ready to follow up with any school, come back to this project and tell me what's happening. I'll remember everything."

---

## STEP 11 — HANDLE FOLLOW-UPS

When the student asks follow-up questions, use the same project memory. Never start from scratch.

Common follow-ups:
- **"What about [different criteria]?"** → Re-run the workflow from Step 2 with adjusted criteria
- **"Tell me more about [school]"** → Deep dive on that school using web search
- **"Help me write my essay for [school]"** → Draft a starting essay based on their profile + that school's values
- **"What if I improve my SAT by [points]?"** → Re-evaluate which matches become reach/match/safety
- **"Compare schools [X] and [Y]"** → Head-to-head comparison referencing their profile priorities

Always reference their original profile. Don't ask them to re-explain themselves.

---

## END OF WORKFLOW

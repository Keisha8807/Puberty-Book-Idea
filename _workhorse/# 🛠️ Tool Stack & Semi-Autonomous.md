# 🛠️ Tool Stack & Semi-Autonomous Operating Plan

> **For:** Keisha · **Written:** August 20, 2026
> **Question this answers:** "What are all these AI tools, and can one of them run my whole book business so I'm not chained to the PC?"
> **Short answer:** No single tool does all of it. A *small combo* does about 80% of it, and the part that makes it work isn't the tool — it's the folder system you already started in `_workhorse/`.

---

## Part 1 — Decoder ring: what each of these things actually is

The single most useful idea: **models, surfaces, and add-ons are three different layers.** People mix them up constantly.

| Layer | What it means | Examples |
|---|---|---|
| **Model** | The brain. Raw intelligence. You don't "use" it directly — it powers a surface. | Claude Fable 5, Opus 5, Sonnet 5 · GPT-5.6 |
| **Surface** | The room you talk to the brain in. Determines what it can *touch* — files? browser? just chat? | Claude chat, Claude Desktop/Cowork, Claude in Chrome, ChatGPT Chat/Work/Codex |
| **Add-on** | Extra reach or reusable know-how bolted onto a surface. | Skills, plugins, connectors, scheduled tasks |

### The models
- **Claude Fable 5** — released June 9, 2026; Anthropic's top-tier "Mythos-class" model, 1M-token context, built for *long-running agent work*. This is a **brain, not an app.** You get it by choosing it inside a Claude surface. Big context = it can hold your whole series bible + 15 chapters + brand voice at once without forgetting. (Siblings: **Sonnet 5** = fast daily driver, June 30 2026; **Opus 5** = heavy reasoning, July 24 2026.)
- **GPT-5.6** — the equivalent brain behind ChatGPT Work.

### The Claude surfaces
- **Claude Desktop** — the app on your computer. The container that holds chat + Cowork.
- **Claude Cowork** — *the big one for you.* Launched Jan 12, 2026. Described as "Claude Code for the rest of your work." You point it at **one folder** on your machine; it reads, edits, creates, renames, and organizes files inside that folder, works through a multi-step plan on its own, and reports back. Built for non-coders — no terminal. Started as a macOS research preview for Max subscribers ($100–200/mo tier); check current availability for your plan/OS.
- **Claude Code** — same engine, but a terminal tool built for programmers. **You do not need this.** Cowork is Claude Code with the scary parts removed.
- **Claude in Chrome** — browser extension. Reads the page you're on, clicks, types, fills forms, downloads — inside *your* logged-in browser session. As of Aug 13, 2026, a full Cowork session runs inside the Chrome side panel, so skills/plugins/connectors work in the browser too. Pattern: Chrome does the research, Cowork turns it into files.

### The OpenAI surfaces
- **ChatGPT Chat** — what you're used to. Ask, get an answer.
- **ChatGPT Work** — launched July 9, 2026. Give it an *outcome*; it gathers context from connected apps, plans, and works for hours, returning **finished artifacts** — spreadsheets, slide decks, documents, shareable web apps. Has **Plan mode** (it proposes a step-by-step plan you approve before it starts) and approval checkpoints. 1,400+ plugins.
- **Codex** — the coding one. Merged into the same ChatGPT desktop app. **Not for you** — except that "automations" (scheduled agent runs) came from it.
- **Scheduled Tasks** — relaunched June 17, 2026. Runs a prompt on a clock (max ~once/hour; 5 active on Plus, 15 on Pro). ⚠️ Important limit: it mostly **notifies you** rather than doing the work. Great for "watch this and tell me," weak as an execution engine.

### The add-ons (this is where the leverage is)
- **Skills** — a reusable folder of instructions + examples that teaches the AI *your* way of doing a recurring job. Write "how a Mia chapter is structured" once as a skill, and every future chapter draft follows it without you re-explaining. **You already have one of these in your repo** (`book-creative-development.skill` on `main`) — you were doing this before you had the vocabulary for it.
- **Plugins / connectors** — pipes to outside services (Drive, Slack, Notion, Gmail, Canva, etc.).
- **Projects** — a persistent container holding files + standing instructions so context survives between sessions.

---

## Part 2 — What "semi-autonomous" honestly means in 2026

Be clear-eyed, because the marketing isn't:

**What it genuinely does now**
- Runs for *hours* on a multi-step job without hand-holding, and hands you finished files.
- Holds your whole canon in context so outputs stay on-brand.
- Works while you're away from the desk — you review on your phone later.
- Repeats a defined process forever without getting bored or drifting.

**What it does NOT do**
- ❌ Run your business unattended for a week. Agent runs are *bounded sessions*, not employees.
- ❌ Auto-post to social platforms. Automated posting violates most platforms' terms; use a real scheduler (Buffer, Metricool, Later) and let the AI fill the queue.
- ❌ Make taste calls. Which cover, which title, which price — that's you.
- ❌ Produce consistent character illustrations by itself. Character consistency across 100+ images is still the hardest unsolved piece. (You've already felt this — it's why `art-v2/` has approved hero images and model boards. That approach — lock a reference sheet, then generate everything *from* it — is the correct workaround.)
- ❌ Spend money or sign things.

**The mental shift:** stop thinking "AI writes my book." Start thinking **"I run a small studio of interns who work fast, never sleep, have no taste, and forget everything unless it's written in a file."** Your job changes from *doing* to *directing + approving*. That's the job that isn't chained to a PC — you can approve from your phone.

---

## Part 3 — Why your `_workhorse/` folder is the actual secret weapon

The thing that separates "I chat with AI" from "AI works for me" is **a written, external memory that every session reads first.** You already built it:

- `01-rules/ACTIVE-CANON.md` — the truth. Names, ages, timeline, voice, what's locked.
- `01-rules/SOURCE-HIERARCHY.md` — which file wins when two disagree.
- `01-rules/SAFETY-AND-APPROVALS.md` — what the AI may never do without you.
- `00-command-center/CURRENT-STATE.md` — where the project stands today.
- `00-command-center/DECISION-LOG.md` — why things are the way they are, so nobody re-litigates.
- `00-command-center/APPROVAL-QUEUE.md` — what's waiting on your yes/no.
- `02-inbox/` — raw new material awaiting review.
- `03-templates/WORK-REQUEST.md` — the standard way to hand off a job.

**That is exactly the architecture professional AI teams use.** Point Cowork at this repo folder and it wakes up already knowing your world — no re-explaining, no copy-paste, no drift. Every hour you spend improving these files multiplies every future run.

The loop:
```
Voice note / idea  →  02-inbox/
        ↓
Agent run (reads canon → drafts → writes files)
        ↓
APPROVAL-QUEUE.md  →  you review on your phone
        ↓
Approved → filed into the project folder + logged in DECISION-LOG.md
```

---

## Part 4 — The recommended stack (a combo, not one tool)

| Job | Tool | Why |
|---|---|---|
| **Studio HQ** — manuscripts, series bible, canon, filing, long drafting | **Claude Cowork** (Desktop, pointed at this repo) + **Fable 5** | Works directly in your files; 1M context holds the whole vault; built for long autonomous runs |
| **Research & decks/sheets** — market research, comp titles, KDP/TPT/Etsy pricing, launch calendars, pitch decks | **ChatGPT Work** | Returns finished spreadsheets/slides; Plan mode keeps you in control |
| **Live web work** — pulling analytics, filling listing forms, competitor pages | **Claude in Chrome** | Acts inside your logged-in session; Cowork panel converts findings into files |
| **Music** | **Suno** (you have it) + AI-written lyrics/style prompts | Your 25 songs are already drafted in `01-mia-puberty-book/marketing/songs/` |
| **Illustrations** | Image model of choice, driven by locked reference sheets in `characters/art-v2/` | Consistency comes from the reference sheets, not the model |
| **Video trailers (30–45s)** | AI writes shot lists + image/video prompts + captions + score brief; you assemble in CapCut, or use a video model | Your `marketing/trailers/` folder already holds concepts and 7–11 second clip plans |
| **Posting** | Buffer / Metricool / Later — AI fills the queue, scheduler publishes | Never auto-post via browser agent |
| **Recurring nudges** | ChatGPT Scheduled Tasks | Weekly "what's in the approval queue," trend checks |
| **Version history / mobile review** | GitHub (already set up) | Every change tracked; review from your phone |

**If you only pick one to start: Claude Cowork.** Your entire operation is already files in a folder, which is precisely what it's designed for.

---

## Part 5 — Can it do "the whole package"? Honest scorecard

| Deliverable | How much AI can carry | Your part |
|---|---|---|
| Series writing (drafts, outlines, continuity) | 🟢 85% | Voice, heart, final line edit — a mom's judgment on what a 10-year-old actually needs to hear |
| Marketing plan + social campaigns | 🟢 85% | Approve angle, brand voice |
| Email campaigns / welcome sequences | 🟢 85% | Send button, list platform |
| Trailer scripts, shot lists, prompts, captions | 🟢 80% | Assembly + taste |
| Songs | 🟢 80% (lyrics/style) | Suno generation, picking takes |
| Sales/launch plan, pricing, KDP/TPT/Etsy listings | 🟡 70% | Money decisions, account setup |
| Market/audience research | 🟢 85% | Verify claims — AI gets facts wrong |
| Illustrations & book interior | 🟡 50% | Heavy art direction; consider hiring an illustrator for the final book |
| Building an audience from zero | 🔴 30% | Showing up as a human. Nobody follows a bot. **This is the real bottleneck — not content production.** |

**The blunt truth about "no audience, self-publishing from scratch":** AI removes the *production* bottleneck entirely — you can have 200 pieces of content by Friday. It does not remove the *trust* bottleneck. Your unfair advantage isn't AI output, it's that you're a mom solving a problem you actually live. Put your face and story in front of parents; let the AI carry everything behind it.

---

## Part 6 — A realistic 30-day ramp

**Week 1 — Foundation (no new tools).** Get `ACTIVE-CANON.md` genuinely accurate. Write one paragraph of "brand voice" and one "who this is for." Everything downstream inherits from these.

**Week 2 — One agent, one folder.** Set up Claude Cowork (or ChatGPT Work with this folder uploaded) pointed at the repo. Give it exactly one bounded job: *"Read the canon and the Book 1 outline. Draft chapter 3. Put it in `02-inbox/`. Add an entry to `APPROVAL-QUEUE.md`. Change nothing else."* Learn the rhythm of request → review → approve.

**Week 3 — Turn repeat jobs into skills.** After you've corrected the same thing three times, write it down as a skill: `chapter-drafting`, `trailer-script`, `social-post-pack`. Now quality holds without you repeating yourself.

**Week 4 — Add the second seat + the schedule.** ChatGPT Work for research/spreadsheets/decks. One Scheduled Task: Monday morning "summarize the approval queue and what's blocked." Then a standing weekly production run.

**Then the weekly cadence that gets you off the PC:**
- **Monday (30 min, desk):** approve the week's plan.
- **Tue–Thu (phone):** voice-note ideas into the inbox; agents run; you approve in spare moments.
- **Friday (1 hr, desk):** review the week's artifacts, schedule the social queue, log decisions.

---

## Part 7 — Guardrails (put these in `SAFETY-AND-APPROVALS.md`)

1. **The agent works in one folder.** Never point it at your whole drive.
2. **Nothing goes public without your explicit yes** — no posting, no publishing, no emailing a list.
3. **Nothing gets deleted, only moved** to `99-superseded/`. Vague instructions are how agents delete things.
4. **Everything is in Git.** Any mistake is recoverable — this is why your GitHub setup matters more than it looks.
5. **Verify every factual claim** in puberty/health content against a real medical source. AI confidently invents facts, and this is a book for children.
6. **Approvals happen in writing** in `APPROVAL-QUEUE.md`, so decisions survive the session.

---

## The one-line version

> Claude **Fable 5** is a brain; **Cowork** is the room where it can touch your files; **ChatGPT Work** is a second room that produces decks and spreadsheets; **Chrome** is its hands on the web; **Codex** isn't for you. Use Cowork as HQ, ChatGPT Work as research/ops, Suno for music, a scheduler for posting — and let `_workhorse/` be the shared brain all of them read first.


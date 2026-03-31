## A Claude Skill for Product Designers

A Claude skill that transforms raw project notes, accomplishment bullets, or brief descriptions into **senior-level portfolio case studies** in Markdown.

Built for product designers who know what they did — but struggle to articulate *why* they made the decisions they did. That gap is exactly what hiring managers probe for in senior designer interviews.

---

## The Problem This Solves

Most designer portfolios describe output. Senior roles require evidence of judgment.

| What designers write | What hiring managers want to see |
|---|---|
| "Conducted usability testing with 24 participants" | "Chose moderated over unmoderated testing because we needed to understand *why* fans hesitated, not just where they failed" |
| "Designed a WYSIWYG editor" | "Chose WYSIWYG over form-based config because client mental models mapped to 'editing a page', not 'filling out settings'" |
| "Created cross-team documentation" | "Documented the *why* behind each pattern so teams could handle edge cases without coming back to me" |

This skill surfaces the decision layer that turns a deliverable list into a leadership story.

---

## What It Generates

Each case study includes 8 structured sections:

1. **Header** — Role, timeline, team, platform
2. **One-Line Impact** — A hook that leads with outcome, not action
3. **Context & Problem** — Business stakes + design problem framed as discovery
4. **Role & Constraints** — What you owned, what made it hard
5. **Design Decisions** — The core section: each major decision with alternatives considered, tradeoffs made, and how it was validated
6. **Process Narrative** — A story, not a checklist — including direction changes and honest moments
7. **Outcome & Impact** — Three tiers: user, business, and org/team impact + "What I'd do differently"
8. **Image Placeholders** — Labelled slots for screenshots and artifacts throughout

---

## Installation

1. Download [`case-study-generator.skill`](./case-study-generator.skill)
2. Go to **Claude.ai → Settings → Skills**
3. Click **Install from file** and upload the `.skill` file

That's it. The skill is now available in your Claude projects.

---

## How to Use It

Once installed, just describe your project to Claude in natural language:

**From raw bullets:**
> "Write a case study for my Flex Plans redesign project. Here are my notes: [paste accomplishment bullets]"

**From a brief description:**
> "Turn this into a case study: I redesigned the checkout flow for a B2B SaaS platform. We had 4 months, I was the sole designer, and we improved task completion by 35%."

**In rewrite mode:**
> "Here's my existing case study draft. It's too listy and doesn't explain my decisions well — help me rewrite it."

**When you're not sure where to start:**
> "Help me write a case study for [project name]"

The skill will ask you three targeted questions before writing if your input is sparse — designed to surface the decision-making layer you might have forgotten to mention.

---

## Example Output Structure

```markdown
# Mobile Checkout Redesign
**Role:** Product Designer (lead designer, 2-person team)
**Timeline:** Q1 2024 (~3 months)
**Platform:** iOS & Android (e-commerce)

> Redesigned the end-to-end mobile checkout flow for a mid-market
> e-commerce platform — reducing drop-off by 28% by replacing a
> 6-step linear flow with a progressive disclosure model. Validated
> through unmoderated usability testing with 32 participants across
> two competing interaction patterns.

## Design Decisions

**Decision: Use progressive disclosure over a step-by-step wizard —
rather than reducing the number of steps**

Why I chose this over alternatives: The team's initial assumption was
that the drop-off was caused by too many steps. I wasn't convinced.
Session recordings pointed to users abandoning when asked for payment
details before seeing a final order summary — a trust problem, not a
length problem. Progressive disclosure let users commit incrementally...

What I had to give up: Progressive disclosure required tighter
coordination with engineering to handle partial state saves.
That added two weeks to the build...

How I validated it: Unmoderated testing via Maze with 32 participants
across both prototypes. The progressive model showed a 34% higher
task completion rate and significantly lower perceived effort scores...
```

---

## Who This Is For

- **Product designers targeting senior roles** — build the case for your judgment, not just your output
- **Senior designers targeting staff or principal** — reframe your work around org-level influence and systems thinking
- **Designers returning from a career break** — document older projects before the details fade
- **Design managers** — help your reports build stronger portfolio narratives during performance cycles

---

## Seniority Calibration

The skill automatically adjusts its framing based on your target level:

| Target Level | Story Emphasis |
|---|---|
| Mid → Senior | Ownership, decision-making, handling ambiguity |
| Senior → Staff/Principal | Org-level influence, cross-team impact, systems thinking |
| IC → Design Leadership | People, process, vision — multiplying team output |

---

## Tips for Best Results

- **Give it messy input** — the skill is designed to work with raw notes, not polished writing. The messier your input, the more transformation it can do.
- **Answer the probing questions** — if Claude asks "what's one decision a less experienced designer might not have made?", take 2 minutes to answer it. That answer is the heart of your case study.
- **Don't sanitize the "What I'd do differently"** — the most memorable case studies include honest reflection. Generic answers ("I'd do more research") are worse than nothing.
- **Use the image placeholders as a capture list** — every `[IMAGE: ...]` placeholder is a screenshot you need to pull from Figma or Miro. Treat it as your asset checklist.

---

## Contributing

Found a way to make the case studies stronger? Improvements welcome.

- **Better probing questions** — what questions surface better decision rationale?
- **New seniority tiers** — freelance, agency, in-house variations?
- **Format variants** — slide deck format, PDF-ready format, interview prep version?

Open a PR or start a discussion.

---

## About

Built by [Milan Gautam](https://in.linkedin.com/in/milangautam) — Product Designer at Ticketmaster, 8+ years in enterprise SaaS.

This skill was created as part of a personal system for documenting design work at scale. The case study structure is based on what actually moves hiring managers in senior design interviews — not portfolio trends.

---

*Compatible with Claude.ai (Pro, Team, and Enterprise plans). Requires Skills feature enabled.*

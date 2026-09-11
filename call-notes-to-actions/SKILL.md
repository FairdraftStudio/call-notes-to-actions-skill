---
name: call-notes-to-actions
description: Turns a meeting transcript, call recording notes, or rough meeting notes into a crisp summary with decisions, an action-item table (owner, action, due date), open questions, risks, and a ready-to-send follow-up email. Use when someone asks to summarize a call or meeting, extract action items, write meeting minutes, or draft a follow-up email after a client call.
---

# Call Notes → Actions

Nobody remembers what was agreed on a call. This makes it explicit in two minutes.

## 1. Gather inputs

**Required**: a transcript, notes, or a description of the call.

**Helpful**: meeting date, participants and their roles, which side the user is on (e.g. freelancer vs. client).

Do not ask questions before the first draft. Put unknowns in "To confirm".

## 2. Rules

- **Only extract what was actually said.** Do not invent decisions, owners, or dates.
- If an owner or due date is implied but not stated, fill it in and mark it **(proposed)**.
- Turn vague intentions ("we should look into…", "let's think about…") into action items with owner **TBD** so they don't get lost.
- A **decision** is something agreed; a **question** is something still open. Don't mix them.
- Merge duplicates. Use participants' real names as they appear.
- Relative dates ("next Friday") become real dates computed from the meeting date, or from today if the meeting date is unknown (note this in "To confirm").
- Keep the user's side's commitments and the other side's commitments clearly separated in the email.
- If a transcript includes timestamps, add the timestamp next to each decision.

## 3. Output format

```markdown
# [Meeting title / topic] · [Date]
**Participants:** [Names (role)]

## Summary
- [Most important outcome]
- [Second]
- [Third]

## Decisions
1. [Decision] [timestamp if available]

## Action items
| # | Owner | Action | Due | Status |
|---|---|---|---|---|
| 1 | [Name] | [Verb-first, specific action] | [Date or (proposed) date] | Open |

## Open questions
- [Question]: who will answer: [Name/TBD]

## Risks & concerns raised
- [Concern]: raised by [Name]

---

## Follow-up email

**Subject:** Recap & next steps: [topic], [date]

Hi [Names],

Thanks for your time today. Here's a quick recap so we're aligned.

**We agreed**
- [Decision]

**I'll**
- [User's actions with dates]

**Could you**
- [Other side's actions with dates]

**Still open**
- [Question]

Let me know if I've missed or misunderstood anything.
[Your name]

---
**To confirm** (delete before sending)
- [Proposed owners/dates, unclear points in the notes]
```

## 4. Quality checklist

Verify silently:
- [ ] Every action item starts with a verb and has an owner (name, or TBD) and a due date (real, proposed, or TBD)
- [ ] Nothing appears that isn't supported by the notes; inferences are marked (proposed)
- [ ] Decisions and open questions are not mixed
- [ ] Relative dates converted to real dates
- [ ] The email matches the action table exactly
- [ ] Summary has at most three bullets

## 5. Delivery

- Default: Markdown in chat.
- If asked for Word/.docx and file creation is available, create a .docx.

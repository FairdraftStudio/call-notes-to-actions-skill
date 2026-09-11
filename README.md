# Call Notes → Actions: a free Claude skill

Paste a meeting transcript or rough notes. Get back:

- a 3-bullet summary
- decisions (with timestamps if your transcript has them)
- an action table with owner, action, and due date
- open questions and risks
- a ready-to-send follow-up email that matches the action table

It never invents owners or dates: anything implied is marked **(proposed)**, and vague "we should look into…" ideas become actions with owner **TBD** so they don't get lost.

See [`example/`](example/) for a real input and output.

## Install

**Claude app (web or desktop)**
1. Settings > Capabilities: turn on **Code execution and file creation**.
2. Customize > Skills > **Upload skill**, then choose `call-notes-to-actions.zip` from this repo.

**Claude Code**
Copy the `call-notes-to-actions` folder into `~/.claude/skills/` (Windows: `%USERPROFILE%\.claude\skills\`) and restart Claude Code.

## Use

> "Summarise this call and draft the follow-up email." *(paste the transcript)*

## Want the rest of the paperwork done too?

This skill is part of the **Client-Ops Kit** for freelancers and small agencies: proposals with 3-tier pricing, scopes of work, client status reports, and late-invoice follow-ups, as Claude skills plus editable Word/Google Docs templates.

👉 [Get the Client-Ops Kit](https://fairdraftstudio.gumroad.com/l/client-ops-kit) (all 5 skills + Word/Google Docs templates)

Or get individual skills on Agensi:
- [Client Proposal Writer](https://www.agensi.io/skill/2131d629-a403-40c3-82a8-fe99c1d3fabc)
- [Scope of Work Builder](https://www.agensi.io/skill/3f8d33df-8001-43a2-958e-9f38c62257a7)
- [Client Status Report](https://www.agensi.io/skill/63070505-9aa2-4d83-928c-55282ddfc2a2)
- [Invoice Follow-Up](https://www.agensi.io/skill/e6fbd3ea-e505-4a57-b3bb-91295efc4bd0)
- [Call Notes to Actions](https://www.agensi.io/skill/6136e654-ebb4-4a94-b348-e520b4c38d80) (this skill, also free on Agensi)

## License

MIT. See [LICENSE](LICENSE). Not affiliated with or endorsed by Anthropic.

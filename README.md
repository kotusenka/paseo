# Workflow swarm card QA

Recorded in Chromium on Linux on 2026-10-17 against PR #7165.
The source tree is identical to PR commit `0345998483bdbe9bd3f2691ddea0de526b4bf19e`.

The fictional **Accessibility audit** workflow covers 10 site pages and 15
accessibility checks, with 150 distinct agent names listed in `agent-names.json`.
Each tooltip shows the status followed by one complete agent name on the next line,
for example `Sign up touch target audit`.
The real Claude Code Workflow tool runs against a local fake Messages API.
Model replies, delays and failures are simulated; no live site is audited.

- `swarm.gif`: the running workflow, from queued work through completion.
- `hover-failed.png`: Failed — Sign up touch target audit.
- `hover-stalled.png`: Stalled — Home form label audit, after 90 seconds without progress.
- `after-finish.png`: the card has folded back into a Workflow row.
- `capture.txt`: raw browser-capture output and assertions.

The GIF compresses time. Its frames are browser screenshots of the running
application. The PNGs are fresh browser screenshots.

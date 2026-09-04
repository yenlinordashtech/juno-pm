## Diagnostic Diff · Juno RAG Lab

_Working notes from Module 3 Lab 1. Do not paste over `03-rag-prd/prd.md`. That file comes from the AI PRD Builder._

**Prototype:** https://ai-prodraft-buddy.lovable.app

### Before - Quality Mode (no strategy)

Feedback is fragmented across Discord, Notion, and Figma
High
Frustrated
PMs lose hours each week manually copying context between tools, making it hard to trace a signal back to its source.

"I spend maybe two hours every Monday just copying feedback from Discord threads into Notion."
Current AI tools only summarise, they don't draft product briefs
High
Frustrated
Existing note-takers reduce transcription overhead but still require the PM to rewrite output into a shareable PRD format.

"We tried a few AI note-takers. They're great for summaries, but summaries aren't PRDs."
Paying customer signals are buried under internal noise
Medium
Neutral
Without clear source tagging, teams mis-prioritise edge cases from internal testers over requests from enterprise customers.

"We shipped a feature three enterprise customers had asked for, but mis-prioritised the edge case and missed the core use case."

### After - Strategy Mode (with RocketShip Strategy One-Pager)

Resolve CSV Export Crash and Hang on Reports
Frustrated
P0
Reliability First
100/100
Users attempting to export 90-day reports to CSV experience a 5-minute spin followed by a silent crash, completely blocking Excel workflows and forcing manual workarounds.

Directly addresses Pillar 1 (Reliability First), which explicitly identifies CSV export crashes as a P0 reliability bug that blocks core user workflows and risks customer retention. It also aligns with the North Star of supporting mid-market analysts who rely on Excel.

It spins for like 5 minutes and then just crashes. No error message. Just blank. I’ve lost hours because of this.
Dark Mode Support
Positive
P3
0/100
User requested dark mode capability to reduce eye strain during dashboard usage.

Not recommended — Falls under the explicit non-goal list for Q3 (Aesthetic refreshes / dark mode) and provides no direct reliability or speed-to-insight improvement.
The Q3 2026 Strategy Document explicitly lists 'Aesthetic refreshes (dark mode, color palette tweaks, "make it pop" UI work)' under 'WHAT WE ARE NOT DOING THIS QUARTER'.

Oh, and I’d love a dark mode.
Aesthetic Navigation Bar Color Adjustment
Frustrated
P3
0/100
User reported that the new blue navigation bar is overly bright and requested color palette adjustments.

Not recommended — Aesthetic tweak that violates the Q3 focus on core reliability and enterprise compliance.
Color palette tweaks and aesthetic UI changes are explicitly excluded in the Q3 strategy under 'WHAT WE ARE NOT DOING THIS QUARTER'.

The first thing I notice is that the new blue navigation bar is really bright, like hurts my eyes bright. Can we change that?

### Takeaway

> RAG creates differentiation by grounding decisions in company strategy, not generic data.


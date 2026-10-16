# Agents folder starter kit

Give your AI assistant a small, readable home for context you want to keep: important decisions, preferences, projects, and the reasons behind them. Store your working notes privately in Google Drive, where you can inspect and edit them yourself.

## Start with one prompt

1. Open [BOOTSTRAP.md](BOOTSTRAP.md) and copy the prompt into your conversation with any capable AI assistant.
2. Complete any required Drive connection or approval, and choose what information to include.
3. Review the private folder and catch-up schedule your assistant sets up with you.

No code or GitHub account is needed to use the prompt. It starts a guided setup; it does not grant access or install anything automatically.

## Assumptions and scope

- This repository is a **Google Drive-specific prompt-and-template workflow**, not an installed application or universal storage connector
- Any AI assistant or agent can bootstrap it if it has user-authorized Drive read/write tools and can read the agreed chats or other sources. Each agent must verify its own access; access held by one agent does not transfer to another
- Source scope is explicit and limited to material the user chooses and the agent can actually access. This kit does not provide access to every past or future conversation
- Scheduled catch-up requires an available scheduler that can access those sources and update Drive. Verify the actual cadence, time zone, and enabled status; otherwise use manual catch-up
- The concept is portable to S3, Dropbox, and other file stores, but those backends are **not implemented here**. A port needs storage-specific adapters or tools, authorization, links, version/conflict handling, and scheduling integration

## What you get

- **HOME.md:** a short index pointing to the right notes
- **PROTOCOL.md:** your instructions for keeping them useful
- **Topic notes:** concise context, sources, decisions, and open questions
- **ACTIVITY.md:** a small record distinguishing successful checks from actual content changes

For example, your private folder might look like this (create only the topics you need):

```text
Agents/
  HOME.md
  PROTOCOL.md
  ACTIVITY.md
  preferences.md
  projects.md
  learning.md
```

Aim for enduring meaning, not a transcript archive. Keep the reasons and evidence that make a note useful.

## Use with other agents

Choose either of these approaches:

- **Canonical Drive folder:** the owner's authoritative, current notes. Give each agent explicit access only to relevant files, usually read-only first. Reading access does not authorize editing the master
- **Dated shared snapshot:** an explicitly shared copy of selected notes for a particular recipient or agent. Record when it was copied or last synchronized, its source/version where safe to share, and any omitted coverage. Treat it as potentially stale; changes do not automatically flow to or from the canonical folder

Share selectively. Review copied content and source links for the intended recipient; do not include unrelated private notes or inaccessible private links. A snapshot should identify its provenance without disclosing private source details to unauthorized readers. Only an explicitly authorized process may reconcile changes back into the canonical notes.

Explicitly grant your chosen assistant access to the files you want it to use, usually read-only first. Paste your private HOME.md link and say: “Read HOME.md and PROTOCOL.md, then the topic files relevant to this task.”

A link alone grants no access, and this kit provides no automatic synchronization. If several assistants can write, have all of them follow the same fresh-read, version/conflict, and read-back safeguards in PROTOCOL.md; avoid simultaneous writes when those safeguards aren't supported.

## Private by design

This repository contains only generic instructions and blank [templates](templates/). Your actual notes belong in your own private Drive folder. Don't commit populated notes, conversation exports, credentials, or private links to this repository.

Drive access, conversation access, and scheduling depend on what your assistant can actually use. The setup checks these separately. Choose daily or hourly catch-up according to your needs and the scheduler's verified capabilities. If scheduling or conversation access is unavailable, use manual catch-up with material you provide. The folder does not guarantee automatic recall in every future conversation: point your assistant to HOME.md when needed.

## Keep it useful

Edit your notes directly, correct mistakes, and remove information you no longer want stored. The [maintenance protocol](templates/PROTOCOL.md) asks each agent to read fresh copies, preserve your edits, label uncertainty, and verify changes. You remain in control of what goes in.

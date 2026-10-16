# Agents folder starter kit

Give dot a small, readable home for context you want to keep: important decisions, preferences, projects, and the reasons behind them. Store your working notes privately in Google Drive, where you can inspect and edit them yourself.

## Start with one prompt

1. Open [BOOTSTRAP.md](BOOTSTRAP.md) and copy the prompt into your conversation with dot.
2. Complete any required Drive connection or approval, and choose what information to include.
3. Review the private folder and catch-up schedule dot sets up with you.

No code or GitHub account is needed to use the prompt. It starts a guided setup; it does not grant access or install anything automatically.

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

## Use with another assistant

Explicitly grant your chosen assistant access to the files you want it to use, usually read-only first. Paste your private HOME.md link and say: “Read HOME.md and PROTOCOL.md, then the topic files relevant to this task.”

A link alone grants no access, and this kit provides no automatic synchronization. If several assistants can write, have all of them follow the same fresh-read, version/conflict, and read-back safeguards in PROTOCOL.md; avoid simultaneous writes when those safeguards aren't supported.

## Private by design

This repository contains only generic instructions and blank [templates](templates/). Your actual notes belong in your own private Drive folder. Don't commit populated notes, conversation exports, credentials, or private links to this repository.

Drive access, conversation access, and scheduling depend on what your dot can actually use. The setup checks these separately. Daily catch-up is the default; hourly is optional. If scheduling or conversation access is unavailable, use manual catch-up with material you provide. The folder does not guarantee automatic recall in every future conversation: point dot to HOME.md when needed.

## Keep it useful

Edit your notes directly, correct mistakes, and remove information you no longer want stored. The [maintenance protocol](templates/PROTOCOL.md) asks dot to read fresh copies, preserve your edits, label uncertainty, and verify changes. You remain in control of what goes in.

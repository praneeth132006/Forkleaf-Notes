---
title: Launch plan
created: 2026-10-09T11:44:49.769Z
updated: 2026-10-09T11:52:03.118Z
editedBy: praneeth132006
generator: https://forkleaf.vercel.app
---

# Launch plan

Writes land on your device first, then drain to GitHub as one **atomic commit**. Close the laptop mid-sentence; it catches up when you land.

- Nothing is lost when the tab closes
- Offline edits queue and replay
- Conflicts are shown side by side — you pick the version that survives

```mermaid
flowchart TD
    n1([Keystroke])
    n2[IndexedDB]
    n3[Online?]
    n4[Commit]
    n1 --> n2
    n2 --> n3
    n3 --> n4
    %% forkleaf:layout n1:80,80;n2:80,208;n3:88,336;n4:96,464
```
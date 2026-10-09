---
title: Sync engine
created: 2026-10-09T11:42:55.662Z
updated: 2026-10-09T11:43:26.946Z
editedBy: praneeth132006
generator: https://forkleaf.vercel.app
---

# Sync engine

Writes land in IndexedDB first, then drain to GitHub as one atomic commit.
Nothing is lost when the tab closes. Offline edits queue and replay. Conflicts are shown, never merged.
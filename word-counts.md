---
title: Word counts
created: 2026-10-09T11:47:43.143Z
updated: 2026-10-09T11:48:28.102Z
editedBy: praneeth132006
generator: https://forkleaf.vercel.app
---

# Word counts

```python
notes = {"sync-engine": 412, "q3-roadmap": 268, "launch-plan": 133}
total = sum(notes.values())
print(f"{'note':<13}{'words':>6}{'read':>7}{'share':>7}")
for name, words in sorted(notes.items(), key=lambda kv: -kv[1]):
    print(f"{name:<13}{words:>6}{words/230:>6.1f}m{words/total:>7.0%}")
print(f"{'total':<13}{total:>6}{total/230:>6.1f}m")
```

```output
— ran 2026-10-09 11:48 UTC · ok · 41ms
note          words   read  share
sync-engine     412   1.8m    51%
q3-roadmap      268   1.2m    33%
launch-plan     133   0.6m    16%
total           813   3.5m
```
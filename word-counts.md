---
title: Word counts
created: 2026-10-09T11:39:28.749Z
updated: 2026-10-09T11:40:09.581Z
editedBy: praneeth132006
generator: https://forkleaf.vercel.app
---

# Word counts

```python
notes = {"sync-engine": 412, "q3-roadmap": 268, "launch-plan": 133}
```

```output
— ran 2026-10-09 11:40 UTC · ok · 41ms
(no output)
```

total = sum(notes.values())

for name, words in sorted(notes.items(), key=lambda kv: -kv\[1\]):

    share = words / total

    print(f"{name:&lt;12} {words:&gt;4}  {'█' \* round(share \* 24):&lt;24} {share:.0%}")

print(f"{'total':&lt;12} {total:&gt;4}")
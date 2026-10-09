---
title: Word counts 2
created: 2026-10-09T11:40:46.927Z
updated: 2026-10-09T11:41:19.816Z
editedBy: praneeth132006
generator: https://forkleaf.vercel.app
---

# Word counts 2

```python
notes = {"sync-engine": 412, "q3-roadmap": 268, "launch-plan": 133}
total = sum(notes.values())
for name, words in sorted(notes.items(), key=lambda kv: -kv[1]):
    share = words / total
    print(f"{name:<12} {words:>4}  {'█' * round(share * 24):<24} {share:.0%}")
print(f"{'total':<12} {total:>4}")
```
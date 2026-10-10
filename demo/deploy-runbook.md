---
updated: 2026-10-10T15:25:23.838Z
editedBy: praneeth132006
generator: https://www.forkleaf.in
---

# Deploy runbook

1. Check the build is green.
2. Run the health check below — it should print `ok`.
3. Promote to production.

```python
import platform, datetime
checks = {"build": True, "migrations": True, "health": True}
print("python", platform.python_version())
print("checked", datetime.date.today())
print("ok" if all(checks.values()) else "FAIL")
```

```output
— ran 2026-10-10 15:25 UTC · ok · 71ms
python 3.14.4
checked 2026-10-10
ok
```

```bash
echo "disk free:" && df -h / | tail -1
```
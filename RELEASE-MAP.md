# Release Map

| Version | Commit | Date | What Shipped |
|----------|--------|------|--------------|
| v1.0.0 | 4febcc6 | 2026-07-21 | Initial project release |
| v1.1.0 | 86989b6 | 2026-07-21 | Added release documentation |
| v1.1.1 | 82535d9 | 2026-07-21 | Added dummy checkout service |

---

# Rollback Traceability

List releases:

```bash
git tag --sort=-v:refname
```

Roll back to the previous known-good release:

```bash
git checkout v1.1.0
```

Using consistent semantic version tags makes it easy to identify the current and previous releases. Each tag points to a specific commit, making rollbacks precise and reproducible instead of relying on guesswork.
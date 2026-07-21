# Tag Audit

## 1. No release tags exist

Evidence:
Running `git tag` returns no results.

Risk:
There is no way to identify which commit corresponds to a production release, making rollback impossible.

---

## 2. No sortable version history

Evidence:
Running `git tag --sort=-v:refname` returns no results.

Risk:
The team cannot determine the latest release or compare versions in a consistent order.

---

## 3. Feature commits are not associated with releases

Evidence:
Commit `82535d9` - feat: add dummy checkout service

Risk:
Although features exist, there is no release tag identifying when this feature entered production.

---

## 4. Documentation changes are not tied to releases

Evidence:
Commit `86989b6` - docs: add old release notes and changelog

Risk:
Release documentation exists but is not linked to any tagged release, reducing auditability.

---

## 5. Initial project has no baseline release

Evidence:
Commit `4febcc6` - first commit

Risk:
Without an initial release tag (such as `v1.0.0`), there is no known starting point for version history or rollback.
# Versioning Convention

## Semantic Versioning

### MAJOR
Increment the MAJOR version for incompatible or breaking changes.

Example:
v1.4.2 → v2.0.0

### MINOR
Increment the MINOR version when adding new backward-compatible features.

Example:
v1.4.2 → v1.5.0

### PATCH
Increment the PATCH version for backward-compatible bug fixes.

Example:
v1.4.2 → v1.4.3

---

## Tag Naming Format

All production releases use the format:

vMAJOR.MINOR.PATCH

Example:

v1.2.0

---

## Annotated Tags

Production releases use annotated tags because they store the tagger, date, and release message.

Command:

```bash
git tag -a v1.2.0 -m "Release 1.2.0: Added authentication"
```

---

## Pre-release Versions

Release candidates use:

v1.2.0-rc.1

Beta versions use:

v1.2.0-beta.1

Pre-release versions always come before the final release.
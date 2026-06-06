# Incident Log

## Incident 1: Misidentified rollback target

- Date: 2026-04-22
- Severity: High
- Description: Production returned `502` errors after a deployment. The team rolled back to `release_2`, but that tag pointed to an older unsupported commit.
- Root Cause: `release_2` is a lightweight tag with no annotation, and no deployment record linked it to a safe rollback version.

## Incident 2: Undocumented production release

- Date: 2026-05-04
- Severity: Medium
- Description: Operations observed a hotfix deployment from `latest-good`, but the tag did not match any semantic version or release notes.
- Root Cause: Meaningless tag names and missing deployment audit entries.

## Incident 3: Confusion during outage

- Date: 2026-03-31
- Severity: Medium
- Description: Incident responders could not determine which tag was currently running in production.
- Root Cause: Production deployment history contained `Unknown version currently running` and tags like `stable-build` and `patch-new` that did not follow any standard.

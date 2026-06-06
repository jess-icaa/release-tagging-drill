# Deployment History

The Checkout service deployment history contains several gaps and incorrect references.

- `2026-05-04`: Production deployed from tag `latest-good`.
- `2026-04-22`: Emergency rollback to tag `release_2` after payment gateway regression.
- `2026-04-10`: A staging promotion was assumed to match `v1.4.2`, but the production tag is undocumented.
- `2026-03-31`: Unknown version currently running in production.
- `2026-03-15`: Missing deployment record for the release tagged `stable-build`.

These records demonstrate poor version traceability and inconsistent tag usage.

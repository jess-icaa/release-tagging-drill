# Release Notes

## v1.1.1 - 22 July 2026 (Deploy #101)

### Change Scope

- Fixed release-tagging workflow.
- Updated repository documentation.
- Improved deployment validation process.

### Validation

- GitHub Actions workflow: PASS
- Repository builds successfully.
- Manual verification of tags completed.

### Risks

- Incorrect release tags may trigger the wrong deployment.
- Deployment workflow should be monitored after release.

### Rollback

Target: v1.1.0

Steps:

1. Checkout tag v1.1.0
2. Redeploy previous version.
3. Verify deployment health.
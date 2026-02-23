## Last Update
- **Timestamp:** 2026-02-23T01:08:32-08:00
- **Task:** Deploy to Azure SWA
- **Status:** BLOCKED
- **Blocker:** The Azure service principal on the Pi (`717bc8e5-7d0c-43e8-8908-c872c643f1c4`) has no RBAC permissions — cannot read resource groups, list resources, or create Static Web Apps. The `swa` CLI is also not installed. Need either: (1) John to assign Contributor role to the SP on `clawdbot-rg`, or (2) John to create the SWA resource manually from his laptop and provide the deployment token, or (3) use an alternative host like GitHub Pages.
- **Summary:** Attempted to deploy love-message-website to Azure SWA but the service principal has zero Azure permissions. All `az` commands fail with AuthorizationFailed.
- **Files Changed:** HANDOFF.md
- **Committed:** No
- **Verified:** N/A — deployment not possible
- **Deployed URL:** N/A

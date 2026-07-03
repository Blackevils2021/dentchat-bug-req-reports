# E2E screenshots — 2026-05-17

Real Chrome captures (mobile 440px @2x) backing [`../e2e-2026-05-17.md`](../e2e-2026-05-17.md).
Regenerate with the dev server running: `node scripts/e2e-capture.mjs`.

| File | Shows |
|---|---|
| 01-manual-card-reachable.png | Manual-request card reachable for a no-ID-card runner (post-fix) |
| 02-manual-search-results.png | Search by surname returns the matching result |
| 03-manual-request-form.png | Reason + evidence request form |
| 04-myclaims-status-badges.png | MyClaims "Manual request — pending" badge |
| 05-dashboard-en.png | Organizer analytics dashboard (English) |
| 06-dashboard-th.png | Organizer analytics dashboard (Thai) — i18n proof |
| 07-organizer-requested-tier.png | "Requested" review tier (reason/evidence + Confirm/Hold/Reject) |
| 08-organizer-reassign-modal.png | Reassign-claim modal with email-lookup result |

No screenshot contains a real national ID or password. The `/admin/conflicts` (merge) screen is intentionally not captured — it renders a real NID; that flow is evidenced by DB verification in the report.

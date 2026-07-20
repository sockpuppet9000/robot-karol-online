# robot-karol-online Fork Backlog

This queue governs only the `sockpuppet9000/robot-karol-online` public fork. The
canonical product, documentation, deployment and contribution workflow belong to
`Entkenntnis/robot-karol-online` unless a deliberate independent fork is approved.

Reviewed on **2026-07-19**:

```text
fork main:     1cbc74c2d6e5096392fbf7fa48b9136f65810cd7
upstream base: same commit exists in Entkenntnis/robot-karol-online
reviewed upstream comparison head: 0764c57879169897ec91b95897e12ae0c0026e4b
upstream commits after fork main: 461
```

## RKF-001 — Decide the fork's purpose and owner

- Priority: P0 topology
- Status: Open

Choose exactly one supported role:

- [ ] short-lived contribution fork;
- [ ] read-only personal mirror;
- [ ] deliberately maintained downstream fork;
- [ ] archived historical snapshot;
- [ ] deletion after dependency review.

- [ ] Name the human owner and review date.
- [ ] Record why a separate public fork is needed.
- [ ] Prevent the fork from being mistaken for the canonical project.

## RKF-002 — Inventory repository identity and configuration

- Priority: P0 correctness
- Status: Open

- [ ] Record stable GitHub repository IDs for fork and upstream.
- [ ] Verify remotes/default branches and actual fork relationship.
- [ ] Review visibility, archived state, Pages, Actions, branch rules, webhooks,
  deploy keys, Apps, secrets, variables and environments.
- [ ] Remove or disable integrations that imply an independent deployment/release.

## RKF-003 — Produce an exact upstream divergence manifest

- Priority: P0 provenance
- Status: Open

- [ ] Record fork head, upstream comparison head and merge base.
- [ ] List fork-only commits, upstream-only commits and changed paths.
- [ ] Distinguish generated/gallery/content changes from product source.
- [ ] Record LFS/submodules/binaries and large assets.
- [ ] Re-run before any sync or archival decision.

## RKF-004 — Verify whether any fork-only work exists

- Priority: P0 provenance
- Status: Open

- [ ] Inspect all fork branches/tags, not only `main`.
- [ ] Identify commits authored specifically for this fork.
- [ ] Check open/closed PRs and unmerged contribution work.
- [ ] Preserve legitimate unique work before reset/archive/delete.
- [ ] Do not infer “no local changes” only from the current main head.

## RKF-005 — Choose a safe sync strategy

- Priority: P0 destructive safety
- Status: Blocked on role and divergence manifest

- [ ] Prefer fast-forward when the fork has no unique work.
- [ ] Preview exact old/new refs and force/delete effects.
- [ ] Preserve a recovery ref/bundle if history will be rewritten.
- [ ] Require explicit approval for force push, tag replacement or branch deletion.
- [ ] Read back final refs/tree after sync.

## RKF-006 — Preserve upstream product authority

- Priority: P0 governance
- Status: Open

- [ ] Keep product README, docs, issues and release guidance attributed to upstream.
- [ ] Route general bugs/features/security fixes to upstream after review.
- [ ] Do not publish independent releases/packages/Pages from the fork by default.
- [ ] Do not claim ownership of upstream features, branding, hosted service or
  educational content.
- [ ] Keep the fork-status notice small and clearly separate from upstream docs.

## RKF-007 — Review license and attribution

- Priority: P0 rights
- Status: Open

- [ ] Preserve the MIT license and upstream copyright notice.
- [ ] Record authorship/license for any future fork-only code or docs.
- [ ] Review third-party image, font, texture, educational-material and asset
  notices separately from the software license.
- [ ] Keep generated gallery/user submissions under their applicable rights and
  moderation policy.

## RKF-008 — Review public content and user submissions

- Priority: P0 rights/privacy/safety
- Status: Open

- [ ] Inventory gallery images, names, embedded data URLs and user-generated
  materials inherited by the snapshot.
- [ ] Review personal data, trademarks, copyrighted characters/logos and unsafe
  content before any independent publication.
- [ ] Do not use student/user submissions as fork marketing or an icon.
- [ ] Route moderation/removal requests to the canonical owner/process.

## RKF-009 — Review backend and hosted-service boundaries

- Priority: P0 operations/privacy
- Status: Open

- [ ] Identify every upstream backend/API/storage/analytics endpoint in the fork.
- [ ] Do not point a downstream build at the canonical hosted service without
  explicit authorization and compatibility review.
- [ ] Define privacy, retention, abuse, rate-limit and account boundaries for any
  independent deployment.
- [ ] Ensure imprint/contact details are not misleading in a downstream build.

## RKF-010 — Review dependency and build drift

- Priority: P1
- Status: Open

- [ ] Compare package manifests/lockfiles/build config with current upstream.
- [ ] Identify stale security/compatibility issues before running or deploying the
  old snapshot.
- [ ] Pin Node/package-manager versions for any retained build.
- [ ] Use upstream tests/CI guidance at the exact synchronized commit.
- [ ] Do not treat `npm run build` success as permission to deploy.

## RKF-011 — Prevent independent release/deployment

- Priority: P0 remote integrity
- Status: Open

- [ ] Disable Pages, production Actions and deployment credentials unless the fork
  is deliberately operated.
- [ ] Remove package publishing tokens and release automation.
- [ ] Require exact owner/domain/backend/security/legal approval for any downstream
  deployment.
- [ ] Use a distinct name/app identity only after rights and user-confusion review.

## RKF-012 — Define archive or deletion lifecycle

- Priority: P1 terminal lifecycle
- Status: Blocked on dependency and unique-work review

- [ ] Inventory clones, links, PRs, integrations and automation depending on the
  fork.
- [ ] Preserve required contribution refs/patches with provenance.
- [ ] Archive read-only when historical/search value remains.
- [ ] Delete only after explicit approval and dependency/replica review.
- [ ] Record that archive/delete does not recall clones or Git objects already
  distributed.

## RKF-013 — Keep documentation changes fork-local and reversible

- Priority: P1
- Status: Open

- [ ] Avoid rewriting the upstream product narrative merely to document fork
  administration.
- [ ] Keep status/disposition files easy to drop during a future fast-forward.
- [ ] Do not create a long-running downstream documentation conflict unnecessarily.
- [ ] Close this fork-status PR unmerged if the chosen disposition is direct
  sync/archive/delete and the record is preserved elsewhere.

## RKF-014 — Publication and branding policy

- Priority: P0 permanent unless an independent fork is approved
- Status: Permanent

- [ ] Do not present this fork as a separate portfolio product.
- [ ] Do not create a new logo, social preview, screenshots or release page from
  upstream/user content.
- [ ] Link to the canonical upstream for product demonstrations.
- [ ] Any independent downstream brand requires name/trademark/asset/legal review
  and a genuinely maintained product line.

## Decisions recorded

- The reviewed fork `main` commit is an upstream commit, not demonstrated unique
  downstream source.
- The reviewed upstream history has 461 later commits.
- Upstream remains canonical for product features, deployment, issues and releases.
- Technical ability to build or publish the fork is not release authority.
- The safest terminal outcome may be sync, archive or deletion rather than a new
  product README/brand.

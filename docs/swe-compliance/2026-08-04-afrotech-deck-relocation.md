# AfroTech AI Edge Deck Repository Relocation

## Phase 0: Baseline And Manual Lookup

- Scope: relocate the clean AfroTech AI Edge session deck into the AfroTech client-application container.
- Instructions and references: global RUDI instructions, `business/AGENTS.md`, `system/AGENTS.md`, this repo's `README.md`, business ignore/manifest files, and the system registry.
- SWE guidance: explicit invariants, proportional operational safety, post-change verification, and no unapproved deployment.
- Baseline: clean and synced `main` at `975235fa303d189339758284589e5259448ddd86`; origin `https://github.com/learnrudi/afrotech-ai-edge-session-02.git`.
- Source: `/Users/hoff/dev/RUDI/business/engagements/afrotech/projects/afrotech-ai-edge/ai for people leaders/slide-deck`.
- Target: `/Users/hoff/dev/RUDI/apps/clients/afrotech/ai-edge-session-02`.
- Identity: directory inode `402576116`, `.git` inode `402610223`, device `16777234`, 101 files, 0 symlinks, 4,927,488 bytes before this checklist.
- No process, parent-tracked file, absolute-path consumer, or target collision exists.
- Invariants: preserve repository identity, Git state, public workshop content, live deck URL, and unrelated work.
- Exit criteria: baseline is reproducible and target is absent.

## Phase 1: Scope Lock

- In scope: same-filesystem rename, business pointer, exact ignore guard, manifest removal, registry update, local targeted commits.
- Non-goals: deck edits, visibility changes, pushes, deployments, or moving another repo.
- Expected files: this checklist, business `.gitignore`, nested manifest, pointer README, and system registry.
- Failure behavior: stop on collision, device mismatch, dirty source, process use, or identity mismatch.
- Exit criteria: only location contracts change.

## Phase 2: Red Tests

- Observable behavior: target becomes the Git root, old path becomes a pointer, registry reports target as `cloned_root`.
- Red probes: target Git root, pointer title, and target registry path.
- Expected failure: all probes fail before the move.
- Exit criteria: failures are limited to intended location state.

## Phase 3: Implementation

- Move the complete repository once, including `.git`.
- Create the old-path pointer and update exact boundary metadata.
- Do not edit deck source or deployment configuration.
- Exit criteria: payload exists only at target; old path is pointer-only.

## Phase 4: Green Tests And Refactor

- Rerun red probes unchanged.
- Verify inode, file/symlink count, branch, HEAD, upstream, and remote.
- Verify parent tracks only the pointer and ignores future payload.
- Exit criteria: all location and identity checks pass.

## Phase 5: Full Verification

- Run staged diff checks, registry inventory, and nested-boundary audit.
- Build/lint/debt scans are not applicable because source is unchanged and the deck is self-contained static HTML.
- Do not redeploy; verify the documented live deck URL remains unchanged.
- Exit criteria: Git, filesystem, registry, pointer, and docs agree.

## Phase 6: Docs, Contracts, And Closure

- Accepted debt: no external Pages smoke or push is performed.
- Definition of Done: the deck is an independent AfroTech client app under `apps/clients`, with a business pointer and authoritative registry entry.

## Verification Results

- PASS: red location probes failed before the move and passed unchanged afterward.
- PASS: directory inode `402576116` and `.git` inode `402610223` are unchanged on device `16777234`.
- PASS: the repo contains 102 files after this checklist, 0 symlinks, clean deck source, unchanged `main`/HEAD/upstream/origin, and the same documented live URL.
- PASS: the old path is pointer-only, future payload is ignored, and the registry reports the target as `cloned_root`.
- PASS: workspace inventory reports 43 repos, 49 registry entries, 0 unregistered repos, and only the pre-existing external-path issue.
- PASS: no source, visibility, deployment, push, or external state changed.

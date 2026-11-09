---
"releaseproof": patch
---

Rebuild projects whose `pnpm-lock.yaml` has `lockfileVersion: 5.3` with pnpm 6 instead of pnpm 10, which rejects that lockfile. When `packageManager` names npm, pnpm or Yarn without an exact version (for example `npm@latest` or `pnpm@^9`), say that an exact version is needed instead of calling the package manager unsupported.

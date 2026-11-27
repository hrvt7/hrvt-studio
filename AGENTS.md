# AGENTS.md — canvix

## Git identity (mandatory)

All commits in this repository MUST be authored as:

- **Name:** `Ashiq Hussain Mir`
- **Email:** `imsrenpsycho@gmail.com`
- **GitHub account:** `mir-ashiq`

If a noreply address is ever required, the only correct form is
`128612922+mir-ashiq@users.noreply.github.com` (user-id prefix + hyphen).
A wrong noreply guess (`mirashiq@…`) once attributed commits to an
unrelated account and added a phantom contributor (corrected 25 Nov 2026).

Verify before committing:

```bash
git config user.name   # Ashiq Hussain Mir
git config user.email  # imsrenpsycho@gmail.com
```

## Gates (CI order — all green before push)

```bash
npm run typecheck
npm run lint
npm test
npm run build
```

<!-- BEGIN:nextjs-agent-rules -->

## This is NOT the Next.js you know

This version has breaking changes — APIs, conventions, and file structure may all differ from your training data. Read the relevant guide in `node_modules/next/dist/docs/` (resolved from this file's directory; in monorepos the `next` package may not be visible from the repo root) before writing any code. Heed deprecation notices.

This block is written and re-added by `next dev` — verify at `node_modules/next/dist/server/lib/generate-agent-files.js`. Removing it from a diff only re-creates the uncommitted change; committing it with your work keeps the tree clean.

<!-- END:nextjs-agent-rules -->

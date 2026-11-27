# interactive-EXPLAIN

Turn boring PostgreSQL `EXPLAIN` output into something you can click, explore and understand.

Add **one script tag** to your website, app or Claude artifact. Any `EXPLAIN` plan on the page becomes interactive.

Live demo: https://pgprism.dev/

## What is this?

When Postgres runs a query, `EXPLAIN` shows how it plans to do it. The output is long, hard to read and full of numbers.

This tool makes it easier to read. It shows the plan as a table, a tree or a flame graph, and it points out what is slow.

## Features

- **Finds problems for you.** It flags things like bad row estimates and disk spills, and jumps to the node that has the problem.
- **Three views.** Table, tree and flame graph.
- **Readable BUFFERS.** `read=94304` becomes `737 MiB`.
- **Copy for AI.** One click copies the plan so you can paste it into Claude Code, Codex, Antigravity and similar tools.
- **Tiny.** 37 KiB gzipped, zero dependencies.
- **Private.** No backend. Your plans never leave your browser.

## Quick start

Add this to your HTML page:

```html
<script async src="https://cdn.jsdelivr.net/npm/pgprism@0.1.0-beta.2/dist/pgprism.iife.js"></script>
```

That's it. Existing `EXPLAIN` plans on the page become interactive.

For production, keep the version pinned (as above) or download `pgprism.iife.js` and host it yourself.

## Supported

- PostgreSQL 15 to 19
- `EXPLAIN` output as plain text or JSON

## Where can I use it?

- Blog posts
- Documentation and runbooks
- Dashboards
- Single-file HTML reports (works offline)
- Claude artifacts

## Credits

This project is built on [pgPrism](https://github.com/NikolayS/pgprism) by [Nikolay Samokhvalov](https://github.com/NikolayS).
Site: https://pgprism.dev/

## License

Open source under Apache-2.0, the same license as the original project.

# CLAUDE.md

**product-superskills** — 8 AI skills for product management, strategy, GTM, and startup growth.

- **npm package**: `product-superskills` (v1.0.1) — `npx product-superskills` — **8 skills**
- **GitHub**: `https://github.com/ericgandrade/product-superskills`

## Skills (8)
product-strategy, product-discovery, product-delivery, product-leadership, product-architecture, product-operating-model, abx-strategy, startup-growth-strategist

## Version Management
Use `node scripts/release.js [patch|minor|major]`. Publishing via GitHub Actions on `v*` tag push.

## graphify

This project has a graphify knowledge graph at graphify-out/.

Rules:
- Before answering architecture or codebase questions, read graphify-out/GRAPH_REPORT.md for god nodes and community structure
- If graphify-out/wiki/index.md exists, navigate it instead of reading raw files
- After modifying code files in this session, run `graphify update .` to keep the graph current (AST-only, no API cost)

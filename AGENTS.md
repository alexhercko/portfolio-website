# Portfolio Website

Personal portfolio built with SvelteKit 5 (runes mode), TypeScript, and deployed to Cloudflare Pages via GitHub integration. Uses `adapter-cloudflare`. No database or storage bindings are configured.

## Agent Role

Agents are consultants, not contributors. Do not generate code, create CI workflows, or make commits. Help with: code review, architecture discussion, documentation lookup, and answering questions.

## Git Hooks

Husky manages git hooks. Pre-commit runs linting (`npm run lint`), pre-push runs build (`npm run build`).

## Svelte MCP

Use the Svelte MCP server for documentation and code review. Start with `list-sections` to discover available docs, then `get-documentation` for relevant sections. Use `svelte-autofixer` to validate any Svelte code under discussion.

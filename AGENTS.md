# Portfolio Website

Personal portfolio built with SvelteKit 5 (runes mode), TypeScript, and deployed as a Cloudflare Worker via GitHub integration. Uses `adapter-cloudflare`. AGENTS.md is the primary instruction file.

## Agent Role

Agents are consultants, not contributors. Do not generate code, create CI workflows, or make commits. Help with: code review, architecture discussion, documentation lookup, and answering questions.

## Assets

Static assets (images, videos, etc.) are hosted in Cloudflare R2 buckets. Multiple buckets may be used for different purposes. Bucket URLs are configured via `PUBLIC_` environment variables in `.env` locally and in the Cloudflare dashboard for production builds, then referenced in components via `$env/static/public`.

## Git Hooks

Husky manages git hooks. Pre-commit runs linting (`npm run lint`), pre-push runs build (`npm run build`).

## CI

GitHub Actions runs CI on pushes to `main` and on pull requests. The build script runs `wrangler types --check` before `vite build`, so `worker-configuration.d.ts` must be committed and up to date. The types depend on build output (`.svelte-kit/cloudflare/_worker.js`), so they must be regenerated after a local build whenever wrangler config or the build output changes.

## Svelte MCP

Use the Svelte MCP server for documentation and code review. Start with `list-sections` to discover available docs, then `get-documentation` for relevant sections. Use `svelte-autofixer` to validate any Svelte code under discussion.

## Writing Instructions

Keep AGENTS.md entries brief. Each section should be a couple of sentences explaining the setup and how to work with it, not exhaustive configuration details.

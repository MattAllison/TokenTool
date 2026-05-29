# Instructions for AI Agents

Welcome! If you are an AI agent or coding assistant operating in this repository, please read and strictly adhere to the following rules:

## 1. Repository Fork Context (CRITICAL)
This repository is a personal fork and re-write of the official Java-based `RPTools/TokenTool` repository. 
We are building a new desktop version of TokenTool using **Tauri, Svelte, and Rust**.

**Rule:** Under NO circumstances should you interact with the upstream `RPTools/TokenTool` repository unless explicitly instructed by the user. 
When using the GitHub CLI (`gh`) within this local clone, it defaults to opening Pull Requests, Issues, and Comments against the upstream repo.
You MUST ALWAYS specify the correct local fork repository using the `--repo` flag.

### Correct `gh` Usage (DO THIS):
Always use the `--repo MattAllison/TokenTool` flag.
- `gh pr create --repo MattAllison/TokenTool --title "..."`
- `gh issue comment 2 --repo MattAllison/TokenTool --body "..."`
- `gh pr list --repo MattAllison/TokenTool`

### INCORRECT `gh` Usage (DO NOT DO THIS):
- `gh pr create` (This defaults to RPTools/TokenTool!)
- `gh issue comment` (This defaults to RPTools/TokenTool!)

Failure to include the `--repo MattAllison/TokenTool` flag will result in spamming the official maintainers. This is a severe error. Do not do it.

## 2. Tech Stack
- **Frontend:** Svelte (via Vite), TypeScript, Vanilla CSS
- **Backend:** Rust, Tauri
- **Package Manager:** npm (frontend), cargo (backend)

Always prioritize idiomatic, memory-safe, and cleanly typed code (e.g., using `thiserror` for Rust errors instead of strings, and proper Svelte event dispatching).

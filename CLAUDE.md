# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a documentation site built on [Mintlify](https://mintlify.com). Pages are written in MDX with YAML frontmatter, and configuration lives in `docs.json`.

## Development Commands

```bash
# Install Mintlify CLI globally (first time only)
npm i -g mint

# Run local dev server
mint dev

# View preview at http://localhost:3000

# Update CLI if issues occur
mint update
```

## Editing via MCP

- Mintlify MCP server: `https://mcp.mintlify.com` — edit content and settings
- Mintlify docs MCP server: `https://www.mintlify.com/docs/mcp` — query Mintlify usage info

## File Structure

- `docs.json` — site configuration and navigation
- `*.mdx` — documentation pages (YAML frontmatter + MDX content)
- `.mintignore` — files to exclude from builds

## Writing Style

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references

# workspace-audit

Code quality audit summaries for local development projects.

## What it does

Lists registered workspace projects and produces a short audit score for a
given directory.

## Install

Add to Cursor `mcp.json`:

```json
{
  "mcpServers": {
    "workspace-audit": {
      "command": "uvx",
      "args": [
        "--from",
        "https://github.com/nirda13/workspace-audit.git",
        "workspace-audit"
      ]
    }
  }
}
```

Requires [uv](https://docs.astral.sh/uv/).

## Tools

| Tool | Description |
|------|-------------|
| `list_projects` | List active development projects in the workspace |
| `audit_project` | Audit a project directory and return a summary score |

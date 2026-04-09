# clictl

A package manager for AI agents. Install any API, MCP server, or website as a CLI command. Your agent discovers it automatically.

**Website:** [clictl.dev](https://clictl.dev) | **Spec:** [clictl.dev/spec](https://clictl.dev/spec) | **Browse tools:** [clictl.dev/browse](https://clictl.dev/browse)

## Install

**macOS / Linux:**
```bash
curl -fsSL https://download.clictl.dev/install.sh | bash
```

**Homebrew:**
```bash
brew install clictl/cli/clictl
```

**Windows (Scoop):**
```powershell
scoop bucket add clictl https://github.com/clictl/scoop-cli
scoop install clictl
```

## How it works

You write a YAML spec describing an API. `clictl install` turns it into a CLI command and registers it as an MCP server. Both you and your agent use the same tool, the same way.

```bash
clictl install github
clictl run github repo-issues --owner octocat --repo hello-world
```

There are 220+ tools in the registry. Every install creates a skill file your agent reads and an MCP server entry, with no background processes or Docker containers.

## Repositories

### Core

| Repo | Description |
|------|-------------|
| [cli](https://github.com/clictl/cli) | The clictl CLI. Written in Go. |

### Toolboxes

| Repo | Description |
|------|-------------|
| [toolbox](https://github.com/clictl/toolbox) | Official curated toolbox with 220+ tool specs. |
| [toolbox-example](https://github.com/clictl/toolbox-example) | Template for creating your own toolbox. |
| [packs](https://github.com/clictl/packs) | Signed skill pack releases. |

### Distribution

| Repo | Description |
|------|-------------|
| [homebrew-cli](https://github.com/clictl/homebrew-cli) | Homebrew tap for macOS and Linux. |
| [scoop-cli](https://github.com/clictl/scoop-cli) | Scoop bucket for Windows. |

## License

Apache License 2.0. clictl is a [Soap Bucket LLC](https://www.soapbucket.org) project.

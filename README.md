# Rekipedia

> Agentic repo-to-wiki: scan any repository into a portable SQLite knowledge store with wiki pages, diagrams, and grounded Q&A.

---

## Installation

### Homebrew (macOS / Linux) — Recommended

```bash
brew tap unrealandychan/tap
brew install rekipedia
```

### Download Binary

Download the latest release from [GitHub Releases](https://github.com/unrealandychan/rekipedia-releases/releases).

| Platform | Architecture | File |
|----------|-------------|------|
| macOS | Apple Silicon (M1/M2/M3) | `reki_darwin_arm64.tar.gz` |
| macOS | Intel | `reki_darwin_amd64.tar.gz` |
| Linux | x86_64 | `reki_linux_amd64.tar.gz` |
| Linux | ARM64 | `reki_linux_arm64.tar.gz` |
| Windows | x86_64 | `reki_windows_amd64.zip` |

Extract and move to your `$PATH`:

```bash
# macOS (Apple Silicon)
tar -xzf reki_darwin_arm64.tar.gz
mv reki /usr/local/bin/
```

---

## Quick Start

```bash
# Scan a repository and generate wiki
reki scan --path /path/to/repo

# Serve the wiki locally (opens in browser)
reki serve --path /path/to/repo

# Ask questions about the codebase (interactive chat mode)
reki ask --path /path/to/repo -i

# Ask a single question
reki ask --path /path/to/repo "How does the authentication work?"

# Update wiki after code changes
reki update --path /path/to/repo

# Generate embeddings for semantic search
reki embed --path /path/to/repo
```

---

## Commands

| Command | Description |
|---------|-------------|
| `scan` | Scan repository and generate wiki pages |
| `serve` | Start local web server to browse the wiki |
| `ask` | Ask questions about the codebase (supports `-i` interactive chat mode) |
| `update` | Incrementally update wiki after code changes |
| `embed` | Generate embeddings for semantic search (RAG) |

---

## Supported Languages

- Go
- Python
- TypeScript / JavaScript
- Rust
- Java
- Ruby
- C / C++

---

## Links

- [Main Repo](https://github.com/unrealandychan/rekipedia)
- [Homebrew Tap](https://github.com/unrealandychan/homebrew-tap)

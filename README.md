# Finance template

A personal finance and investment tracker that keeps everything on the user's own device: accounts, budgets, net worth over time and an investment portfolio, stored in a single encrypted file. No server, no account, no bank connections.

| Folder | What it is | Stack | Runs on |
| --- | --- | --- | --- |
| [`desktop`](desktop) | Desktop app: core, window and interface | Python, pywebview, SvelteKit | macOS (Windows and Linux through pywebview) |

The folder is a Git submodule with its own repository. The demo brand, "Coffer", and every name in its demo data are fictional.

## Getting started

```bash
git clone --recurse-submodules https://github.com/mattoznav/templates-finance.git
```

Then follow the [`desktop`](desktop) README.

Part of the [`templates`](https://github.com/mattoznav/templates) collection.

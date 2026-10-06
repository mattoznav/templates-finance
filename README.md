# Finance template

A personal finance and investment tracker that keeps everything on the user's own device: accounts, budgets, net worth over time and an investment portfolio, stored in a single encrypted file. No server, no account, no bank connections.

| Folder | What it is | Stack | Runs on |
| --- | --- | --- | --- |
| [`desktop`](desktop) | Desktop app: core, window and interface | Python, pywebview, SvelteKit | macOS (Windows and Linux through pywebview) |

The folder is a Git submodule with its own repository; its README covers the security model, the data model and the CSV formats. The demo brand, "Coffer", and every name in its demo data are fictional.

## Requirements

| Tool | Version |
| --- | --- |
| Git | any recent version |
| Python | 3.11 or newer |
| Node.js and npm | Node 22.12 or newer, to build the interface |

## Install and run

```bash
git clone --recurse-submodules https://github.com/mattoznav/templates-finance.git
cd templates-finance/desktop
python3 -m venv .venv
.venv/bin/pip install -r requirements-dev.txt
cd ui && npm install && npm run build && cd ..
.venv/bin/python -m coffer
```

A window opens. Choose **Create vault** and pick a master password of at least 10 characters, then store the recovery key it shows: there is no other way back in if the password is lost. To look around first, choose **Explore Coffer with demo data**: two years of fictional finances, held in memory and never saved.

There are no default credentials: every vault has only the password chosen when it was created.

## Develop and test

See [`desktop/README.md`](desktop/README.md) for running the interface in a browser with hot reload, the tests and the project layout.

## License

The code is released under the [MIT License](LICENSE).

Part of the [`templates`](https://github.com/mattoznav/templates) collection.

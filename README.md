# Codex Agent Sandbox

This repository is a **fully‑functional agent sandbox** powered by Codex CLI.  It demonstrates how to build, run, and test small self‑contained “agents” that can interact with the host system, access files, run commands, and maintain state across sessions.

## Why an Agent Sandbox?

* **Rapid prototyping** – Quickly spin up a sandboxed environment for your agents without touching the host machine.
* **Safe experimentation** – Agents run in an isolated workspace with sandboxed permissions, so you can test malicious‑looking code safely.
* **Integrated tooling** – The sandbox comes with an in‑repo README, a basic `todo` command‑line app, and optional skills you can drop in.

## Repository Layout

```
├── README.md          ← This file
├── index.html         ← Optional demo page
├── todo.py            ← Simple TODO CLI application
├── requirements.txt   ← Python dependencies
├── .codex/            ← Codex CLI configuration & skills
└── ...                ← Other assets
```

Feel free to modify or extend the `todo.py` script, or add new agents under `.codex/agents`.  All changes are automatically picked up by the sandbox runtime.

## Quick Start

```bash
# Clone the repo (or use the sandbox directly in your terminal)
git clone https://github.com/your-org/agent-sandbox.git
cd agent-sandbox

# Install the Python dependencies
pip install -r requirements.txt

# Run the example TODO app
python todo.py list
```

The sandbox also supports running commands inside the agent runtime:

```bash
codex-cli exec "python todo.py add \"Finish the report\""
```

See the `index.html` for a lightweight UI demo of the TODO app.

## Contributing

Open a pull request or issue any time you want to add new agent examples, improve the sandbox, or extend the tooling.

## License

MIT © Codex Team


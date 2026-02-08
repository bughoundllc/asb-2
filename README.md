# TODO Task Tracking App

A lightweight command‑line application for tracking TODO items. It supports creating,
listing, completing, and deleting tasks while persisting them to a simple JSON file.

## Features
- Add new tasks with an optional description
- List all tasks with status (pending/completed)
- Mark tasks as completed
- Delete tasks
- Persist tasks between runs

## Installation
```bash
# Clone the repository
git clone <repo_url>
cd repo

# Install dependencies (if any)
pip install -r requirements.txt

# Run the application
python todo.py
```

## Usage
```bash
# Add a new task
python todo.py add "Buy milk"

# List all tasks
python todo.py list

# Complete a task (by its ID)
python todo.py complete 1

# Delete a task
python todo.py delete 2
```

## Contributing
Feel free to submit pull requests or open issues for improvements.

## License
MIT © Your Name

# 🐍 Python CLI Prompt Template V 1.1

> A structured, reusable prompt template for building any Python CLI project with AI assistance — from idea to working code, one prompt at a time.

---

## 📖 What Is This?

This is a **prompt engineering template** designed to help you generate complete Python CLI projects using AI (like Claude, ChatGPT, etc.) without writing code manually.

Instead of vague prompts like _"make me a task manager"_, this template gives the AI everything it needs to produce clean, structured, production-ready Python code on the first try.

---

## 📁 Files Included

| File | Description |
|------|-------------|
| `python_cli_prompt_template.md` | The main template with all sections, options, and 3 filled examples |
| `README.md` | This file — how to use the template |

---

## 🚀 Quick Start

**1. Open** `python_cli_prompt_template.md`

**2. Copy** the Full Template section

**3. Fill in** the brackets with your project details:

```
Build a CLI [TOOL NAME] in Python.

## What it does:
[Your description here]

## Commands:
- [your command]: [what it does]
...
```

**4. Paste** the completed prompt into Claude, ChatGPT, or any AI assistant

**5. Follow** the step-by-step prompting order to generate each file

---

## 🧩 Template Sections Explained

| Section | What to fill in |
|---------|----------------|
| **What it does** | A 1-2 sentence description of your tool's purpose |
| **Target Users** | Who will use it (developers, students, personal use) |
| **Commands** | List each CLI command and what it does |
| **Data & Storage** | Where and how data is saved |
| **Technical Requirements** | Python version, CLI library, allowed packages |
| **Input & Output** | How users give input and see results |
| **Error Handling** | What happens when things go wrong |
| **Authentication** | API keys, login, credential storage |
| **Configuration** | Config files, environment variables, defaults |
| **Code Quality** | Docstrings, PEP 8, type hints, logging |
| **Testing** | Unit test framework and coverage target |
| **Packaging** | Entry point, pip install, requirements.txt |

---

## 🗂️ Choosing Your Options

### CLI Library
| Choice | When to use |
|--------|-------------|
| `argparse` | No dependencies needed, simple tools, standard library only |
| `click` | Cleaner syntax, decorator-based, good auto-help |
| `typer` | Modern, type-hint driven, supports auto-completion |

### Storage
| Choice | When to use |
|--------|-------------|
| `JSON file` | Small datasets, human-readable, no setup |
| `SQLite` | Structured queries, medium data, no server needed |
| `PostgreSQL / MySQL` | Large scale, multi-user, production apps |
| `CSV` | Exportable data, spreadsheet-friendly |
| `in-memory` | Prototyping, temporary session data |
| `none` | Stateless tools, pure processing |

### Output Format
| Choice | When to use |
|--------|-------------|
| `plain text` | Simple, scriptable, UNIX-pipeline friendly |
| `colored terminal` | User-friendly UX (`rich` or `colorama`) |
| `JSON` | Machine-readable, API-like output |
| `table` | Structured data display (`rich` or `tabulate`) |
| `CSV` | Exportable results |

---

## 🔁 Step-by-Step Prompting Workflow

After sending your starter prompt, **always follow this order**:

```
Step 1 → Ask for folder/file structure (no code yet)
Step 2 → Generate models.py (data classes)
Step 3 → Generate storage.py (read/write logic)
Step 4 → Generate core logic (business functions)
Step 5 → Generate CLI layer (argparse/click/typer commands)
Step 6 → Add error handling throughout
Step 7 → Generate unit tests
Step 8 → Generate README for the project
```

**Why this order matters:** Each file depends on the one before it. Generating them in order prevents the AI from contradicting itself or making incompatible assumptions.

---

## ✅ Filled Examples Included

The template file contains 3 ready-to-use filled examples you can study or use directly:

### Example 1 — Task Manager
- Storage: JSON file
- Library: click + rich
- Features: add, list, done, delete, clear

### Example 2 — Weather CLI Tool
- Storage: JSON config + live API
- Library: typer + requests + rich
- Features: current weather, 5-day forecast, API key management

### Example 3 — Expense Tracker
- Storage: SQLite database
- Library: click + rich + tabulate
- Features: add, list, delete, summary, CSV export

---

## 💡 Tips for Best Results

**Do this every time:**
- Always ask for **structure before code** — it prevents major rewrites
- **Paste existing code** into each follow-up prompt so the AI stays in sync
- Generate **one file per prompt** — not everything at once

**Common mistakes to avoid:**
- Don't say _"make the whole project"_ — break it into steps
- Don't skip the structure step — it's the blueprint for everything else
- Don't forget to mention your Python version — it affects available syntax

**When you hit errors:**
```
Paste this into your next prompt:

"I got this error: [paste error message]
Here is the relevant code: [paste code]
What is wrong and how do I fix it?"
```

---

## 📋 Example: Minimal Starter Prompt

```
Build a CLI Note-Taking App in Python.

## What it does:
Saves and retrieves short text notes from the terminal.

## Commands:
- add: saves a new note with a title and body
- list: shows all note titles
- view: displays the full body of a note by ID
- delete: removes a note by ID

## Data & Storage:
- Storage type: JSON file
- Data to store: id, title, body, created_at
- File location: ~/.notes/notes.json

## Technical Requirements:
- Language: Python 3.10+
- CLI library: argparse
- Standard library only: yes
- OS support: all

## Code Quality:
- Docstrings, PEP 8, type hints
- Error handling: yes

## Deliverables (do not write code yet):
1. Folder and file structure
2. One-line description of each file
3. All CLI commands with example usage
```

---

## 🔖 Version History

| Version | Changes |
|---------|---------|
| 1.1 | Added Example 3 (Expense Tracker), expanded options tables |
| 1.0 | Initial release with full template and 2 examples |

---

*Made for use with Claude, ChatGPT, or any AI assistant that supports detailed prompting.*

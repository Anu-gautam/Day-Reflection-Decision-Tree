# Day Reflection Decision Tree

> *An interactive end-of-day journalling tool powered by a Python AI agent*

---

## What Does This Project Do?

At the end of a workday, it can be hard to know **how** you really showed up — not just what you did, but *how* you thought and felt about it.

This tool is a short, guided **5-minute reflection exercise** that asks you a handful of targeted questions and then gives you a personalised insight into your mindset for that day.

Think of it like a smart questionnaire: based on how you answer each question, it steers you down a different path and ends with a plain-English summary of your day's "mental profile."

---

## How It Works (No Tech Knowledge Needed)

1. **You run the programme** and it greets you with a prompt.
2. **It asks questions** — one at a time — about how your day felt. For example:
   - *"When you think about the 'shape' of your day, which feels most true?"*
   - Options: `I drove the day` / `The day drove me` / `It was a tug-of-war`
3. **Depending on your answer**, it follows up with a more specific question (just like a real conversation).
4. After each section, it gives you a short **reflection insight** before moving on.
5. At the end, it prints a **personalised summary** like:
   > *"Reflecting on today: You navigated with an internal locus, a focus on contribution, and an altro radius of concern."*

---

## What the Tool Measures

The reflection is built around **three axes of self-awareness**:

| Axis | What It Explores | Two Ends of the Spectrum |
|---|---|---|
| **Locus** | Did you feel in control of your day, or did the day control you? | Victor ↔ Victim |
| **Orientation** | Were you focused on what you could *give*, or on what you deserved to *get*? | Contribution ↔ Entitlement |
| **Radius** | When you were stressed, were you thinking about yourself or about others? | Self-focused ↔ Others-focused |

There are no "right" answers. The goal is honest self-awareness, not a score.

---

## Why This Project Was Built

This project demonstrates how **AI-agent thinking** can be applied to personal development — not just business problems. It shows:

- **Structured reasoning**: The branching logic mirrors how a skilled coach would guide a conversation.
- **State tracking**: The programme remembers your answers throughout the session and uses them in the final summary.
- **Data-driven design**: The entire conversation flow is stored in a separate data file (`reflection-decision-tree.json`), meaning the questions and logic can be updated without touching the code.

---

## What's Inside the Repository

| File | What It Is |
|---|---|
| `Simple-agent.ipynb` | The main Python programme (a Jupyter Notebook — an interactive coding environment) |
| `reflection-decision-tree.json` | The "script" for the entire conversation — all questions, answers, and branching rules |
| `decision-tree-visualization.png` | A visual map of all the possible conversation paths |

---

## Technologies Used

| Technology | Plain-English Description |
|---|---|
| **Python** | The programming language the tool is written in |
| **Jupyter Notebook** | An interactive environment that lets you run code step by step, like a document that also executes |
| **JSON** | A lightweight, human-readable file format used to store the conversation logic |

---

## How to Run It

1. Make sure Python and Jupyter are installed on your computer.
2. Open a terminal and navigate to this folder.
3. Run `jupyter notebook` and open `Simple-agent.ipynb`.
4. Click **Run All** and follow the prompts in the output area.

> **Note:** The JSON file uses comment-style annotations (`/* ... */`) for readability. Python's standard JSON reader does not support comments, so a small pre-processing step (stripping comments before loading) is needed to run the file without errors.

---

## Skills Demonstrated

- Designing a **conversational AI agent** with branching logic and state management
- Separating **data from code** (the conversation lives in JSON; the engine lives in Python)
- Applying **psychological frameworks** (Locus of Control, Contribution vs. Entitlement, Self-Transcendence) to a software problem
- Writing **clean, readable Python** with a class-based structure

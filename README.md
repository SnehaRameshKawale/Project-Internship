# Daily Reflection Tree (Deterministic Reflection Agent)

## 📌 Overview

This project implements a **deterministic reflection tool** that guides a user through an end-of-day reflection using a structured decision tree.

Unlike AI-based chat systems, this tool is:

* Fully deterministic (same input → same output)
* Based on fixed options (no free text)
* Designed using psychological frameworks

---

## 🧠 Concept

The reflection is built across **three psychological axes**:

### 1. Locus (Control)

* Victim vs Victor mindset
* Measures how much control the user takes over their actions

### 2. Orientation (Contribution)

* Contribution vs Entitlement
* Measures whether the user focused on giving or expecting

### 3. Radius (Perspective)

* Self vs Others
* Measures how broadly the user viewed their day

---

## 🌳 How It Works

The system is implemented as a **decision tree**:

* Each node represents a step (question, decision, reflection)
* User selects from fixed options
* Based on selection, the system moves to the next node
* No randomness, no AI calls — fully rule-based

---

## 📂 Project Structure

```
tree/
  reflection-tree.json   → Main tree structure

diagrams/
  reflection-tree-diagram.png   → Visual flow of the tree

write-up.md   → Design explanation
README.md     → Project documentation
```

---

## ⚙️ Node Types Used

* **start** → Entry point
* **question** → User selects one option
* **decision** → Internal branching logic
* **reflection** → Insight based on answers
* **bridge** → Transition between axes
* **summary** → Final reflection
* **end** → Session close

---

## 🔒 Key Constraints Followed

* No LLM used at runtime
* Fully deterministic flow
* Fixed options for all questions
* Structured tree format (JSON)
* Covers all 3 axes in sequence

---

## 🚀 Optional Execution (Part B)

This project can be extended into a CLI/Web app that:

* Reads the JSON tree
* Walks through nodes
* Tracks user responses
* Displays final reflection

---

## ✍️ Author

* Name: Sneha R. Kawale
* Role: Business Analyst / Data Science Candidate

---

## 📌 Note

This project focuses on **knowledge engineering** — transforming psychological concepts into structured, navigable systems.

---


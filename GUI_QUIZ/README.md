# 🧒 Smart Kids Learning Games (AI)

An interactive educational desktop application built with **Python and Tkinter**, designed to help kids learn through fun quizzes covering Math, General Knowledge, and Spelling.

---

## 📋 Table of Contents

- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Game Modes](#game-modes)
- [Code Overview](#code-overview)
- [Known Limitations](#known-limitations)
- [Future Improvements](#future-improvements)

---

## ✨ Features

- ➕ **Math Quiz** — randomly generated arithmetic expressions using `+`, `-`, `*`
- 🧠 **GK Quiz** — general knowledge questions for kids
- 📚 **Spelling Game** — unscramble jumbled words to find the correct spelling
- 🎯 **Score Tracking** — tracks correct answers in real time
- 🔄 **Reset Button** — clears score, question, and entry in one click
- ✅ **Answer Validation** — green for correct, red for wrong answers
- ⚠️ **Quiz Guard** — alerts the kid to select a quiz before submitting
- 🔒 **Fixed Window Size** — consistent layout across all devices

---

## 🛠️ Requirements

- Python 3.6+
- [`simpleeval`](https://pypi.org/project/simpleeval/) — safe math expression evaluator
- `tkinter` — built into Python (no separate install needed)

---

## 📦 Installation

1. **Clone or download** the repository:
   ```bash
   git clone https://github.com/your-username/smart-kids-learning-games.git
   cd smart-kids-learning-games
   ```

2. **Install dependencies:**
   ```bash
   pip install simpleeval
   ```

3. **Run the program:**
   ```bash
   python kids_game.py
   ```

---

## 🚀 Usage

1. Launch the app — the main window opens with 3 quiz buttons.
2. Click any quiz button to load a question.
3. Type your answer in the entry box.
4. Click **🎰 SUBMIT ANSWER** to check.
   - 🎊 Correct → score increases by 1
   - 👍 Wrong → entry turns red with a friendly message
5. Click **🔄 Reset** to clear everything and start fresh.

---

## 🎮 Game Modes

### ➕ Math Quiz
- Generates a random arithmetic expression using two numbers (1–10)
- Supports addition, subtraction, and multiplication
- Example: `3  *  7  =  ?`

### 🧠 GK Quiz
- Displays a random general knowledge question
- Answer is checked case-insensitively
- Example: `how many legs does a cat have?`

### 📚 Spelling Game
- Displays a jumbled/reversed word
- Kid must type the correct unscrambled word
- Example: `elppa` → Answer: `apple`

---

## 🗂️ Code Overview

| Function | Description |
|---|---|
| `mathquiz()` | Generates a random math expression and displays it |
| `GK()` | Picks a random GK question from the dictionary |
| `Spelling()` | Picks a random jumbled word from the dictionary |
| `submit1()` | Validates the answer and updates the score |
| `reset()` | Resets score, clears question and entry box |

### Layout Structure

```
┌─────────────────────────────────────────┐
│     🤖 AI EDUCATION GAMES FOR KIDS      │  ← Title label
│                                         │
│         [ Question appears here ]       │  ← label2
│                                         │
│            [ Entry Box ]                │  ← entry
│                                         │
│  [➕ MATH] [🧠 GK QUIZ] [📚 SPELLING]  │  ← 3 quiz buttons
│                                         │
│          [🎰 SUBMIT ANSWER]             │  ← submit button
│                                         │
│       SCORE:  0                         │  ← score display
│                                         │
│            [🔄 Reset]                   │  ← reset button
└─────────────────────────────────────────┘
```


---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 🙌 Acknowledgements

- [`simpleeval`](https://pypi.org/project/simpleeval/) for safe math expression evaluation
- Python's built-in `tkinter` for the GUI
- `random` module for generating questions dynamically

# User Flow

## Overview

A user flow shows the path a user takes to complete a task inside the app.

For NoteFlow, the main user flow focuses on helping a beginner music student start a short note-reading practice, answer questions, see the result, and check progress.

---

## Main User Flow

The main flow of NoteFlow is:

**Welcome → Home → Practice → Result → Progress**

---

## Flow Steps

### 1. Welcome Screen

The user opens the app and sees a short introduction to NoteFlow.

The screen explains that the app helps users practice note reading step by step.

Main actions:

* Start Practice
* View Progress

---

### 2. Home Screen

The user enters the Home Screen and sees the main practice options.

The Home Screen includes:

* Greeting
* Today’s Practice
* Quick Actions
* Progress Preview
* Bottom Navigation

Main action:

* Start Practice

---

### 3. Practice Screen

The user starts a note-reading practice session.

The Practice Screen shows:

* Current question
* Practice progress
* Music staff with a note
* Multiple-choice answer options
* Next button

Main actions:

* Select an answer
* Move to the next question

---

### 4. Result Screen

After completing the practice session, the user sees the result.

The Result Screen shows:

* Number of correct answers
* Accuracy percentage
* Weak notes
* Encouraging feedback
* Practice Again button
* View Progress button

Main actions:

* Practice Again
* View Progress

---

### 5. Progress Screen

The user checks their learning progress.

The Progress Screen shows:

* Practice streak
* Average accuracy
* Total practice time
* Weekly accuracy chart
* Weak notes
* Recommended practice

Main actions:

* Start Review
* Go back to Practice
* Use Bottom Navigation

---

## User Flow Diagram

```text
User opens app
      ↓
Welcome Screen
      ↓
Home Screen
      ↓
Start Practice
      ↓
Practice Screen
      ↓
Answer Questions
      ↓
Result Screen
      ↓
View Progress
      ↓
Progress Screen
```

---

## Navigation Flow

The main navigation is designed to be simple for beginner users.

```text
Welcome
   ↓
Home
   ↓
Practice
   ↓
Result
   ↓
Progress
```

The Bottom Navigation allows the user to move between:

* Home
* Practice
* Progress

---

## Key User Actions

The most important user actions are:

* Start Practice
* Select Answer
* Continue to Next Question
* View Result
* Review Weak Notes
* View Progress
* Practice Again

---

## Flow Design Decisions

### Simple Entry Point

The Start Practice button is designed as the main action so the user can quickly begin.

### One Task at a Time

The Practice Screen focuses on one note question at a time to reduce confusion.

### Result After Practice

The Result Screen gives the user a clear summary after completing the practice session.

### Progress After Result

The Progress Screen helps the user understand improvement over time and stay motivated.

---

## Summary

The NoteFlow user flow is designed to be short, clear, and beginner-friendly.

The user can quickly move from opening the app to starting practice, answering questions, reviewing results, and checking progress.

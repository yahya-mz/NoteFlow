# User Flow

## Overview

A user flow shows the path a user takes to complete a task inside the app.

For NoteFlow, the main user flow is designed to help a beginner music student start a short note-reading practice, answer questions, receive feedback, and check progress.

This flow is based on the UX foundations, proto-research, affinity diagram, and proto-persona. The goal is to keep the experience short, clear, and beginner-friendly.

---

## UX Sources Used for the Flow

The user flow was shaped by previous UX steps:

* UX Foundations
* UX Research
* Affinity Diagram
* Proto-Persona
* Information Architecture

These steps showed that beginner users need:

* A simple way to start practice
* Short and focused exercises
* Clear feedback after answering
* A way to review weak notes
* Visible progress to stay motivated

---

## Main User Flow

The main flow of NoteFlow is:

**Welcome → Home → Practice → Result → Progress**

This flow follows the user’s main learning journey:

**Understand the app → Start practice → Answer questions → See result → Check progress**

---

## Research-Based Flow Decisions

| UX Finding                                                | Source                        | Flow Decision                                               |
| --------------------------------------------------------- | ----------------------------- | ----------------------------------------------------------- |
| Beginner users need a clear starting point.               | UX Foundations, Persona       | Start the flow with Welcome and Home before Practice.       |
| Users prefer short and simple practice.                   | UX Research, Affinity Diagram | Place Start Practice as the main action on the Home Screen. |
| Users may feel confused if too many tasks appear at once. | Persona, UX Foundations       | Keep the Practice Screen focused on one question at a time. |
| Users need immediate feedback after practice.             | Affinity Diagram, UX Research | Show the Result Screen directly after Practice.             |
| Users want to know what to review.                        | UX Research, Affinity Diagram | Show Weak Notes on the Result Screen.                       |
| Seeing progress can motivate users to continue.           | Persona, Affinity Diagram     | Let users move from Result to Progress.                     |

---

## Flow Steps

## 1. Welcome Screen

The user opens the app and sees a short introduction to NoteFlow.

The screen explains that the app helps users practice note reading step by step.

### Main Actions

* Start Practice
* View Progress

### UX Reasoning

Based on UX Foundations, the user should quickly understand what the app does and what they can do next.

Because of this, the Welcome Screen uses a simple introduction and clear actions.

---

## 2. Home Screen

The user enters the Home Screen and sees the main practice options.

The Home Screen includes:

* Greeting
* Today’s Practice
* Quick Actions
* Progress Preview
* Bottom Navigation

### Main Action

* Start Practice

### UX Reasoning

Based on the UX Research and Affinity Diagram, beginner users need short and simple practice.

Because of this, Today’s Practice is placed as the main action on the Home Screen.

The Home Screen also includes a progress preview because the persona may feel more motivated when progress is visible.

---

## 3. Practice Screen

The user starts a note-reading practice session.

The Practice Screen shows:

* Current question
* Practice progress
* Music staff with a note
* Multiple-choice answer options
* Next button

### Main Actions

* Select an answer
* Move to the next question

### UX Reasoning

Based on the Proto-Persona, beginner users may feel stressed or confused if the practice screen has too much information.

Because of this, the Practice Screen focuses on one note question at a time.

Based on the Affinity Diagram, users need simple and clear feedback. Therefore, answer options are designed with different states such as Default, Selected, Correct, and Wrong.

---

## 4. Result Screen

After completing the practice session, the user sees the result.

The Result Screen shows:

* Number of correct answers
* Accuracy percentage
* Weak notes
* Encouraging feedback
* Practice Again button
* View Progress button

### Main Actions

* Practice Again
* View Progress

### UX Reasoning

Based on the Affinity Diagram, users need immediate and supportive feedback after practice.

Because of this, the Result Screen appears directly after the Practice Screen.

Based on the UX Research assumptions, users may not know which notes they should review. Therefore, Weak Notes are shown on the Result Screen.

The screen also includes Practice Again and View Progress so the user can either repeat the learning activity or reflect on improvement.

---

## 5. Progress Screen

The user checks their learning progress.

The Progress Screen shows:

* Practice streak
* Average accuracy
* Total practice time
* Weekly accuracy chart
* Weak notes
* Recommended practice

### Main Actions

* Start Review
* Go back to Practice
* Use Bottom Navigation

### UX Reasoning

Based on the Persona and Affinity Diagram, seeing progress can motivate beginner users to continue practicing.

Because of this, the flow allows users to move from Result to Progress.

The Progress Screen also includes weak notes and recommended practice because users need to understand their next learning step.

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

Result is not included in the Bottom Navigation because it is a temporary screen that appears after completing a practice session.

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

### 1. Simple Entry Point

Based on UX Foundations, beginner users need to understand the product quickly.

Because of this, the flow starts with a simple Welcome Screen and then moves to the Home Screen.

---

### 2. Start Practice as the Main Action

Based on UX Research and the Affinity Diagram, users need short and achievable practice.

Because of this, Start Practice is the main action on the Home Screen.

---

### 3. One Task at a Time

Based on the Proto-Persona, the user may feel confused or stressed by complex screens.

Because of this, the Practice Screen focuses on one note question at a time.

---

### 4. Result After Practice

Based on the Affinity Diagram, users need clear feedback after practice.

Because of this, the Result Screen comes directly after the Practice Screen and shows score, accuracy, weak notes, and next actions.

---

### 5. Progress After Result

Based on the Persona and UX Research assumptions, progress can help users stay motivated.

Because of this, users can move from the Result Screen to the Progress Screen to see improvement and recommended practice.

---

## Summary

The NoteFlow user flow is designed to be short, clear, and beginner-friendly.

The flow is based on previous UX findings, especially the need for simple practice, clear feedback, weak note review, and visible progress.

The user can quickly move from opening the app to starting practice, answering questions, reviewing results, and checking progress.

# Prototype

## Overview

A prototype is an interactive version of the design that shows how users move through the app before the product is developed.

For NoteFlow, the prototype was created in Figma to test the main user journey:

**Welcome → Home → Practice → Result → Progress**

The goal of the prototype is to show the main flow of the app, not to build the final functional product.

---

## Prototype Export

The prototype flow export can be viewed here:

![Prototype Flow](../exports/prototype-flow.png)

The Figma prototype link is stored here:

[View Figma Link](../figma-link.txt)

---

## UX Sources Used for the Prototype

The prototype was shaped by previous UX steps:

* UX Foundations
* Design Thinking
* UX Research
* Affinity Diagram
* Proto-Persona
* User Flow
* Information Architecture
* Wireframes
* Design System

These steps showed that beginner music students need:

* A clear starting point
* Short and focused practice
* Simple navigation
* Clear answer selection
* Immediate result after practice
* Weak note review
* Visible progress

Because of these findings, the prototype focuses on a simple and beginner-friendly practice journey.

---

## Main Prototype Flow

The main prototype flow is:

**Welcome → Home → Practice → Result → Progress**

### Flow Explanation

1. The user starts from the Welcome Screen.
2. The user moves to the Home Screen.
3. The user starts a practice session.
4. The user answers a note-reading question.
5. The user sees the Result Screen.
6. The user can view Progress or practice again.

---

## Prototype Interactions

## 1. Welcome Screen

### Interaction

* `Start Practice` leads to the Home or Practice flow.
* `View Progress` leads to the Progress Screen.

### UX Reasoning

Based on UX Foundations, the user should quickly understand the purpose of the app and what action to take.

Because of this, the Welcome Screen includes clear entry actions.

---

## 2. Home Screen

### Interaction

* `Start Practice` leads to the Practice Screen.
* Quick action cards can represent access to Flashcards, Progress, or Weak Notes.
* Bottom Navigation allows access to Home, Practice, and Progress.

### UX Reasoning

Based on UX Research and the Affinity Diagram, beginner users need short and simple practice.

Because of this, the Home Screen makes Start Practice the main action.

The Progress Preview also supports motivation by showing improvement early in the experience.

---

## 3. Practice Screen

### Interaction

* The user selects an answer option.
* The answer option can move between states such as Default, Selected, Correct, and Wrong.
* `Next` leads to the Result Screen in the current prototype.

### UX Reasoning

Based on the Proto-Persona, beginner users may feel confused if too many things happen at once.

Because of this, the Practice Screen focuses on one note question at a time.

Based on the Affinity Diagram, users need clear feedback, so answer states are included in the design system and can be represented in the prototype.

---

## 4. Result Screen

### Interaction

* `Practice Again` returns to the Practice Screen.
* `View Progress` leads to the Progress Screen.

### UX Reasoning

Based on the Affinity Diagram, users need immediate and supportive feedback after practice.

Because of this, the Result Screen appears directly after Practice.

The screen shows score, accuracy, weak notes, and next actions so the user understands both performance and next steps.

---

## 5. Progress Screen

### Interaction

* `Start Review` can lead back to Practice.
* Bottom Navigation allows the user to move between main sections.

### UX Reasoning

Based on the Persona and UX Research assumptions, seeing progress can motivate beginner users.

Because of this, the prototype includes a dedicated Progress Screen with stats, weekly accuracy, weak notes, and recommended practice.

---

## Research-Based Prototype Decisions

| UX Finding                                  | Source                        | Prototype Decision                         |
| ------------------------------------------- | ----------------------------- | ------------------------------------------ |
| Beginner users need a clear starting point. | UX Foundations, Persona       | Start the prototype with Welcome and Home. |
| Users need short and simple practice.       | UX Research, Affinity Diagram | Make Start Practice the main action.       |
| Users may feel confused by complex flows.   | Persona                       | Keep the prototype flow linear and simple. |
| Users need feedback after practice.         | Affinity Diagram              | Show Result immediately after Practice.    |
| Users want to know what to review.          | UX Research                   | Show Weak Notes on Result and Progress.    |
| Seeing progress can motivate users.         | Persona, Affinity Diagram     | Add Progress as a main destination.        |

---

## Prototype Purpose

The prototype was created to:

* Demonstrate the main user journey
* Test screen-to-screen navigation
* Show the relationship between Practice, Result, and Progress
* Make the app idea easier to understand
* Prepare the design for future usability testing
* Support developer handoff

---

## What the Prototype Tests

In a future usability test, the prototype could be used to check whether users can:

* Understand what NoteFlow does
* Find the Start Practice button
* Start a practice session
* Select an answer
* Understand the result
* Recognize weak notes
* Open the Progress Screen
* Understand their next step

---

## Prototype Limitations

This prototype is not a fully functional app.

The current version shows the main interaction flow and screen structure, but it does not include:

* Real question logic
* Real answer validation
* Real progress calculation
* User accounts
* Saved practice history
* Backend integration

These features would be added during frontend and backend development.

---

## Connection to Developer Handoff

The prototype supports developer handoff by showing:

* Main screen order
* Navigation flow
* Primary actions
* Component states
* Dynamic behavior expectations
* User journey logic

For example, the Progress Ring in the Result Screen should later become a dynamic frontend component that receives an accuracy value from practice results.

---

## Summary

The NoteFlow prototype shows the main learning journey of a beginner music student.

It connects the UX research, user flow, information architecture, wireframes, and design system into one clickable experience.

The prototype helps explain how the user starts practice, answers questions, receives feedback, and checks progress.

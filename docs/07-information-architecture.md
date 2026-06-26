# Information Architecture

## Overview

Information Architecture, or IA, is about organizing the content, screens, and navigation of an app in a clear and understandable way.

For NoteFlow, the goal of the information architecture is to help beginner music students move through the app without confusion.

The IA is not only based on visual layout. It is based on the UX foundations, proto-research, affinity diagram, and proto-persona.

The main structure is designed around this simple learning journey:

**Start practice → Answer questions → See result → Check progress**

---

## UX Sources Used for IA

The information architecture of NoteFlow was shaped by the previous UX steps:

* UX Foundations
* Design Thinking
* UX Research
* Affinity Diagram
* Proto-Persona
* User Flow

These steps helped define what the user needs and how the app should be organized.

---

## Research-Based IA Decisions

| UX Finding                                                         | Source                        | IA Decision                                                                                       |
| ------------------------------------------------------------------ | ----------------------------- | ------------------------------------------------------------------------------------------------- |
| Beginner users need short and simple practice.                     | UX Research, Affinity Diagram | Place Today’s Practice as the main section on the Home Screen.                                    |
| Beginner users may feel confused if too many tasks appear at once. | Persona, UX Foundations       | Keep the Practice Screen focused on one question at a time.                                       |
| Users need immediate feedback after practice.                      | Affinity Diagram, UX Research | Add a separate Result Screen after the Practice Screen.                                           |
| Users want to know which notes they should review.                 | UX Research, Affinity Diagram | Include Weak Notes in both the Result Screen and Progress Screen.                                 |
| Seeing progress can motivate users to continue.                    | UX Research, Persona          | Create a dedicated Progress Screen with streak, accuracy, weekly chart, and recommended practice. |
| Beginner users need simple navigation.                             | UX Foundations, Persona       | Use clear screen names and a simple Bottom Navigation with Home, Practice, and Progress.          |

These decisions help connect the app structure directly to user needs instead of organizing screens only based on visual appearance.

---

## App Structure

```text
NoteFlow
│
├── Welcome
│
├── Home
│   ├── Greeting
│   ├── Today's Practice
│   ├── Quick Actions
│   └── Progress Preview
│
├── Practice
│   ├── Question
│   ├── Progress Bar
│   ├── Music Staff
│   ├── Answer Options
│   └── Next Button
│
├── Result
│   ├── Score
│   ├── Accuracy
│   ├── Weak Notes
│   ├── Encouraging Message
│   └── Actions
│
└── Progress
    ├── Practice Streak
    ├── Average Accuracy
    ├── Total Practice Time
    ├── Weekly Accuracy Chart
    ├── Weak Notes
    └── Recommended Practice
```

---

## Screen Breakdown

## 1. Welcome Screen

The Welcome Screen introduces the app and gives the user a simple entry point.

### Content

* App name
* Short description
* Music-related visual
* Start Practice button
* View Progress button

### UX Reasoning

Based on UX Foundations, the user should quickly understand what the app does and what action to take first.

Because of this, the Welcome Screen uses a simple introduction and clear primary action.

### Purpose

The purpose of this screen is to explain the value of the app quickly and help the user start.

---

## 2. Home Screen

The Home Screen acts as the main dashboard.

### Content

* Greeting
* Today’s Practice
* Quick action cards
* Weekly progress preview
* Bottom navigation

### UX Reasoning

Based on the UX Research and Affinity Diagram, beginner users need short and simple practice.

Because of this, Today’s Practice is placed as the main section on the Home Screen.

The Home Screen also includes Quick Actions and a Progress Preview, because users may want quick access to flashcards, weak notes, or progress.

### Purpose

The purpose of this screen is to help the user quickly access practice and see a preview of progress.

---

## 3. Practice Screen

The Practice Screen is focused on one main task: answering a note-reading question.

### Content

* Question title
* Question progress
* Music staff
* Note visual
* Multiple-choice answer options
* Next button

### UX Reasoning

Based on the Proto-Persona, the beginner user may feel confused or stressed if the screen shows too much information at once.

Because of this, the Practice Screen focuses on one question at a time.

Based on the Affinity Diagram, users need clear feedback and simple practice. Therefore, the answer options are designed to be easy to understand and easy to tap.

### Purpose

The purpose of this screen is to keep the practice experience focused, simple, and beginner-friendly.

---

## 4. Result Screen

The Result Screen summarizes the user’s performance after practice.

### Content

* Encouraging message
* Score
* Accuracy percentage
* Progress ring
* Weak notes
* Practice Again button
* View Progress button

### UX Reasoning

Based on the Affinity Diagram, users need immediate and clear feedback after practice.

Because of this, the Result Screen appears directly after the Practice Screen.

Based on the UX Research assumptions, users may not know which notes they need to review. Therefore, Weak Notes are shown on the Result Screen.

The result is also presented in a supportive way, because the persona may feel discouraged after mistakes.

### Purpose

The purpose of this screen is to give feedback, reduce confusion, and help the user understand what to review next.

---

## 5. Progress Screen

The Progress Screen helps the user understand improvement over time.

### Content

* Practice streak
* Average accuracy
* Total practice time
* Weekly accuracy chart
* Weak notes
* Recommended practice
* Bottom navigation

### UX Reasoning

Based on the Persona and Affinity Diagram, seeing progress can motivate beginner users to continue practicing.

Because of this, Progress is separated into its own screen.

The screen includes streak, accuracy, weekly chart, weak notes, and recommended practice because these elements help the user understand both improvement and next steps.

### Purpose

The purpose of this screen is to motivate the user and show learning progress clearly.

---

## Navigation Structure

NoteFlow uses a simple navigation structure.

### Main Flow

```text
Welcome → Home → Practice → Result → Progress
```

### Bottom Navigation

The Bottom Navigation includes:

* Home
* Practice
* Progress

### UX Reasoning

Based on UX Foundations, beginner users need a simple and predictable navigation system.

Because of this, the bottom navigation is limited to the most important areas of the app.

Result is not included in the Bottom Navigation because it appears only after a practice session.

---

## IA Design Decisions

### 1. Today’s Practice is placed on the Home Screen

Based on the UX Research assumptions, beginner music students need short and achievable practice sessions.

Because of this, the Home Screen highlights Today’s Practice as the main action. This helps the user quickly understand where to start.

---

### 2. Practice is focused on one task at a time

Based on the Proto-Persona, the beginner user may feel confused or stressed if the interface shows too much information at once.

Because of this, the Practice Screen focuses on one note question, one music staff area, and clear answer options.

---

### 3. Result appears immediately after Practice

Based on the Affinity Diagram, users need clear and immediate feedback.

Because of this, the Result Screen comes right after the Practice Screen. It shows score, accuracy, weak notes, and encouraging feedback.

---

### 4. Weak Notes are shown after practice

Based on the UX Research assumptions, users may not know which notes they need to review.

Because of this, Weak Notes are included in both the Result Screen and Progress Screen. This helps users understand what to practice next.

---

### 5. Progress has a separate screen

Based on the Persona and Affinity Diagram, seeing improvement can motivate beginner users.

Because of this, Progress is separated into its own screen with practice streak, average accuracy, weekly chart, weak notes, and recommended practice.

---

### 6. Navigation is kept simple

Based on UX Foundations, the app should be easy to understand for beginner users.

Because of this, the main navigation is limited to the most important areas: Home, Practice, and Progress.

---

## Content Priority

The most important content is placed first on each screen.

### Home Screen

Priority:

1. Start practice
2. Quick actions
3. Progress preview

This supports the research insight that users need a short and easy way to begin practice.

### Practice Screen

Priority:

1. Question
2. Music note
3. Answer options
4. Next action

This supports the persona need for a simple and focused practice experience.

### Result Screen

Priority:

1. Score and accuracy
2. Weak notes
3. Next actions

This supports the affinity diagram insight that users need feedback and review guidance.

### Progress Screen

Priority:

1. Main stats
2. Weekly progress
3. Weak notes
4. Recommended practice

This supports the research insight that users may stay motivated when they can see progress.

---

## Summary

The information architecture of NoteFlow is designed to keep the experience clear and easy for beginner music students.

The app structure is based on previous UX steps, including UX Research, Affinity Diagram, Persona, and User Flow.

The main IA goal is to support a simple learning journey:

The user starts practice, answers questions, receives feedback, and checks progress.

This organization helps reduce confusion and keeps the app focused on the user’s main goal: improving note recognition.

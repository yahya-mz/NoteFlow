# Accessibility and Usability

## Overview

Accessibility and usability are important parts of the NoteFlow design because the app is made for beginner music students.

The goal is not only to make the interface visually nice, but also to make it easy to understand, easy to use, and supportive for users who may feel confused or stressed while learning note reading.

---

## UX Sources Used

The accessibility and usability decisions were shaped by previous UX steps:

* UX Foundations
* UX Research
* Affinity Diagram
* Proto-Persona
* User Flow
* Information Architecture
* Wireframes
* Design System
* Prototype

These steps showed that beginner music students need:

* Clear instructions
* Short and simple practice
* Easy-to-tap answer options
* Immediate feedback
* A calm interface
* Visible progress
* Support after mistakes

Because of these findings, the design focuses on clarity, readability, simple navigation, and supportive feedback.

---

## Usability Goals

The main usability goals of NoteFlow are:

1. The user should quickly understand what the app does.
2. The user should easily find the Start Practice action.
3. The user should understand how to answer a note question.
4. The user should clearly understand the result after practice.
5. The user should know which notes to review.
6. The user should be able to check progress without confusion.
7. The app should feel simple and beginner-friendly.

---

## Research-Based Usability Decisions

| UX Finding                                       | Source                        | Usability Decision                                      |
| ------------------------------------------------ | ----------------------------- | ------------------------------------------------------- |
| Beginner users need a clear starting point.      | UX Foundations, Persona       | Make Start Practice visually clear on Welcome and Home. |
| Users prefer short and simple practice.          | UX Research, Affinity Diagram | Keep the practice flow short and focused.               |
| Users may feel confused by too much information. | Persona                       | Show one note question at a time.                       |
| Users need feedback after practice.              | Affinity Diagram              | Show Result Screen immediately after Practice.          |
| Users want to know what to review.               | UX Research                   | Show Weak Notes after practice.                         |
| Progress can motivate users.                     | Persona, Affinity Diagram     | Use progress stats, weekly chart, and accuracy.         |
| Mobile users need easy interaction.              | Mobile Design                 | Use large buttons and clear answer options.             |

---

## Usability Considerations

## 1. Clear Main Action

The most important action on the Home Screen is Start Practice.

### Design Reasoning

Based on UX Research, beginner users need short and achievable practice.

Because of this, Start Practice is shown as the main call-to-action so users can begin quickly without searching through the interface.

---

## 2. One Task at a Time

The Practice Screen focuses on one note question at a time.

### Design Reasoning

Based on the Proto-Persona, the user may feel confused or stressed if too much information appears at once.

Because of this, the screen includes only the current question, music staff, answer options, and next action.

---

## 3. Simple Navigation

The app uses simple navigation between Home, Practice, and Progress.

### Design Reasoning

Based on Information Architecture, the main sections should be easy to understand and easy to reach.

Because of this, the Bottom Navigation includes only the most important destinations:

* Home
* Practice
* Progress

The Result Screen is not placed in the Bottom Navigation because it appears only after a practice session.

---

## 4. Clear Feedback

The user needs to understand whether an answer is correct or wrong.

### Design Reasoning

Based on the Affinity Diagram, users need immediate and supportive feedback.

Because of this, Answer Option components include different states:

* Default
* Selected
* Correct
* Wrong
* Disabled

This helps users understand what happened after they choose an answer.

---

## 5. Result Screen After Practice

The Result Screen appears after the Practice Screen.

### Design Reasoning

Based on UX Research and the Affinity Diagram, users need feedback after completing practice.

Because of this, the Result Screen shows:

* Score
* Accuracy
* Weak notes
* Encouraging message
* Practice Again action
* View Progress action

This helps the user understand both performance and next steps.

---

## 6. Weak Notes

Weak notes are shown on the Result and Progress screens.

### Design Reasoning

Based on UX Research, users may not know which notes they should review.

Because of this, Weak Notes help users understand what to practice next.

---

## Accessibility Goals

The accessibility goals of NoteFlow are:

1. Text should be readable.
2. Buttons should be easy to tap.
3. Feedback should not rely only on color.
4. Progress should be shown visually and numerically.
5. The interface should have clear visual hierarchy.
6. Navigation should be simple and predictable.
7. The app should avoid unnecessary visual complexity.

---

## Accessibility Considerations

## 1. Readable Text

Text should be clear and readable on mobile screens.

### Design Decision

The design uses clear typography roles:

* Screen titles
* Section titles
* Body text
* Button text
* Small labels

This helps users scan the screen and understand content quickly.

---

## 2. Touch-Friendly Buttons

Mobile users need buttons that are easy to tap.

### Design Decision

Primary actions and answer options are designed as large tappable elements.

This supports mobile usability and reduces mistakes when selecting answers.

---

## 3. Feedback Should Not Rely Only on Color

Correct and wrong answers should not be communicated only through green and red colors.

### Design Decision

The design uses color for feedback states, but in a future version, the feedback should also include icons or text labels.

For example:

* Correct answer: green color + check icon + "Correct"
* Wrong answer: red color + x icon + "Try again"

This makes feedback clearer and more accessible.

---

## 4. Progress Shown with Numbers

Progress should not be shown only through a visual chart or ring.

### Design Decision

The Progress Ring should also display a percentage number, such as 80%.

This helps users understand their performance more clearly.

---

## 5. Clear Visual Hierarchy

Important information should be visually prioritized.

### Design Decision

The design uses hierarchy to make important content easier to notice.

Examples:

* Start Practice is the main action on Home.
* The question is clear on Practice.
* Accuracy is central on Result.
* Progress stats are placed near the top of Progress.

---

## 6. Calm Visual Style

The app should not feel stressful or overwhelming.

### Design Decision

Based on the Persona, NoteFlow uses:

* Soft colors
* Rounded cards
* Light shadows
* Clean spacing
* Simple layouts

This helps the product feel more supportive and beginner-friendly.

---

## Usability Testing Plan

This project has not completed full usability testing yet.

In a future version, I would test the Figma prototype with 2–3 beginner music students.

## Test Tasks

Users would be asked to:

1. Open the app and explain what they think it does.
2. Find the Start Practice button.
3. Start a practice session.
4. Select an answer.
5. Understand the Result Screen.
6. Find weak notes.
7. Open the Progress Screen.
8. Explain what they should practice next.

---

## Success Criteria

The design would be considered usable if users can:

* Understand the app purpose quickly
* Start practice without help
* Select an answer easily
* Understand correct or wrong feedback
* Understand their score and accuracy
* Find weak notes
* Navigate to Progress
* Know what to do next

---

## Possible Improvements After Testing

Based on usability testing, I might improve:

* Button labels
* Feedback messages
* Answer option states
* Progress visualization
* Weak note explanation
* Navigation clarity
* Text size and contrast
* Touch target spacing

---

## Limitations

This accessibility and usability review is an early-stage evaluation.

The current version includes basic accessibility and usability considerations, but it has not yet been tested with real users.

In a future version, I would perform:

* Color contrast checks
* Mobile touch target checks
* Usability testing
* Accessibility review for feedback states
* Iteration based on user feedback

---

## Summary

The usability and accessibility decisions in NoteFlow are based on the needs of beginner music students.

The design focuses on:

* Simple practice
* Clear navigation
* Readable content
* Large tappable elements
* Supportive feedback
* Weak note review
* Visible progress
* Calm visual style

These decisions help make NoteFlow easier to use, more beginner-friendly, and more prepared for future usability testing.

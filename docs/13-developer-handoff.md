# Developer Handoff

## Overview

Developer handoff is the process of preparing the design so frontend developers can understand and implement it correctly.

For NoteFlow, the developer handoff explains the screens, components, design tokens, component states, assets, and dynamic behavior needed to turn the Figma design into a real mobile app.

The goal is to reduce guesswork during implementation.

---

## UX Sources Used for Developer Handoff

The developer handoff is based on previous UX and UI documents:

* UX Foundations
* Design Thinking
* UX Research
* Affinity Diagram
* Proto-Persona
* User Flow
* Information Architecture
* Wireframes
* Design System
* Prototype
* Accessibility and Usability
* AI-Assisted Design

These documents explain why each screen, component, and interaction exists.

Because of this, the handoff is not only about visual design. It also explains how the design supports the user’s needs.

---

## Handoff Exports

The following exports support the developer handoff:

### Final Screens

![Welcome Screen](../assets/welcome-screen.png)

![Home Screen](../assets/home-screen.png)

![Practice Screen](../assets/practice-screen.png)

![Result Screen](../assets/result-screen.png)

![Progress Screen](../assets/progress-screen.png)

### Design System

![Design Tokens](../exports/design-tokens.png)

![Components](../exports/components.png)

### Prototype Flow

![Prototype Flow](../exports/prototype-flow.png)

---

## Main Screens

The app includes five main screens:

1. Welcome Screen
2. Home Screen
3. Practice Screen
4. Result Screen
5. Progress Screen

---

## Screen Implementation Notes

## 1. Welcome Screen

### Purpose

The Welcome Screen introduces the app and gives the user a clear starting point.

### Main Elements

* App name
* Short description
* Music-related visual
* Start Practice button
* View Progress button

### Developer Notes

* `Start Practice` should move the user into the main practice flow.
* `View Progress` should navigate to the Progress Screen.
* The screen should remain visually simple and centered.

### UX Reasoning

Based on UX Foundations, the user should quickly understand what the app does and what action to take first.

---

## 2. Home Screen

### Purpose

The Home Screen acts as the main dashboard and helps the user quickly start practice.

### Main Elements

* Greeting
* Today’s Practice card
* Quick Action cards
* Progress preview
* Bottom Navigation

### Developer Notes

* `Start Practice` should navigate to the Practice Screen.
* Quick Actions can later link to Flashcards, Weak Notes, or Progress.
* Progress preview should use user progress data when backend data is available.

### UX Reasoning

Based on UX Research and the Affinity Diagram, beginner users need short and simple practice.

Because of this, Today’s Practice is the main action on the Home Screen.

---

## 3. Practice Screen

### Purpose

The Practice Screen lets the user answer one note-reading question at a time.

### Main Elements

* Question number
* Progress bar
* Question text
* Music staff area
* Note visual
* Answer options
* Next button
* Bottom Navigation

### Developer Notes

The Practice Screen should manage:

* Current question index
* Selected answer
* Correct answer
* Answer state
* Score
* Weak notes
* Practice progress

### Possible State Variables

```text
currentQuestion
selectedAnswer
correctAnswer
score
weakNotes
questionIndex
totalQuestions
isAnswerSelected
```

### UX Reasoning

Based on the Proto-Persona, beginner users may feel confused if too much information appears at once.

Because of this, the Practice Screen focuses on one note question at a time.

---

## 4. Result Screen

### Purpose

The Result Screen gives feedback after a practice session.

### Main Elements

* Encouraging message
* Score
* Accuracy percentage
* Progress Ring
* Weak Notes
* Practice Again button
* View Progress button

### Developer Notes

The Result Screen should receive or calculate:

* Total questions
* Correct answers
* Accuracy percentage
* Weak notes
* Practice session summary

### Accuracy Rule

```text
accuracy = correctAnswers / totalQuestions * 100
```

Example:

```text
correctAnswers = 8
totalQuestions = 10
accuracy = 80%
```

### UX Reasoning

Based on the Affinity Diagram, users need immediate and supportive feedback after practice.

Because of this, Result appears directly after Practice and shows score, accuracy, weak notes, and next actions.

---

## 5. Progress Screen

### Purpose

The Progress Screen helps the user understand improvement over time.

### Main Elements

* Practice streak
* Average accuracy
* Total practice time
* Weekly accuracy chart
* Weak notes
* Recommended practice
* Bottom Navigation

### Developer Notes

The Progress Screen should display saved user progress when backend data is available.

Possible data:

```text
practiceStreak
averageAccuracy
totalPracticeTime
weeklyAccuracy
weakNotes
recommendedPractice
```

### UX Reasoning

Based on the Persona and Affinity Diagram, seeing progress can motivate beginner users to continue practicing.

Because of this, Progress is a dedicated screen.

---

## Reusable Components

The design should be implemented using reusable frontend components.

## 1. Button

### Types

* Primary Button
* Secondary Button
* Small Button

### States

* Default
* Pressed
* Disabled

### Usage

Used for actions such as:

* Start Practice
* Next
* Practice Again
* View Progress
* Start Review

### Developer Notes

The Button component should support:

```text
label
type
state
onClick
disabled
```

---

## 2. Card

### Types

* Practice Card
* Quick Action Card
* Progress Card
* Result Card
* Stat Card

### Usage

Cards group related content and create clear sections.

### Developer Notes

The Card component should support:

```text
title
description
icon
children
onClick
```

---

## 3. Answer Option

### States

* Default
* Selected
* Correct
* Wrong
* Disabled

### Usage

Used on the Practice Screen for multiple-choice answers.

### Developer Notes

The Answer Option component should support:

```text
label
state
isSelected
isCorrect
onClick
disabled
```

### Behavior

* Before selection, options are in Default state.
* When the user selects an option, it becomes Selected.
* If the answer is correct, show Correct state.
* If the answer is wrong, show Wrong state.
* After answer validation, other options may become Disabled.

### Accessibility Note

Feedback should not rely only on color.

In a future version, correct and wrong states should also include icons or text labels.

---

## 4. Bottom Navigation

### Items

* Home
* Practice
* Progress

### States

* Default
* Active

### Developer Notes

The Bottom Navigation should support:

```text
activeTab
onNavigate
items
```

### Behavior

The active item should match the current screen.

The Result Screen is not included in Bottom Navigation because it appears only after a practice session.

---

## 5. Progress Ring

### Usage

Used to show accuracy or completion percentage.

### Developer Notes

The Progress Ring should be a dynamic component.

It should receive:

```text
value
label
```

Example:

```text
value = 80
label = "80%"
```

### Behavior

* The ring fill should represent the value from 0 to 100.
* The center text should display the percentage number.
* The component should not be only decorative; the number must be visible.

---

## 6. Weekly Chart

### Usage

Used on the Progress Screen to show weekly accuracy.

### Developer Notes

The Weekly Chart should receive data such as:

```text
weeklyAccuracy = [
  { day: "Sat", accuracy: 60 },
  { day: "Sun", accuracy: 72 },
  { day: "Mon", accuracy: 80 }
]
```

### Behavior

* Each bar should represent accuracy for one day.
* The chart should remain simple and readable on mobile.

---

## 7. Weak Note Chip

### Usage

Used to show notes that the user should review.

Example:

```text
F
B
G
```

### Developer Notes

The component should receive:

```text
noteName
```

Weak Note Chips can appear on:

* Result Screen
* Progress Screen

---

## Design Tokens for Frontend

Design tokens should be converted into frontend variables or theme values.

Examples:

```text
colorPrimary
colorPrimaryLight
colorBackground
colorSurface
colorTextPrimary
colorTextSecondary
colorSuccess
colorError
radiusSmall
radiusMedium
radiusLarge
radiusFull
shadowCard
shadowButton
spacingSmall
spacingMedium
spacingLarge
```

These values should be reused across components to keep the UI consistent.

---

## Dynamic Behavior

## 1. Practice Logic

The app should show one question at a time.

Basic flow:

```text
Show question
↓
User selects answer
↓
Validate answer
↓
Update score and weak notes
↓
Move to next question
↓
Show result after final question
```

---

## 2. Accuracy Calculation

Accuracy should be calculated from correct answers and total questions.

```text
accuracy = correctAnswers / totalQuestions * 100
```

The result should be displayed on the Result Screen and used in the Progress Ring.

---

## 3. Weak Notes

If a user answers a note incorrectly, that note can be added to the weak notes list.

Example:

```text
weakNotes = ["F", "B"]
```

Weak notes should appear on:

* Result Screen
* Progress Screen

---

## 4. Practice Again

When the user taps Practice Again:

```text
Practice Again → Practice Screen
```

The app can either restart the same question set or generate a new short session.

---

## 5. View Progress

When the user taps View Progress:

```text
View Progress → Progress Screen
```

The user should see updated progress data after completing practice.

---

## Assets

Assets should be exported from Figma when needed.

Recommended asset types:

* SVG for icons
* PNG for screen previews
* SVG or vector format for music icons when possible

Possible assets:

```text
music-note-icon.svg
treble-clef-icon.svg
home-icon.svg
practice-icon.svg
progress-icon.svg
```

---

## Accessibility Notes for Developers

Developers should consider:

* Buttons should be large enough for mobile tapping.
* Text should remain readable on small screens.
* Correct and wrong feedback should not rely only on color.
* Progress should be shown with both visual and numeric information.
* Navigation should be simple and predictable.
* Interactive elements should have clear labels.

---

## Future Backend Considerations

If NoteFlow becomes a real product, backend support may include:

* User account
* Saved practice sessions
* Question database
* User progress history
* Weak notes history
* Streak tracking
* Analytics events

Possible analytics events:

```text
Start Practice Clicked
Answer Selected
Practice Completed
View Progress Clicked
Practice Again Clicked
Weak Notes Opened
```

---

## Handoff Summary

The developer handoff provides the main information needed to implement NoteFlow:

* Screens
* User flow
* Components
* Component states
* Design tokens
* Dynamic behavior
* Assets
* Accessibility notes
* Future backend considerations

The goal is to make the design easier to understand, easier to implement, and more consistent with the UX decisions made earlier in the project.

---

## Summary

The NoteFlow developer handoff connects the design process to future frontend implementation.

It explains not only what should be built, but also why each part exists.

The handoff is based on the UX research assumptions, affinity diagram, persona, user flow, information architecture, wireframes, design system, prototype, and accessibility review.

This makes the project more organized and easier to continue as a real product.

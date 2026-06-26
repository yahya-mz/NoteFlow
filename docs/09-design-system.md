# Design System

## Overview

A design system is a collection of reusable design decisions, styles, components, and rules that help keep the product consistent.

For NoteFlow, a small design system was created to make the mobile app feel consistent, clear, and beginner-friendly.

The design system includes:

* Design tokens
* Colors
* Typography
* Spacing
* Radius
* Shadows
* UI elements
* Reusable components
* Component states
* Mobile design rules
* Basic Gestalt principles

---
## Design System Exports

The NoteFlow design system is divided into two main parts:

1. Design Tokens
2. Components

### Design Tokens

Design tokens include the core visual values used across the app, such as colors, typography, spacing, radius, and shadows.

![Design Tokens](../exports/design-tokens.png)

### Components

Components include reusable UI elements such as buttons, cards, answer options, bottom navigation, progress ring, weak note chips, and other repeated interface elements.

![Components](../exports/components.png)

---

## UX Sources Used for the Design System

The design system was shaped by previous UX steps:

* UX Foundations
* UX Research
* Affinity Diagram
* Proto-Persona
* User Flow
* Information Architecture
* Wireframes

These steps showed that beginner music students need:

* A calm and simple interface
* Clear visual hierarchy
* Short and focused practice
* Easy-to-tap answer options
* Clear feedback for correct and wrong answers
* Visible progress
* Consistent navigation

Because of these findings, the design system focuses on clarity, consistency, accessibility, and beginner-friendly visual design.

---

## Research-Based Design Decisions

| UX Finding                                              | Source                        | Design System Decision                                              |
| ------------------------------------------------------- | ----------------------------- | ------------------------------------------------------------------- |
| Beginner users may feel stressed by complex interfaces. | Persona, UX Research          | Use a calm visual style with soft colors and rounded cards.         |
| Users need short and simple practice.                   | Affinity Diagram              | Keep components simple and focused on one action at a time.         |
| Users need clear feedback after answering.              | Affinity Diagram, UX Research | Create Answer Option states: Default, Selected, Correct, and Wrong. |
| Users need easy mobile interaction.                     | Mobile Design, UX Foundations | Use large touch-friendly buttons and answer options.                |
| Users need visible progress.                            | Persona, Affinity Diagram     | Create progress components such as Progress Ring and Weekly Chart.  |
| Users need simple navigation.                           | Information Architecture      | Use a consistent Bottom Navigation component.                       |
| The interface should feel supportive, not stressful.    | Persona                       | Use friendly microcopy, soft shadows, and calm spacing.             |

---

## Visual Style

The visual style of NoteFlow is:

* Calm
* Educational
* Beginner-friendly
* Soft
* Simple
* Clean
* Not childish
* Not overdesigned

The goal is to make the app feel like a helpful learning tool, not a stressful exam.

---

## Design Tokens

Design tokens are the basic visual values used across the product.

They help keep the UI consistent and easier to implement in frontend development.

---

## Colors

### Primary Colors

| Token                 | Purpose                                           |
| --------------------- | ------------------------------------------------- |
| `color/primary`       | Main actions, active states, important highlights |
| `color/primary-light` | Soft background for selected or highlighted areas |
| `color/background`    | Main app background                               |
| `color/surface`       | Cards and elevated sections                       |

### Text Colors

| Token                  | Purpose                          |
| ---------------------- | -------------------------------- |
| `color/text-primary`   | Main headings and important text |
| `color/text-secondary` | Supporting text and descriptions |

### Feedback Colors

| Token           | Purpose                                    |
| --------------- | ------------------------------------------ |
| `color/success` | Correct answers and positive feedback      |
| `color/error`   | Wrong answers and error feedback           |
| `color/accent`  | Small highlights and motivational elements |

### Design Reasoning

Based on the persona, the app should feel calm and supportive.

Because of this, the color palette uses a soft background, white cards, and purple as the main action color.

Success and error colors are used only for feedback states, so the user can clearly understand correct and wrong answers.

---

## Typography

Typography is used to create clear hierarchy and improve readability.

### Typography Roles

| Role          | Purpose                                                     |
| ------------- | ----------------------------------------------------------- |
| App Title     | Main brand name on Welcome Screen                           |
| Screen Title  | Main title of each screen                                   |
| Section Title | Section headers such as Today’s Practice or Weekly Accuracy |
| Body Text     | Descriptions and supportive text                            |
| Button Text   | Main actions                                                |
| Small Label   | Small details such as question count or note labels         |

### Design Reasoning

Based on UX Foundations, beginner users should quickly understand each screen.

Because of this, typography is organized with clear hierarchy:

* Larger titles for main screen purpose
* Medium section titles for content groups
* Smaller body text for descriptions
* Strong button text for actions

---

## Spacing

Spacing helps the interface feel clean and readable.

The design uses consistent spacing between:

* Sections
* Cards
* Buttons
* Text blocks
* Answer options
* Navigation items

### Design Reasoning

Based on the Proto-Persona, beginner users may feel overwhelmed by cluttered screens.

Because of this, the design uses enough spacing to separate sections clearly and reduce visual stress.

---

## Radius

Rounded corners are used across the interface.

### Radius Usage

| Element           | Radius Style               |
| ----------------- | -------------------------- |
| Cards             | Large rounded corners      |
| Buttons           | Full or pill-shaped radius |
| Answer Options    | Medium rounded corners     |
| Chips             | Pill-shaped radius         |
| Progress elements | Rounded shapes             |

### Design Reasoning

Rounded shapes help the app feel softer and more beginner-friendly.

This supports the goal of making NoteFlow feel calm and encouraging instead of strict or exam-like.

---

## Shadows

Soft shadows are used to separate cards from the background.

### Shadow Usage

| Element            | Shadow Purpose            |
| ------------------ | ------------------------- |
| Cards              | Create soft elevation     |
| Buttons            | Show interactive priority |
| Main practice card | Highlight the main action |

### Design Reasoning

The shadows are kept subtle because the app should feel clean and calm.

The goal is to create visual separation without making the UI look heavy.

---

## UI Elements

The main UI elements in NoteFlow include:

* Buttons
* Cards
* Answer options
* Bottom navigation
* Progress ring
* Weekly chart
* Weak note chips
* Music staff area
* Practice progress bar
* Icons

Each element supports a specific part of the user journey.

---

## Components

Reusable components help keep the interface consistent across screens.

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

Buttons are used for main actions such as:

* Start Practice
* Next
* Practice Again
* View Progress
* Start Review

### UX Reasoning

Based on UX Foundations, the user should quickly understand what action to take.

Because of this, the Primary Button is used for the most important action on each screen.

---

## 2. Card

### Types

* Practice Card
* Quick Action Card
* Progress Card
* Result Card
* Stat Card

### Usage

Cards are used to group related information.

### UX Reasoning

Based on Gestalt’s Common Region principle, related content is easier to understand when placed inside the same visual container.

Because of this, cards are used to group practice details, progress stats, and quick actions.

---

## 3. Answer Option

### States

* Default
* Selected
* Correct
* Wrong
* Disabled

### Usage

Answer options are used on the Practice Screen for multiple-choice note recognition.

### UX Reasoning

Based on the Affinity Diagram, users need immediate and clear feedback.

Because of this, Answer Option states are designed to show the user what they selected and whether the answer is correct or wrong.

Feedback should not rely only on color. In a future version, icons or text labels can also be added for accessibility.

---

## 4. Bottom Navigation

### Items

* Home
* Practice
* Progress

### States

* Default
* Active

### UX Reasoning

Based on Information Architecture, the app needs simple navigation between the main sections.

Because of this, the Bottom Navigation includes only the most important areas.

The Result Screen is not included because it appears only after completing a practice session.

---

## 5. Progress Ring

### Usage

The Progress Ring is used to show accuracy or completion percentage.

### Dynamic Rule

The Progress Ring should receive a value from 0 to 100.

Example:

If the user answers 8 out of 10 questions correctly, the accuracy is 80%.

The ring should visually represent this value and also show the number as text.

### UX Reasoning

Based on the Persona and Affinity Diagram, seeing progress can motivate beginner users.

Because of this, progress is shown visually and numerically.

---

## 6. Weekly Chart

### Usage

The Weekly Chart is used on the Progress Screen to show accuracy over time.

### UX Reasoning

Based on UX Research, users may feel more motivated when they can see improvement.

Because of this, the Progress Screen includes a simple weekly chart.

The chart should be easy to understand and not visually overwhelming.

---

## 7. Weak Note Chip

### Usage

Weak note chips show notes that the user should review.

Examples:

* F
* B
* G

### UX Reasoning

Based on the UX Research assumptions, users may not know which notes they need to review.

Because of this, Weak Notes are shown as small chips on the Result and Progress screens.

This helps the user understand the next learning step.

---

## Component Hierarchy

The design system is organized from small decisions to full screens.

```text
Design Tokens
      ↓
Base Components
      ↓
Composite Components
      ↓
Screen Sections
      ↓
Full Screens
```

### Example

```text
color/primary
      ↓
Primary Button
      ↓
Today’s Practice Card
      ↓
Home Screen
```

This structure helps keep the design consistent and easier to hand off to frontend development.

---

## UI Design Principles Used

## 1. Visual Hierarchy

Important information is made more visible.

Examples:

* Start Practice is the main action on Home.
* Accuracy is visually important on Result.
* Progress stats are placed near the top of Progress.

## 2. Consistency

Repeated elements use the same style.

Examples:

* Buttons follow the same shape and typography.
* Cards use similar radius and shadow.
* Navigation items follow the same structure.

## 3. Contrast

Important actions use stronger visual contrast.

Examples:

* Primary buttons use the main purple color.
* Text uses clear dark colors on light backgrounds.

## 4. Alignment

Elements are aligned consistently to make screens easier to scan.

## 5. Spacing

Spacing is used to separate sections and reduce visual clutter.

---

## Gestalt Principles Used

## 1. Proximity

Related elements are placed close together.

Example:

The question, music staff, and answer options are grouped together on the Practice Screen.

## 2. Similarity

Elements with similar functions look similar.

Example:

All answer options have the same shape and style.

## 3. Common Region

Related content is placed inside the same card or section.

Example:

Today’s Practice content is placed inside one card.

## 4. Visual Hierarchy

Important actions and information are visually prioritized.

Example:

The Start Practice button is more visually prominent than secondary actions.

---

## Mobile Design Considerations

NoteFlow is designed as a mobile app, so the design system considers mobile usability.

### Mobile Rules

* Buttons should be easy to tap.
* Answer options should have enough spacing.
* The layout should be vertical and easy to scan.
* Navigation should stay simple.
* Each screen should focus on one main task.
* Text should be readable on a small screen.

### Design Reasoning

Based on UX Foundations, the user should not feel confused while using the app on mobile.

Because of this, the design uses a simple vertical layout, large touch targets, and clear screen structure.

---

## Figma Usage

The design system was created in Figma using:

* Frames
* Auto Layout
* Components
* Variants
* Instances
* Assets
* Prototype connections

Reusable components were created to make the design easier to update and more consistent.

---

## Connection to Developer Handoff

The design system supports developer handoff by defining:

* Reusable components
* Component states
* Visual tokens
* Dynamic UI behavior
* Layout rules
* Assets

This makes it easier for frontend developers to understand how the design should be implemented.

---

## Summary

The NoteFlow design system translates UX findings into consistent visual and interactive patterns.

It supports:

* Calm visual style
* Clear hierarchy
* Simple mobile interaction
* Reusable components
* Feedback states
* Progress visualization
* Beginner-friendly learning experience

The design system helps make NoteFlow more consistent, scalable, and easier to explain as a UX/UI case study.

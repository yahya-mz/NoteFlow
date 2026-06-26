# Affinity Diagram

## Overview

An affinity diagram is used to organize research notes into meaningful groups and turn scattered user needs into clear design insights.

For NoteFlow, this affinity diagram is based on proto-research and assumption-based UX analysis. Since full user interviews have not been completed yet, the notes below represent possible needs, pain points, and expectations of beginner music students.

The goal of this document is to connect research assumptions to actual product decisions.

---

## Research Context

Based on the UX Research document, the main research goal was to understand what beginner music students may need when practicing note reading.

The research assumptions suggested that beginner users may:

* Recognize notes slowly
* Feel bored by long exercises
* Need clear feedback
* Feel discouraged after mistakes
* Stay motivated when they can see progress

The affinity diagram organizes these assumptions into four main groups.

---

## Research Notes

Possible user statements:

* I recognize notes slowly.
* I sometimes confuse notes on the staff.
* Some notes look very similar to me.
* Long exercises feel boring.
* I prefer short daily practice.
* I want to know immediately if my answer is correct.
* I feel discouraged when I make mistakes.
* I want feedback that helps me improve.
* Seeing my progress would motivate me.
* I want to know which notes I should review.
* A simple app would make practice easier.
* I do not want the app to feel like a stressful exam.

---

## Affinity Groups

## Group 1: Note Recognition Problems

### Related Notes

* I recognize notes slowly.
* I sometimes confuse notes on the staff.
* Some notes look very similar to me.

### Insight

Beginner music students may need focused and simple note-recognition practice. Since they are still learning, showing too many tasks at once may make the experience confusing.

### Design Decision

Because of this insight, NoteFlow includes a Practice Screen that focuses on one note question at a time.

The question is supported by:

* A music staff area
* One note visual
* Multiple-choice answer options
* A simple next action

This helps keep the practice experience focused and beginner-friendly.

---

## Group 2: Need for Short and Simple Practice

### Related Notes

* Long exercises feel boring.
* I prefer short daily practice.
* A simple app would make practice easier.

### Insight

Beginners may be more likely to continue practicing if the session feels short, simple, and achievable.

### Design Decision

Because of this insight, NoteFlow uses a short practice model, such as a 5-minute note-reading exercise.

This decision affects the Home Screen and Practice Screen:

* The Home Screen highlights Today’s Practice as the main action.
* The Practice Screen keeps the task focused and limited.
* The app avoids unnecessary complexity in the main flow.

---

## Group 3: Need for Clear and Supportive Feedback

### Related Notes

* I want to know immediately if my answer is correct.
* I feel discouraged when I make mistakes.
* I want feedback that helps me improve.

### Insight

Feedback should be immediate, clear, and supportive. Wrong answers should help the user learn instead of making the experience feel stressful.

### Design Decision

Because of this insight, NoteFlow includes answer states and a Result Screen.

Answer Option states include:

* Default
* Selected
* Correct
* Wrong

The Result Screen also shows:

* Score
* Accuracy
* Weak notes
* Encouraging message
* Practice Again action
* View Progress action

This helps users understand both their performance and their next step.

---

## Group 4: Motivation and Progress

### Related Notes

* Seeing my progress would motivate me.
* I want to know which notes I should review.
* I do not want the app to feel like a stressful exam.

### Insight

Progress tracking can motivate beginner users, but it should feel encouraging rather than stressful. Users also need to understand what they should review next.

### Design Decision

Because of this insight, NoteFlow includes a dedicated Progress Screen.

The Progress Screen includes:

* Practice streak
* Average accuracy
* Total practice time
* Weekly accuracy chart
* Weak notes
* Recommended practice

Weak notes are also shown on the Result Screen so users can immediately understand which notes need more review.

---

## Final Insights

The affinity diagram helped organize the main user needs into four key areas:

1. Note recognition problems
2. Short and simple practice
3. Clear and supportive feedback
4. Motivation through progress tracking

These insights shaped the main structure of NoteFlow.

---

## Impact on Product Design

Based on the affinity groups, NoteFlow focuses on:

* Short note-reading exercises
* One question at a time
* Simple multiple-choice answers
* Instant feedback
* Correct and wrong answer states
* Weak note review
* Progress tracking
* Calm and beginner-friendly UI

---

## Connection to Other UX Documents

This affinity diagram supports later UX and UI decisions in the project.

### Connection to Information Architecture

The IA uses these insights to organize the app into:

* Home
* Practice
* Result
* Progress

For example, because users need short practice, Today’s Practice is placed on the Home Screen. Because users need feedback, the Result Screen comes after Practice.

### Connection to Persona

The proto-persona represents a beginner music student who needs short practice, clear feedback, and visible progress.

### Connection to Design System

The design system should support the same needs by using:

* Clear hierarchy
* Soft visual style
* Reusable answer option states
* Friendly feedback components
* Simple and consistent navigation

---

## Summary

The affinity diagram shows that beginner music students need more than practice questions. They need a simple, supportive, and motivating learning experience.

This helped shape NoteFlow as a mobile app focused on short practice, clear feedback, weak note review, and visible progress.

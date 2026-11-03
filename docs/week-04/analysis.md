
# Week 04 - Use Case and User Story

## 1. Project Overview
Pomodoro is a web-based time management application designed to help users manage focus sessions, breaks, and daily tasks.

## 2. Actor
- User: Interacts with the application to manage timers, tasks, settings, and focus statistics.

## 3. Use Cases
- UC-01: Manage Timer
- UC-02: Configure Focus and Break Durations
- UC-03: Manage Daily Tasks
- UC-04: Update Task Status
- UC-05: Manage Focus and Break Cycles
- UC-06: View Focus Statistics
- UC-07: Save and Restore Application Data

## 4. User Stories and Acceptance Criteria

### US-01: Start Timer
As a user, I want to start the timer so that I can begin a focus session.

Acceptance Criteria:
- The countdown starts when the user selects Start.
- The remaining time is displayed.
- Repeated clicks do not create multiple timers.

### US-02: Pause and Resume Timer
As a user, I want to pause and resume the timer so that I can manage temporary interruptions.

Acceptance Criteria:
- The countdown stops when Pause is selected.
- The remaining time is preserved.
- The timer continues from the saved remaining time after Resume.

### US-03: Reset Timer
As a user, I want to reset the timer so that I can restart a session.

Acceptance Criteria:
- The current countdown stops.
- The timer returns to its configured initial duration.
- The previous session is not counted as completed.

### US-04: Configure Session Duration
As a user, I want to configure focus and break durations so that the schedule matches my needs.

Acceptance Criteria:
- The user can enter focus and break durations.
- Valid positive values are accepted.
- Empty, zero, and negative values are rejected.
- The selected duration is applied to the next session.

### US-05: Manage Focus and Break Cycles
As a user, I want to see the next stage after a session ends so that I can follow the Pomodoro cycle.

Acceptance Criteria:
- The current stage is identified as focus or break.
- When the timer reaches zero, the current stage is marked as completed.
- The next stage is displayed.
- A completed stage is counted only once.

### US-06: Manage Tasks
As a user, I want to add, edit, and delete tasks so that I can organize my daily activities.

Acceptance Criteria:
- The user can add a task with a valid title.
- Empty task titles are rejected.
- Existing tasks can be edited.
- Deleted tasks are removed from the list.

### US-07: Update Task Status
As a user, I want to mark tasks as completed so that I can track my progress.

Acceptance Criteria:
- The user can mark a task as completed.
- The task status is visibly updated.
- The user can change a completed task back to pending.

### US-08: View Focus Statistics
As a user, I want to view completed focus sessions so that I can evaluate my productivity.

Acceptance Criteria:
- The number of completed focus sessions is displayed.
- Incomplete sessions are not counted.
- Each completed session is counted only once.

### US-09: Persist Application Data
As a user, I want my tasks and settings to remain saved after reloading the page so that I do not lose my information.

Acceptance Criteria:
- Tasks and settings are saved in browser storage.
- Saved information is restored after page reload.
- Default values are displayed when no saved data exists.

### US-10: View Current Session
As a user, I want to see the remaining time and current session status so that I know which stage I am in.

Acceptance Criteria:
- The remaining time is displayed clearly.
- The current stage is identified.
- The displayed information updates when the timer changes.

## 5. Scope Limitations
- No user authentication in the first version.
- No online database.
- No cross-device synchronization.
- No AI-based features.

## 6. Project Status
This document represents the analysis and design phase. Application implementation has not started yet.

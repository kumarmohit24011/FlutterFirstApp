# To-Do App Blueprint

## Overview

This document outlines the plan for creating a To-Do application for Android devices. The app will allow users to create, manage, and track their tasks.

## Features

*   **View Tasks:** Display a list of all tasks.
*   **Add Tasks:** Add new tasks to the list.
*   **Complete Tasks:** Mark tasks as completed.
*   **Delete Tasks:** Remove tasks from the list.

## Design and Style

The application will feature a modern and clean user interface, adhering to Material Design 3 principles. It will include:

*   **Color Scheme:** A color scheme generated from a seed color for a harmonious and accessible palette.
*   **Typography:** Consistent text styles using the `google_fonts` package.
*   **Component Theming:** Custom themes for components like `AppBar` and `ElevatedButton`.
*   **Dark/Light Mode:** Support for both light and dark themes with a theme toggle.

## Technical Plan

1.  **Project Setup:**
    *   Create a `blueprint.md` file to document the project.
    *   Add the `provider` and `google_fonts` packages to `pubspec.yaml`.

2.  **Theme and App Structure:**
    *   Create a `ThemeProvider` class to manage the application's theme.
    *   Define light and dark `ThemeData` using `ColorScheme.fromSeed` and `google_fonts`.
    *   Update `lib/main.dart` to use the `provider` package for theme management and set up the main application structure.

3.  **Task Management:**
    *   Create a `Task` model in `lib/models/task.dart`.
    *   Create a `TaskProvider` in `lib/providers/task_provider.dart` to manage the state of tasks.
    *   Implement the `HomeScreen` to display the list of tasks using a `ListView`.
    *   Create an `AddTaskScreen` to allow users to add new tasks.
    *   Implement `TaskList` and `TaskTile` widgets for displaying tasks.

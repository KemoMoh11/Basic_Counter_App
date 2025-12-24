#  Basic Counter App

A fundamental Flutter mobile application that demonstrates the core concepts of **Stateful Widgets** and **Local State Management**. This project serves as a perfect starting point for understanding how user interactions trigger UI updates in the Flutter framework.

---

## 📖 Project Overview

This application provides a clean, minimalist interface featuring a central counter. When the user interacts with the Floating Action Button (FAB), the application state is updated, and the UI reflects the new counter value immediately.

### Key Learning Objectives:
* Implementing a `StatefulWidget`.
* Using `setState()` to manage and update UI logic.
* Basic layout structure using `Scaffold`, `Center`, and `Column`.
* Applying Material 3 design principles.

---

## ✨ Features

* **Real-time Updates**: The counter increments instantly upon clicking the button.
* **Minimalist UI**: Focused on clarity and simplicity with no external dependencies.
* **Material 3 Ready**: Uses the latest Flutter design standards for a modern look.
* **Clean Code**: Fully documented `main.dart` following Dart best practices.

---

## 🚀 Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:
* [Flutter SDK](https://docs.flutter.dev/get-started/install)
* [Dart SDK](https://dart.dev/get-started/sdk)
* An Android/iOS emulator or a physical mobile device.

### Installation & Execution

1.  **Clone or Create the Project**:
    If you are starting fresh, create a new Flutter project:
    ```bash
    flutter create simple_counter_app
    cd simple_counter_app
    ```

2.  **Add the Code**:
    Replace the contents of `lib/main.dart` with the provided application code.

3.  **Run the App**:
    Execute the following command in your terminal:
    ```bash
    flutter run
    ```

---

## 🛠 Technical Explanation

### State Management
The heart of this application is the `setState()` method. In Flutter, widgets are immutable. To change what is on the screen, we use a `StatefulWidget` which maintains a `State` object.

```dart
void _incrementCounter() {
  setState(() {
    _counter++; 
  });
}
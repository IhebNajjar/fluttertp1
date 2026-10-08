# Waiting Room App — Workshop 1: UI Widgets, Lifecycle & Interactive Card

A Flutter application developed for **Workshop 1**, focusing on basic UI widgets, widget lifecycle (`StatefulWidget`), and periodic timers.

---

## 📌 Workshop 1 Overview

In this first workshop, the objective is to build an interactive waiting room greeting card displaying user info and a real-time running clock:

- **Greeting Card (`WaitingRoomCard`)**: Displays a customized greeting with the student's name (`Najjar Iheb`).
- **Interactive State**: Tapping the card highlights its background color to `Colors.lightBlueAccent` using `setState()`.
- **Live Clock (`WaitingRoomTimestamp`)**: Uses `Timer.periodic(const Duration(seconds: 1))` to update the displayed current time every second, properly disposing the timer in `dispose()`.

---

## 🏗️ Architecture

```
lib/
├── main.dart                  # App entry point, MaterialApp, and Scaffold
├── waiting_room_card.dart     # Interactive card widget with onTap color toggle
└── waiting_room_timestamp.dart# Real-time clock updated every second via Timer
test/
└── waiting_room_card_test.dart# Widget tests for card rendering and tap behavior
```

---

## 🧪 Tests

Run tests using:
```bash
flutter test
```

Tests verify:
- Displaying the greeting and name correctly.
- Background color highlighting upon tap.

---

## 🚀 How to Run

```bash
flutter pub get
flutter run -d chrome # or edge / windows
```

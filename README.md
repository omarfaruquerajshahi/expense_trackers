# Expense Tracker (Flutter + SQLite)

Module 10 Assignment — a simple expense tracker built with Flutter and SQLite (`sqflite`).

## Features
- **Home Screen**: app name, total expenses, ListView of all expenses (title + amount), FAB (+) to add, delete via IconButton.
- **Add Expense Screen**: form with Expense Title and Amount (numeric keyboard), Save Expense button.
  - Validation: no empty fields, amount must be greater than zero.
  - Saves to SQLite and returns to Home Screen.

## Database
Table `expenses`:

| Column | Type |
|--------|------|
| id | INTEGER PRIMARY KEY AUTOINCREMENT |
| title | TEXT |
| amount | REAL |

## Project structure
```
lib/
├── main.dart
├── models/expense.dart
├── db/database_helper.dart
└── screens/
    ├── home_screen.dart
    └── add_expense_screen.dart
```

## Run
```
flutter pub get
flutter run
```

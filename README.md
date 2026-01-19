# dev-habit

DevHabit is a mobile habit tracking application designed specifically for developers to build consistent learning and coding habits, track progress, and maintain long-term discipline.

---

##  Features
- User authentication (Firebase Authentication)
- Create and manage developer-focused habits
- Flexible habit frequency (daily / weekly / custom)
- Daily check-in & habit logs
- Streak tracking (current & longest streak)
- Reminder notifications
- Dashboard with basic statistics

---

##  Tech Stack
- **Flutter**
- **Dart**
- **Firebase Authentication**
- **Firebase Firestore**
- **State Management**: Riverpod / Provider
- **IDE**: VS Code

---

##  Database Design

### Users
- id (UUID)
- name
- email
- avatar_url
- timezone
- created_at
- last_login_at

### Habits
- id (UUID)
- user_id (FK → Users)
- title
- description
- category
- frequency_type (daily / weekly / custom)
- frequency_value
- reminder_time
- start_date
- end_date
- icon
- color
- created_at
- is_active

### Habit Logs
- id (UUID)
- habit_id (FK → Habits)
- log_date
- status (done / missed / skipped)
- note
- created_at

### Habit Streaks
- habit_id (FK → Habits)
- current_streak
- longest_streak
- last_completed_date
- updated_at

### Reminders
- id (UUID)
- habit_id (FK → Habits)
- time
- repeat_days
- is_enabled

### User Statistics
- user_id (FK → Users)
- total_habits
- total_completed
- completion_rate
- updated_at

---

##  Project Structure

```text
lib/
├── core/
│   ├── constants/
│   ├── utils/
│
├── features/
│   ├── auth/
│   │   ├── login_screen.dart
│   │   └── register_screen.dart
│   │
│   ├── habits/
│   │   ├── habit_model.dart
│   │   ├── habit_service.dart
│   │   └── habit_screen.dart
│   │
│   └── dashboard/
│       └── dashboard_screen.dart
│
├── widgets/
└── main.dart
```


##  Screenshots
> Updating...

##  Future Improvements
- Analytics & charts
- AI habit suggestion
- Cloud sync
- Dark mode

##  Author
Ngô Trần Nguyên Quân

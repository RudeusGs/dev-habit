# DevHabit 📱

DevHabit is a habit tracking mobile application designed specifically for developers to build consistent learning and coding habits.

## 🚀 Features
- User authentication (Firebase Auth)
- Create and manage daily coding habits
- Daily check-in system
- Streak tracking
- Habit history tracking
- Reminder notifications

## 🛠 Tech Stack
- Flutter
- Dart
- Firebase Authentication
- Firebase Firestore
- State Management: Riverpod / Provider

## 🗄 Database Design

### Users
- id
- name
- email
- created_at

### Habits
- id
- user_id
- title
- description
- frequency
- reminder_time
- created_at
- is_active

### Habit Logs
- id
- habit_id
- date
- status

## 📂 Project Structure
lib/
├── core/
├── features/
│   ├── auth/
│   ├── habits/
│   └── dashboard/
├── widgets/
└── main.dart

## 📸 Screenshots
> Updating...

## 🎯 Future Improvements
- Analytics & charts
- AI habit suggestion
- Cloud sync
- Dark mode

## 👨‍💻 Author
Ngô Trần Nguyên Quân

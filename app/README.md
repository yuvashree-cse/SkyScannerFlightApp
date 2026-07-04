✈️ Flight Info UI App (Backpack Android)

A simple Android application built using Kotlin and Skyscanner Backpack UI components, designed as part of an introductory Android development task. The app displays a clean flight information interface using cards for flight number, departure, and arrival details.

📱 App Preview

The app displays:

✈️ Flight Information Card
🛫 Departure Details Card
🛬 Arrival Details Card

Each section is built using Backpack UI components for a modern and consistent design system.

🚀 Features
Built with Kotlin
Uses Backpack Android UI Library
Clean XML-based UI design
Card-based layout using BpkCardView
Structured information display:
Flight number
Departure airport code + time
Arrival airport code + time
Responsive ConstraintLayout-based UI
🛠️ Tech Stack
Language: Kotlin
UI Design: XML (ConstraintLayout + LinearLayout)
UI Library: Backpack Android (net.skyscanner.backpack)
Min SDK: API 33 (Android Tiramisu)
IDE: Android Studio
📦 Dependencies

Backpack UI library used:

implementation 'net.skyscanner.backpack:backpack-android:43.0.0'

Make sure Gradle sync is completed after adding this dependency.

🏗️ Project Structure
app/
└── src/
└── main/
├── java/           # Kotlin source files
├── res/
│   ├── layout/
│   │   └── activity_main.xml   # Main UI layout
│   ├── values/     # Strings, themes, styles
└── AndroidManifest.xml
🎨 UI Design Overview

The UI is built using Backpack components:

✈️ Flight Card
Displays flight number using BpkText
Styled with heading typography
🛫 Departure Card
Airport code (3-letter IATA code)
Departure time
🛬 Arrival Card
Airport code (3-letter IATA code)
Arrival time

All components are wrapped inside BpkCardView for a modern card-based UI experience.

🧩 Key Components Used
BpkCardView → Card containers for flight sections
BpkText → Styled text components
ConstraintLayout → Main screen structure
LinearLayout (vertical) → Content organization inside cards
▶️ How to Run
Clone this repository:
git clone https://github.com/your-username/flight-ui-app.git
Open the project in Android Studio
Wait for Gradle Sync to complete
Click ▶️ Run button
Launch on emulator (API 33 recommended)
🧪 What I Learned
Setting up a new Android project from scratch
Working with XML layouts and ConstraintLayout
Using third-party UI libraries via Gradle
Building structured UI using Backpack components
Handling UI constraints and layout debugging
📌 Future Improvements
Add real-time flight data API integration
Make UI interactive (search flights)
Add navigation between screens
Improve responsiveness for tablets
👨‍💻 Author

Yuvashree C

📜 License

This project is for educational purposes.
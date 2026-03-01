# 🚀 Flutter PostHog Test App

A simple Flutter application demonstrating **PostHog analytics integration** for tracking user behavior, screen views, and custom events in a mobile application.

---

## 📌 Overview

This project shows how to integrate the **PostHog Flutter SDK** into a Flutter application to:

* Track button click events
* Track screen views
* Identify users
* Capture custom properties
* Prepare for feature flags integration

This app is built as a learning + portfolio project for analytics implementation in production-ready Flutter apps.

---

## 🛠️ Tech Stack

* Flutter
* Dart
* PostHog Flutter SDK
* Android Emulator / Physical Device

---

## 📂 Project Structure

```
lib/
 ├── main.dart
 ├── screens/
 │    └── home_screen.dart
 ├── services/
 │    └── analytics_service.dart
```

---

## 🔑 Features Implemented

### ✅ Event Tracking

Tracks button clicks using:

```dart
Posthog().capture(
  eventName: "Button Clicked",
  properties: {
    "button_name": "Main Button"
  },
);
```

---

### ✅ Screen Tracking

```dart
Posthog().screen(
  screenName: "Home Screen",
);
```

---

### ✅ User Identification

```dart
Posthog().identify(
  userId: "user_email@example.com",
);
```

---

## ⚙️ Setup Instructions

### 1️⃣ Clone Repository

```
git clone https://github.com/your-username/flutter_posthog_test.git
cd flutter_posthog_test
```

---

### 2️⃣ Install Dependencies

```
flutter pub get
```

---

### 3️⃣ Add Your PostHog API Key

Open:

```
lib/main.dart
```

Replace:

```dart
'phc_6hlafAgUv2X24zOR88SPVjWCbOxFYkeLD9TSwJt0Opu'
```

With your actual PostHog project API key.

---

### 4️⃣ Run Application

```
flutter run
```

---

## 📊 Analytics Dashboard

After running the app:

1. Click the button inside the app
2. Go to your PostHog dashboard
3. Navigate to **Events**
4. You should see:

   * Button Clicked event
   * Screen View event

---

## 🔥 Future Improvements

* Feature flags integration
* Firebase Authentication
* Crash reporting
* Clean MVVM architecture
* Analytics service abstraction layer
* Unit testing

---

## 🎯 Learning Outcomes

* Understanding event-based analytics
* Integrating third-party SDK in Flutter
* Tracking user behavior in mobile apps
* Preparing analytics-ready production apps

---

## 👨‍💻 Author

Bangaru Karthikreddy
Flutter Developer | Software Engineer Aspirant

---

# ⭐ If You Like This Project

Give it a star ⭐ on GitHub.

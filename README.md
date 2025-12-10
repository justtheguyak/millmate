# 🌾 MillMate - Fresh Flour Delivery App

**MillMate** is a premium Flutter e-commerce application designed for local flour mills. It allows users to order fresh grains, spices, and flour with customizable grinding preferences (Fine, Medium, Coarse), featuring a seamless offline-first experience.

---

## ✨ Key Features

### 🛍️ Smart Shopping
* **Custom Grinding:** Users can choose specific grinding levels (e.g., "Fine for Rotis", "Coarse for Ladoo").
* **Search & Filter:** Advanced search for products with category filters.
* **Wishlist:** Save favorite items for quick access later.

### 💳 Payment & Checkout
* **Wallet System:** Add, Edit, and Delete Credit Cards, Debit Cards, and UPI IDs with beautiful gradient UI.
* **Smart Inputs:** Auto-formatting for card numbers and expiry dates.
* **Secure Checkout:** Simulated checkout process with multiple payment modes (COD, UPI).

### 🚚 Real-Time Tracking & Notifications
* **Live Tracking:** Animated timeline showing Order Confirmed → Out for Delivery → Delivered.
* **Local Notifications:** Background alerts update the user on order status even when the app is closed.
* **Simulated Delivery:** Realistic time delays (15s for dispatch, 30s for delivery) for testing.

### 👤 User Experience
* **Dark/Light Mode:** Fully persistent theme support that remembers user preference.
* **Profile Management:** Set profile pictures directly from the gallery.
* **Order History:** Persistent storage of past orders with "Clear History" functionality.

---

## 🛠️ Tech Stack

* **Framework:** [Flutter](https://flutter.dev/) (Dart)
* **State Management:** Provider
* **Local Storage:** SharedPreferences (For Orders, Profile, Theme, and Cards)
* **Notifications:** Flutter Local Notifications & Timezone
* **Architecture:** MVC Service-Based Architecture

---

## 🚀 How to Run Locally

1.  **Clone the project**
    ```bash
    git clone [https://github.com/justtheguyak/millmate.git](https://github.com/justtheguyak/millmate.git)
    ```
2.  **Install dependencies**
    ```bash
    flutter pub get
    ```
3.  **Run the app**
    ```bash
    flutter run
    ```

---

## 📲 Release Workflow (The "Calculator Method")

**Note to Developer:** This project uses a custom workflow where source code remains private, and only the APK is hosted via GitHub.

### Step 1: Build the Update
1.  Open `pubspec.yaml` and increment the version (e.g., `1.1.0+1`).
2.  Run the build command:
    ```bash
    flutter build apk --release
    ```

### Step 2: Upload the APK
1.  Copy `build/app/outputs/flutter-apk/app-release.apk`.
2.  Paste it into your **Desktop/millmate** folder.
3.  Rename it to `millmate.apk` (Replace the old file).
4.  Open Terminal in that folder and run:
    ```powershell
    git add .
    git commit -m "Update Release v1.x.x"
    git push
    ```

### Step 3: Trigger the Update Signal
1.  Go to the GitHub repository.
2.  Edit `version.json`.
3.  Update the version number to match your release (e.g., `"1.1.0"`).
4.  Commit changes.

*Users will now receive the update popup immediately.*

---

## 📝 License
Copyright © 2024 MillMate. All rights reserved.

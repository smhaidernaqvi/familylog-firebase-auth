# 🔥 FamilyLog — Firebase Authentication

> **Week 1 Deliverable** | WiseGem AI Internship Program

A complete Firebase + Google Sign-In authentication flow built from scratch. Users can sign in with Google, view their profile, and their session data is saved to Firestore in real-time.

---

## 🚀 Live Demo

👉 **[https://familylog-dev.web.app](https://familylog-dev.web.app)**

---

## ✅ Features

- Google Sign-In with Firebase Auth
- Smooth animated panel transitions
- Google-colored loading spinner
- Displays user name, email & profile photo after login
- Saves `uid`, `email`, `login_time` to Firestore on every login
- Sign-Out with animated transition
- Firestore Security Rules — users can only access their own data

---

## 🛠️ Tech Stack

- HTML, CSS, JavaScript (ES Modules)
- Firebase Authentication v10
- Cloud Firestore
- Firebase Hosting

---

## 📸 Screenshots

### Firestore Console
![Firestore Console](screenshots/Firestore%20Console.png)

### Google Cloud OAuth Setup
![Google Cloud Console](screenshots/Google%20Cloud%20Console.png)

---

## ⚠️ Errors & Solutions

- **`auth/unauthorized-domain`** — Firebase did not recognize `127.0.0.1` as an authorized domain. Fixed by adding `127.0.0.1` to the authorized domains list in Firebase Console.
- **Google popup closing immediately** — `127.0.0.1:5501` was not registered in Google Cloud Console OAuth client. Fixed by adding it to the authorized JavaScript origins.
- **Firebase CLI login fail** — Firebase CLI version `v24.17.0` was buggy causing authentication to fail repeatedly. Downgraded to `v24.16.0` which resolved the login issue successfully.

---

## 📁 Project Structure

```
familylog-firebase-auth/
├── index.html        # Main login page
├── 404.html          # Error page
├── firebase.json     # Firebase hosting config
├── .firebaserc       # Firebase project reference
└── screenshots/      # Submission screenshots
```
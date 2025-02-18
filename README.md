This is a fully functional LinkedIn Clone built using React.js, Redux, Firebase, and Material-UI. It includes authentication, real-time content posting, and a responsive design that replicates LinkedIn's core functionalities.

## 📜 Table of Contents

- [Overview](#overview)
  - [Introduction](#introduction)
  - [Screenshots](#screenshots)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Installation & Setup](#installation--setup)
- [Challenges & Solutions](#challenges--solutions)
- [Future Enhancements](#future-enhancements)
- [Author](#author)

---

## 📝 Overview

### Introduction

This project is a dynamic social networking platform that mimics LinkedIn's functionality. It allows users to:

- Register and sign in using Firebase Authentication (including Google Sign-In OAuth).
- Create and share posts with other users in real time using Firebase Firestore.
- View posts from other users in a live feed.
- Logout securely and persist authentication state using Redux.
- Experience a fully responsive and interactive UI with Material-UI components and animations.

---

## 🚀 Features

✔️ **OAuth-Based Authentication:** Secure login using Firebase Authentication and Google Sign-In API.
✔️ **Real-Time Database:** Posts update instantly using Firebase Firestore.
✔️ **Redux State Management:** User authentication and session persistence.
✔️ **Material-UI Styling:** Sleek and responsive UI with modern design elements.
✔️ **React Flip Move Animation:** Smooth transitions when posts are added or removed.
✔️ **Mobile-Friendly Design:** Fully responsive layout for seamless experience on all devices.
✔️ **Firebase Hosting:** Live deployment using Firebase Hosting.

---

## 💻 Tech Stack

- **Frontend:** React.js, Redux
- **Backend:** Firebase Firestore (NoSQL database)
- **Authentication:** Firebase Authentication (Email/Password, Google OAuth)
- **UI Components:** Material-UI
- **Animations:** React Flip Move
- **Hosting:** Firebase Hosting

---

## ⚙️ Installation & Setup

1. **Clone the repository:**
   ```sh
   git clone https://github.com/your-username/linkedin-clone.git
   cd linkedin-clone
   ```
2. **Install dependencies:**
   ```sh
   npm install
   ```
3. **Set up Firebase:**
   - Create a Firebase project at [Firebase Console](https://console.firebase.google.com/).
   - Enable Authentication (Email/Password & Google Sign-In).
   - Set up Firestore Database in test mode.
   - Obtain Firebase config and replace it in `firebase.js`.
4. **Run the project:**
   ```sh
   npm start
   ```

---

## 🛠️ Challenges & Solutions

### 🔹 Authentication State Persistence
**Issue:** User authentication state was lost on page refresh.
**Solution:** Implemented Firebase `onAuthStateChanged` listener and stored user state in Redux for persistence.

### 🔹 Optimizing Firestore Queries
**Issue:** Firestore reads were high, affecting performance.
**Solution:** Optimized queries using indexes and limited reads by only fetching necessary data.

---


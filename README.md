# 📲 Android Firebase Notification System

This Android application demonstrates a complete notification system integrated using **Firebase Cloud Messaging (FCM)**. Notifications received are stored locally, displayed in a list, and highlighted based on whether they are **read** or **unread**.

---

## 🛠️ Tech Stack

- **Language**: Java
- **IDE**: Android Studio
- **Backend**: Firebase Cloud Messaging (FCM)
- **Local Storage**: Room / SQLite
- **Notification UI**: Material Design Components

---

## 🔔 Features

- Receive push notifications via Firebase
- Store all received notifications locally
- Display a list of notifications with timestamp
- Highlight **unread** notifications
- Show **detailed view** of each notification on tap
- Change card background color to grey once notification is read

---

## 📱 UI Screenshots

### 🔹 Firebase Notifications in Action
| Notification Drawer | Multiple Notifications | Details Screen |
|---------------------|------------------------|----------------|
| ![notif1](screenshots/notification1.jpg) | ![notif2](screenshots/notification2.jpg) | ![notif3](screenshots/notification3.jpg) |

### 🔹 In-App Notification List
| Notification List | Detailed Notification | Read Highlight |
|-------------------|------------------------|----------------|
| ![notif4](screenshots/notification4.jpg) | ![notif5](screenshots/notification5.jpg) | ![notif6](screenshots/notification6.jpg) |

---

## 🧩 How It Works

1. **Firebase Setup**: 
   - Firebase project created and FCM enabled.
   - `google-services.json` added to the project.

2. **Notification Receiving**:
   - FirebaseMessagingService subclass handles incoming messages.
   - Notification data is parsed and saved locally.

3. **Local Storage**:
   - Notifications are stored in SQLite/Room database.
   - Read/unread status is tracked using a boolean flag.

4. **UI Display**:
   - RecyclerView shows all notifications.
   - Clicking an item opens the detailed view.
   - Background color updates on read to visually distinguish.

---

## 📂 Project Structure


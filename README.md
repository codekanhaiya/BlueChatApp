# 💙 BlueChat App

**BlueChat** is an Android Bluetooth-based peer-to-peer chat application built using **Java**. It allows users to chat over a Bluetooth connection without the need for an internet connection. The app is designed to be compatible with **Android 10 (API 29)** and above.

---

## 📱 Features

- 📡 Bluetooth device discovery and connection
- 📲 Peer-to-peer messaging between two devices
- 🔐 Runtime permissions for Android 10+ and 12+
- ⚙️ Clean, modular codebase using multithreading
- ✅ Compatible with Android 10+ (API 29 and above)

---

## 🛠 Technologies Used

- **Language**: Java
- **IDE**: Android Studio 2022.3.0.0 (Electric Eel)
- **Android SDK**: API 29+
- **Bluetooth**: Classic Bluetooth SPP (`RfcommSocket`)
- **Threading**: `AcceptThread`, `ConnectThread`, `ConnectedThread`

---

## 📂 Folder Structure

```
BlueChat/
|
├── .gradle/
├── .idea/
├── app/
│ ├── build/
│ ├── libs/
│ ├── src/
│ │ ├── androidTest/
│ │ ├── main/
│ │ │ ├── java/
│ │ │ │ └── com/example/bluechat/
│ │ │ │ ├── MainActivity.java
│ │ │ │ ├── ChatUtils.java
│ │ │ │ └── (other classes)
│ │ │ └── res/
│ │ │ ├── layout/
│ │ │ └── values/
│ │ │ └── AndroidManifest.xml
│ ├── test/
│ │ └── java/com/example/bluechat/ExampleUnitTest.java
│ ├── build.gradle
│ └── proguard-rules.pro
├── gradle/
│ └── wrapper/
│ ├── gradle-wrapper.jar
│ └── gradle-wrapper.properties
├── build.gradle
├── gradle.properties
├── gradlew
├── gradlew.bat
├── local.properties
└── settings.gradle
```

---

## 🚀 How to Run

### 🧰 Prerequisites

- Android Studio (v2022.3.0.0 or higher)
- Java 11+ installed
- Android SDK API 29+
- Physical Android device (Bluetooth won't work on emulators)

### 🧾 Setup Instructions

1. **Clone the repo**

   ```bash
   git clone https://github.com/codekanhaiya/BlueChatApp.git
   cd bluechat
   ```

2. **Open in Android Studio**

   File → Open → Select BlueChat/ directory

3. **Connect your Android phone via USB**

   Enable Developer Options

   Enable USB Debugging

4. **Run the app**

### 🔐 Permissions Required

In AndroidManifest.xml:

```
<uses-permission android:name="android.permission.BLUETOOTH" />
<uses-permission android:name="android.permission.BLUETOOTH_ADMIN" />
<uses-permission android:name="android.permission.BLUETOOTH_CONNECT" />
<uses-permission android:name="android.permission.BLUETOOTH_SCAN" />
<uses-permission android:name="android.permission.ACCESS_FINE_LOCATION" />

```

At runtime (Android 10+ and 12+), request:

- BLUETOOTH_CONNECT
- BLUETOOTH_SCAN
- ACCESS_FINE_LOCATION

## 🧪 Testing

- Pair two Android phones via Bluetooth manually
- Open app on both
- Use one to connect → start chat → send messages

## 🧠 Concepts Covered

- Bluetooth RFCOMM sockets
- Threads for connection handling
- Handler for UI updates from threads
- Runtime permissions
- Android Bluetooth API compatibility for newer versions

## 📃 License

- This project is open-source and free to use.
- Feel free to fork or extend it.

## 👨‍💻 Author

**Kanhaiya Gupta**

- 🌐 [Portfolio](http://officialkanha.epizy.com/)
- 💼 [LinkedIn](https://www.linkedin.com/in/kanhaiya-gupta-401303240)
- 📧 Email: [kanahaiyaguptaksg@gmail.com](mailto:kanahaiyaguptaksg@gmail.com)

---

Feel free to connect with me for collaborations, feedback, or contributions!

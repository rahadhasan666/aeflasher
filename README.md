<div align="center">

# ⚡ AE Flasher

### Arduino / ESP Flasher APK

**Flash, upload & manage firmware on Arduino and ESP modules — right from your Android device.**

[![Platform](https://img.shields.io/badge/Platform-Android-3DDC84?style=for-the-badge\&logo=android\&logoColor=white)](https://www.android.com/)
[![Version](https://img.shields.io/badge/Version-V1-blue?style=for-the-badge)](https://github.com/rahadhasan666/aeflasher/releases)
[![Developer](https://img.shields.io/badge/Developer-Rahad%20Hasan-orange?style=for-the-badge)](https://github.com/rahadhasan666)
[![License](https://img.shields.io/badge/License-MIT-purple?style=for-the-badge)](LICENSE)

[**⬇️ Download APK**](https://github.com/rahadhasan666/aeflasher/releases/download/AE_Flasher_V1/AE.Flasher.apk) · [**Report Bug**](https://github.com/rahadhasan666/aeflasher/issues) · [**Request Feature**](https://github.com/rahadhasan666/aeflasher/issues)

</div>

---

## 📖 About

**AE Flasher (Arduino ESP Flasher)** is a mobile embedded development and firmware flashing application for Android.

It allows you to **connect, flash, upload and manage supported Arduino, ESP32 and ESP8266 modules directly from your Android device using USB OTG**.

AE Flasher is designed for makers, IoT developers, embedded developers, students and hardware enthusiasts who want a convenient mobile workflow without always needing a PC.

---

## ✨ Features

* 🔌 **USB OTG Support** — Connect compatible Arduino, ESP32, ESP8266 and USB-serial boards directly to Android.
* 🔥 **Firmware Flashing** — Flash supported firmware files directly to connected modules.
* 📁 **Firmware File Upload** — Select and upload firmware/files from your device.
* 📝 **Built-in Code Editor** — Write and edit Arduino-style C/C++ code directly inside the app.
* 📦 **Module Package Downloader** — Download required board packages and module resources.
* 🔍 **Hardware Detection** — Detect supported connected USB devices and board information.
* 📡 **Serial Communication** — Communicate with supported boards through USB serial.
* ⚡ **Fast Mobile Workflow** — Designed for quick embedded development and flashing.
* 🌙 **Modern Dark Interface** — Clean and mobile-friendly UI.
* 📱 **PC-Free Workflow** — Perform supported operations directly from an Android smartphone.
* 💾 **Offline Flashing** — Flashing can work without internet when the required files/packages are already available locally.

---

## 📸 Screenshots

<div align="center">

|                             🚀 Splash Screen                             |                             🏠 Main Screen                             |
| :----------------------------------------------------------------------: | :--------------------------------------------------------------------: |
| <img src="https://i.ibb.co.com/JFGg7V9w/splash-screen.png" width="220"/> | <img src="https://i.ibb.co.com/ycfT3K4G/main-screen.png" width="220"/> |

|                             💻 Code Write Screen                             |                                      📤 File Upload                                     |
| :--------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------: |
| <img src="https://i.ibb.co.com/DDc161qq/code-write-screen.png" width="220"/> | <img src="https://i.ibb.co.com/SXMyFmHJ/file-upload-to-module-screen.png" width="220"/> |

|                               📦 Module Package Downloader                              |
| :-------------------------------------------------------------------------------------: |
| <img src="https://i.ibb.co.com/991RHfH0/module-pkg-downloader-screen.png" width="220"/> |

</div>

---

## 🧩 Supported Platforms

AE Flasher is designed for supported Arduino-compatible and ESP development boards.

### ESP Family

* ESP32
* ESP8266
* Compatible ESP development boards

### Arduino Family

* Arduino Uno
* Arduino Nano
* Arduino Mega
* Other compatible Arduino boards

### USB Interfaces

Compatible USB-to-serial interfaces may include:

* CH340 / CH341
* CP210x
* FTDI
* PL2303
* USB CDC / ACM
* Espressif native USB

> Actual compatibility depends on the Android device, USB OTG implementation, board hardware and USB chipset.

---

## 🔌 USB OTG Connection

A typical setup looks like this:

```text
┌──────────────────┐
│  Android Phone   │
│                  │
│   AE Flasher     │
└────────┬─────────┘
         │
      USB OTG
         │
         ▼
┌──────────────────┐
│ Arduino / ESP    │
│ ESP32 / ESP8266  │
└──────────────────┘
```

You need an Android device that supports **USB OTG / USB Host**.

---

## 🔥 Firmware Flashing

AE Flasher is designed to simplify firmware flashing from Android.

### Supported file types

```text
.bin
.hex
.ino
```

For supported ESP boards, the flashing workflow can communicate with the device bootloader through USB serial communication.

Typical workflow:

```text
Select Firmware
       ↓
Connect Module
       ↓
Detect Device
       ↓
Enter Flash Mode
       ↓
Upload Firmware
       ↓
Verify
       ↓
Completed ✓
```

---

## 📝 Code Editor

AE Flasher includes a mobile code-writing interface for embedded development.

The editor is designed around Arduino-style C/C++ development and provides a convenient environment for writing or editing code directly from an Android device.

Example:

```cpp
void setup() {
    Serial.begin(115200);
}

void loop() {
    Serial.println("Hello from AE Flasher!");
    delay(1000);
}
```

---

## 📤 File Upload

The **File Upload to Module** interface allows users to select supported files from Android storage and send them to the connected hardware where supported.

This is useful for firmware files and other embedded development resources.

---

## 📦 Module Package Downloader

AE Flasher includes a package downloader for obtaining required module/board resources.

It is intended to make board setup easier by providing package-related resources directly from the application.

Internet access may be required when downloading packages.

---

## 🛠️ Technology Stack

| Technology               | Purpose                         |
| ------------------------ | ------------------------------- |
| **Flutter**              | Android application framework   |
| **Dart**                 | Application development         |
| **Kotlin**               | Native Android integration      |
| **Android USB Host API** | USB hardware communication      |
| **MethodChannel**        | Flutter ↔ Android communication |
| **C/C++**                | Arduino / embedded development  |
| **Crypto**               | File verification / hashing     |
| **File Picker**          | Firmware and file selection     |
| **Path Provider**        | Local file management           |
| **Shared Preferences**   | Local settings                  |

---

## 📁 Project Structure

```text
lib/
├── core/
│   ├── usb/
│   └── serial/
│
├── devices/
│   ├── common/
│   ├── esp32/
│   └── esp8266/
│
├── flashing/
│
├── boards/
│
├── editor/
│
├── terminal/
│
└── screens/
```

---

## ⬇️ Download

<div align="center">

### 📱 AE Flasher V1

[![Download APK](https://img.shields.io/badge/⬇️_DOWNLOAD-AE_Flasher_V1-blue?style=for-the-badge)](https://github.com/rahadhasan666/aeflasher/releases/download/AE_Flasher_V1/AE.Flasher.apk)

**[View All Releases](https://github.com/rahadhasan666/aeflasher/releases)**

</div>

### Direct APK

```text
https://github.com/rahadhasan666/aeflasher/releases/download/AE_Flasher_V1/AE.Flasher.apk
```

---

## 🚀 Getting Started

### 1. Install AE Flasher

Download the APK and install it on your Android device.

If Android blocks APK installation, enable installation permission for the browser or file manager you used to download the APK.

### 2. Connect Your Module

Connect your Arduino, ESP32 or ESP8266 board through a compatible **USB OTG adapter/cable**.

### 3. Open AE Flasher

Launch the application and allow USB access when Android requests permission.

### 4. Select Your Workflow

Depending on your project, you can:

* Write code
* Select firmware
* Upload files
* Download module packages
* Communicate with the board

### 5. Flash / Upload

Select the required firmware or file and start the supported operation.

---

## 📋 Requirements

| Requirement    | Details                                     |
| -------------- | ------------------------------------------- |
| **Platform**   | Android                                     |
| **USB**        | USB OTG / USB Host                          |
| **Storage**    | At least 50 MB recommended                  |
| **Connection** | USB OTG adapter + compatible cable          |
| **Boards**     | ESP32, ESP8266, Arduino & compatible boards |
| **Internet**   | Required for online package downloads       |

> Android version and hardware compatibility may vary depending on the device and connected board.

---

## ⚠️ Important

AE Flasher interacts directly with connected embedded hardware.

Before flashing firmware:

* Make sure the correct board is selected.
* Use the correct firmware file.
* Ensure the board has sufficient power.
* Do not disconnect the USB connection during flashing.
* Use a reliable USB OTG adapter and cable.

Incorrect firmware or interrupted flashing may cause the device to require recovery or re-flashing.

---

## 🔐 Responsible Use

AE Flasher is intended for legitimate embedded development and hardware testing.

Use the application only with hardware that you own or are authorized to modify.

---

## 👨‍💻 Developer

### Rahad Hasan

**Developer:** Rahad Hasan

* 🐙 **GitHub:** [@rahadhasan666](https://github.com/rahadhasan666)
* 📦 **Repository:** [aeflasher](https://github.com/rahadhasan666/aeflasher)
* 🌐 **Portfolio:** [rahadhasan.iam.bd](https://rahadhasan.iam.bd)
* 📱 **Telegram:** [@third_eye666](https://t.me/third_eye666)

---

## 🤝 Contributing

Contributions, bug reports and feature requests are welcome.

### Fork the repository

```bash
git clone https://github.com/rahadhasan666/aeflasher.git
cd aeflasher
```

### Install dependencies

```bash
flutter pub get
```

### Run

```bash
flutter run
```

### Build APK

```bash
flutter build apk --release
```

---

## 🐞 Bug Reports

Found a problem?

Open an issue:

👉 [**Report a Bug on GitHub**](https://github.com/rahadhasan666/aeflasher/issues)

For feature suggestions:

👉 [**Request a Feature**](https://github.com/rahadhasan666/aeflasher/issues)

---

## 📄 License

This project is licensed under the **MIT License**.

See the [LICENSE](LICENSE) file for details.

---

## ⭐ Support AE Flasher

If you find AE Flasher useful:

⭐ **Star the repository**

🐛 **Report bugs**

💡 **Suggest features**

🔧 **Contribute to the project**

📢 **Share it with other Arduino & ESP developers**

<div align="center">

### ⚡ AE Flasher

**Arduino / ESP Flasher for Android**

Made with ❤️ by **[Rahad Hasan](https://github.com/rahadhasan666)**

</div>

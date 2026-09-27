# 👵👴 Elder Voice Check-In

A highly accessible, voice-activated daily check-in application designed specifically for the elderly. 

Many modern communication apps require reading small text, navigating complex menus, or typing on tiny keyboards. **Elder Check-In** solves this by offering a zero-friction interface. Elders can simply tap a large visual icon or press a single button to record a voice message, while an empathetic AI voice guides them through the process.

## ✨ Features
* **Zero-Typing Interface:** Users check in by tapping large emotional faces or pressing the microphone.
* **Instant Telegram Alerts:** Any check-in or voice recording is instantly beamed to a family member's Telegram account, complete with live GPS coordinates.
* **Native Voice Recording:** Uses the `MediaRecorder` API to capture and play back actual voice messages.
* **Empathetic AI Narration:** Integrated with the **ElevenLabs API** to provide incredibly natural, calm, and human-like voice responses.
* **Cross-Platform:** Built as a standard web application, but architected with **Capacitor** to compile natively into an Android mobile application.

## 🛠️ Tech Stack
* **Frontend:** Vanilla HTML, CSS, JavaScript (No heavy frameworks, highly optimized).
* **Voice Synthesis:** ElevenLabs TTS API / Web Speech API.
* **Notifications:** Telegram Bot API.
* **Mobile Architecture:** Ionic Capacitor (for Android packaging).

## 🚀 How to Test (For Judges)

### 1. Test the Web Version (Easiest)
You can test the core functionality directly in your browser without installing anything!
1. Open the `elder-checkin (2).html` file in any modern web browser.
2. Click the **⚙️ Settings Gear** in the top right to configure API keys.
3. Tap a face or the **Microphone** button to test the workflow.

**To test the Telegram Integration:**
1. Open the **⚙️ Settings Gear**.
2. Paste a valid Telegram Bot Token and your personal Telegram Chat ID.
3. Click Save, and tap a face. You will receive an instant alert to your phone!

### 2. Build the Native Android App
This repository contains the `package.json`, `www` folder, and `capacitor.config.json` blueprints for native mobile compilation.
1. Ensure you have Node.js and Android Studio installed.
2. Run `npm install` in the directory.
3. Run `npx cap sync android`.
4. Run `npx cap open android` to build and deploy the app to an emulator or physical device.

---
*Built for the Hackathon!*

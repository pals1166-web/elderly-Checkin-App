# 👵👴 Elder Voice Check-In

A highly accessible, voice-activated daily check-in application designed specifically for the elderly. 

Many modern communication apps require reading small text, navigating complex menus, or typing on tiny keyboards. **Elder Check-In** solves this by offering a zero-friction interface. Elders can simply tap a large visual icon or press a single button to record a voice message, while an empathetic AI voice guides them through the process.

## ✨ Features
* **Zero-Typing Interface:** Users check in by tapping large emotional faces or pressing the microphone.
* **Native Voice Recording:** Uses the `MediaRecorder` API to capture and play back actual voice messages.
* **Empathetic AI Narration:** Integrated with the **ElevenLabs API** to provide incredibly natural, calm, and human-like voice responses (with a seamless fallback to the browser's built-in TTS if offline or if no API key is provided).
* **Dynamic Family Management:** A secure, local-storage-based CRUD interface to manage emergency contacts.
* **Cross-Platform:** Built as a standard web application, but architected with **Capacitor** to compile natively into an Android mobile application with native microphone and GPS permissions.

## 🛠️ Tech Stack
* **Frontend:** Vanilla HTML, CSS, JavaScript (No heavy frameworks, highly optimized).
* **Voice Synthesis:** ElevenLabs TTS API / Web Speech API (SpeechSynthesis).
* **Voice Capture:** Web `MediaRecorder` API.
* **Mobile Architecture:** Ionic Capacitor (for Android packaging).

## 🚀 How to Test (For Judges)

### 1. Test the Web Version (Easiest)
You can test the core functionality directly in your browser without installing anything!
1. Open the `elder-checkin (2).html` file in any modern web browser.
2. Click the **Microphone** button to test the voice recording workflow.
3. Click the **⚙️ Settings Gear** in the top right to manage emergency contacts.

**Want to hear the Premium AI Voice?**
By default, the app uses your browser's robotic offline voice. To hear the empathetic ElevenLabs voice:
1. Click the **⚙️ Settings Gear**.
2. Paste your own ElevenLabs API Key into the top box.
3. Leave the Voice ID blank (it defaults to "Antoni", a calm male voice), and click Save!

### 2. Build the Native Android App
This repository contains the `package.json` and `capacitor.config.json` blueprints for native mobile compilation.
1. Ensure you have Node.js and Android Studio installed.
2. Run `npm install` in the directory.
3. Run `npx cap sync android`.
4. Run `npx cap open android` to build and deploy the app to an emulator or physical device.

---
*Built for the Hackathon!*

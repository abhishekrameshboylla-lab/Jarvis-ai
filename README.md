# JARVIS Android Starter

A small Android starter project for a voice-controlled English assistant. It includes:
- Tap-to-talk speech input using Android speech recognition
- Spoken responses using Android Text-to-Speech
- Demo commands for time/date, status, security, encryption, and housekeeping
- A simple in-memory housekeeping task list

## Important limitations
This is a starter prototype, not a complete advanced JARVIS:
- It does not connect to an online AI model yet.
- Security and encryption screens are informational placeholders. Do not use this build to protect sensitive files.
- It does not continuously listen for a wake word.
- Android speech recognition availability depends on device services and permissions.

## Build an APK
1. Install Android Studio on a computer.
2. Open this folder as an existing project.
3. Allow Gradle to sync and install any requested Android SDK platform (API 35).
4. Connect the tablet with USB debugging enabled, or use Build > Build Bundle(s) / APK(s) > Build APK(s).
5. The debug APK is normally created under `app/build/outputs/apk/debug/`.

## Security before real use
- Never embed an OpenAI API key in the APK. Use a secure backend for online AI requests.
- Real file encryption should use authenticated encryption (for example AES-GCM), strong random keys, and careful recovery/key-management design.
- Add Android runtime microphone permission handling and test on the target tablet before distributing.
- Require confirmation for destructive or sensitive operations.

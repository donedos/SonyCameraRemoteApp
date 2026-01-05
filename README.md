# SonyCameraRemoteApp | Sony Camera Voice Remote


A feature-rich Android application that transforms your smartphone into an intelligent remote controller for Sony Wi-Fi enabled cameras (Action Cams, Alpha series, Cybershot).

Beyond standard remote capabilities, this app features a **Voice Command Assistant** allowing for completely hands-free camera operation.

## 🌟 Key Features

### 🎙️ Voice Control Assistant
Operate your camera without touching the screen. The app uses continuous speech recognition to listen for commands.
- **Wake Word:** Commands typically require the word **"Remote"** to prevent accidental triggers.
- **Feedback:** The app speaks back to confirm actions (e.g., "Recording!", "Switching to Video Mode").
- **Commands:**
    - *"Remote Capture"* or *"Remote Snap"* → Take a photo.
    - *"Remote Record"* → Start video recording.
    - *"Remote Stop"* → Stop video recording.
    - *"Remote Switch Mode"* → Toggle between Photo and Video modes.
    - *"What is time?"* → Reads current time.

### 📸 Advanced Camera Control
- **Live View:** Low-latency real-time video feed from the camera.
- **Zoom:** Dedicated Tele/Wide zoom controls (for supported lenses).
- **Mode Switching:** Seamlessly toggle between "Still" (Photo) and "Movie" (Video) modes.
- **Auto-Download:** Photos taken via the app are automatically downloaded to your phone's gallery (`DCIM/SonyCamera/`).

### 📍 GPS Geotagging
- The app utilizes your phone's GPS data.
- When a photo is transferred from the camera, the app automatically injects your current Latitude/Longitude into the image's EXIF data, ensuring your photos are correctly placed on the map.

## 🛠️ Tech Stack

- **Language:** Java
- **Platform:** Android SDK
- **Communication:**
    - **SSDP (Simple Service Discovery Protocol):** For finding cameras on the local Wi-Fi network.
    - **Sony Camera Remote API:** JSON-RPC over HTTP for sending commands.
- **Libraries:**
    - **OkHttp:** For reliable network requests and image downloading.
    - **ButterKnife:** For view binding.
    - **Android SpeechRecognizer:** For voice command processing.
    - **Google TextToSpeech (TTS):** For voice feedback.

## 🚀 Getting Started

### Prerequisites
1. An Android device running Android 6.0 (Marshmallow) or higher.
2. A Sony Camera compatible with the *Camera Remote API* (e.g., Sony a6000 series, RX100 series, Action Cams).

## 🤝 Contributing
Feel free to fork this project, report issues, or submit pull requests to enhance the remote control capabilities.

### Installation
1. Clone the repo:
   ```sh
   git clone [https://github.com/YOUR_USERNAME/SonyCameraVoiceRemote.git](https://github.com/YOUR_USERNAME/SonyCameraVoiceRemote.git)

# Text-To-Speech

An Android application that converts typed text into spoken audio using Android's built-in Text-to-Speech (TTS) engine.

## Features

- Enter any text and have it read aloud
- Uses the device's native TTS engine (works offline once voice data is installed)
- Simple, lightweight interface
- Built with Gradle for easy setup in Android Studio

## Tech Stack

- **Platform:** Android
- **Build system:** Gradle
- **IDE:** Android Studio
- **Core API:** `android.speech.tts.TextToSpeech`

## Project Structure

```
Text-To-Speech/
├── app/                  # Main application module (source code, resources, manifest)
├── gradle/wrapper/       # Gradle wrapper files
├── build.gradle          # Top-level build configuration
├── settings.gradle       # Project module settings
├── gradle.properties     # Gradle project properties
├── gradlew               # Gradle wrapper script (macOS/Linux)
└── gradlew.bat           # Gradle wrapper script (Windows)
```

## Prerequisites

- [Android Studio](https://developer.android.com/studio) (latest stable version recommended)
- JDK 11 or higher (bundled with recent Android Studio versions)
- An Android device or emulator running a version supported by the project's `minSdkVersion`
- A TTS engine installed on the device (Google Text-to-Speech is preinstalled on most devices)

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/shreya-setty/Text-To-Speech.git
cd Text-To-Speech
```

### 2. Open in Android Studio

1. Launch Android Studio
2. Select **File → Open** and choose the cloned `Text-To-Speech` folder
3. Wait for Gradle to sync and download dependencies

### 3. Run the app

1. Connect an Android device (with USB debugging enabled) or start an emulator
2. Click **Run ▶** in Android Studio, or build from the command line:

```bash
# macOS / Linux
./gradlew installDebug

# Windows
gradlew.bat installDebug
```

## Usage

1. Open the app
2. Type or paste the text you want to hear
3. Tap the speak button to play the audio

## Troubleshooting

- **No sound:** Check that the device volume is up and media volume isn't muted.
- **"Language not supported" or silent output:** Open *Settings → System → Languages & input → Text-to-speech output* and install the voice data for your language.
- **Gradle sync fails:** Make sure you're using a compatible JDK and that Android Studio has the required SDK platform installed (SDK Manager).

## Future Improvements

- Adjustable speech rate and pitch
- Language and voice selection
- Save speech output to an audio file
- Pause / resume controls

## Contributing

Contributions are welcome!

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m "Add your feature"`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

## License

No license has been specified yet. Consider adding one, such as the [MIT License](https://choosealicense.com/licenses/mit/), if you'd like others to use or contribute to this project.

## Author

**Shreya Setty** — [@shreya-setty](https://github.com/shreya-setty)

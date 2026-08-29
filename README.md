### *LocalMind*: an Android application for <a href="https://lmstudio.ai/">LM Studio</a> as a server.

# Features

* Chat with our AI assistant to get instant responses.
* Seamlessly switch between different loaded models to explore various AI capabilities.
* Customize the model's behavior by using a system prompt in the settings.
* Enjoy Markdown support based on [Markdown-Compose](https://github.com/Yazan98/Markdown-Compose?utm_source=chatgpt.com), allowing for easy text formatting.
* Get hands-free input with the voice input feature.

# Download

Install the latest release APK from GitHub:

**[LocalMind 0.0.1 (app-release.apk)](https://github.com/brazer/LmStudioAndroid/releases/tag/v0.0.1)**

# Requirements

* A PC with a well-performance configuration for LLM models.
* Installed LM Studio.
* Android Studio (or JDK 17+ and the Android SDK). The Gradle wrapper runs on JDK 17 through 26, including Android Studio's bundled JDK.
* Connect both the mobile phone and the PC to the same local network via Wi-Fi.

# How to build

The project uses **Gradle 9.7.1** (via the wrapper) and **Android Gradle Plugin 9.3.0**. You do not need to install Gradle yourself.

## Prerequisites

* [Android Studio](https://developer.android.com/studio), or a standalone Android SDK
* JDK 17 or newer
* Android SDK with **compileSdk / targetSdk 35** and **minSdk 24**

If you clone the project on a new machine, create `local.properties` in the repo root (Android Studio does this automatically) with:

```
sdk.dir=/path/to/Android/Sdk
```

On Windows that is typically:

```
sdk.dir=C:\\Users\\<you>\\AppData\\Local\\Android\\Sdk
```

## Option 1: Android Studio

1. Open the project in Android Studio.
2. Wait until Gradle sync finishes.
3. In the Build Variants panel, select the **release** variant for the `app` module.
4. Use **Build → Build Bundle(s) / APK(s) → Build APK(s)**.
5. The APK is written to `app/build/outputs/apk/release/app-release.apk`.

## Option 2: Command line

From the repository root:

**Windows**

```powershell
.\gradlew.bat assembleRelease
```

**macOS / Linux**

```bash
./gradlew assembleRelease
```

The release APK is created at:

```
app/build/outputs/apk/release/app-release.apk
```

Copy it to your phone and install it (you may need to allow installing apps from unknown sources).

# The demo video
[![Watch the video](./icon_app.png)](https://youtube.com/shorts/nA5ngnSu6L4?feature=share)

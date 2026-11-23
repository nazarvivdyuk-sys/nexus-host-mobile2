# NEXUS HOST Mobile

Android application preview built with Kotlin and Jetpack Compose.

## Build APK with GitHub Actions

1. Upload the **contents** of this folder to the root of a GitHub repository (not the enclosing folder).
2. Keep `.github/workflows/android.yml` in place.
3. Open the Actions tab and run **Build NEXUS HOST APK**.
4. Download the `NEXUS-HOST-APK` artifact and extract `app-debug.apk`.

## Project layout

- `settings.gradle.kts` includes `:app`.
- Root `build.gradle.kts` declares Android and Kotlin Compose plugins.
- `app/build.gradle.kts` applies `com.android.application` and enables Compose.
- `.github/workflows/android.yml` builds `:app:assembleDebug` using JDK 17 and Gradle 8.9.

## Current functionality

This is a UI preview. Server status, console commands, and settings are local demo state. No real server connection or server-control API is implemented yet. The app does not request network access.

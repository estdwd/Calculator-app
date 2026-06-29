```
# Scientific Calculator - Android App

## Built Without Android Studio

This project was built using **VS Code + Gradle CLI** on a 4GB RAM PC that couldn't run Android Studio.

## Tech Stack
- Kotlin (native Android logic)
- XML (native Android layouts)
- exp4j (expression evaluation library)
- Gradle 8.7 (build system)

## How It Works
- VS Code for editing Kotlin/XML files
- Android SDK command-line tools (no Studio)
- Gradle wrapper builds the APK via terminal
- ADB installs directly to phone via USB
- Fully offline builds after first setup

## Features
- Scientific functions (sin, cos, tan, log, ln)
- Permutations (nPr) & Combinations (nCr)
- Factorial, square root, powers
- Auto-bracket functions (sin9 → sin(9))
- Implicit multiplication (9sin9 → 9×sin(9))
- Dual display (expression preview + result)
- Dark theme with depth shadows
- Rounded buttons with glow effects

## Build Commands
```

gradlew assembleDebug --offline    (build APK)
adb install app-debug.apk           (install on phone)
rename_package.bat                  (change package name)

```

## Why No Android Studio?
- 4GB RAM couldn't handle Studio
- Learned Gradle build system directly
- Same Kotlin + XML output
- Lighter, faster workflow
- Works offline after first setup

## Project Structure
```

app/src/main/java/.../MainActivity.kt    (calculator logic)
app/src/main/res/layout/activity_main.xml (UI design)
app/src/main/res/drawable/                (button styles)
app/build.gradle                          (dependencies)
gradle.properties                         (build config)

```

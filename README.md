# Heart Rate Limits

A simple Android app that calculates your target heart rate zone for exercise based on your age.

Made as a course exercise for **Mobile Programming with Native Technologies** at Oulu University of Applied Sciences (Oamk).

## Features

- Enter your age in a text field
- The app instantly shows your recommended heart rate limits
- Invalid input (e.g. letters) is handled safely without crashing
## How it works

The app uses a common formula for estimating target heart rate:

| Value             | Formula                    |
|-------------------|----------------------------|
| Max heart rate    | `220 - age`                |
| Lower limit (65%) | `(220 - age) * 0.65`       |
| Upper limit (85%) | `(220 - age) * 0.85`       |

**Example:** age 30 → limits are **123.50 - 161.50** bpm.

## Built with

- [Kotlin](https://kotlinlang.org/)
- [Jetpack Compose](https://developer.android.com/compose) (Material 3)
- Android Studio
## Getting started

1. Clone the repository:
```bash
git clone https://github.com/jmitteli/HeartRateLimits.git
```
2. Open the project in Android Studio (**File → Open**).
3. Wait for Gradle sync to finish.
4. Run the app on an emulator or a physical device (**Run ▶**).
## Project structure

```
app/src/main/
├── java/fi/oamk/heartratelimits/
│   └── MainActivity.kt      # UI and heart rate calculation
└── res/values/
    └── strings.xml          # UI texts
```
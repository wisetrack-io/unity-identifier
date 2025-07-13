# WiseTrack Unity Identifier Plugin

This is the **Identifier Plugin** for the [WiseTrack Unity SDK](https://github.com/wisetrack-io/unity-sdk).

This plugin provides native Android libraries to help the core SDK retrieve important identifiers such as **Google App Set ID** and **Advertising ID**.

> **Note:** This plugin does nothing by itself. It must be used **together with the WiseTrack Unity SDK**.

## Table of Contents

- [Requirements](#requirements)
- [What’s Inside](#whats-inside)
- [Installation](#installation)
- [License](#license)

## Requirements

- Unity 2019.4 or later
- Kotlin version 1.9.0 or later
- Android API 21 (Lollipop) or later
- External Dependency Manager for Unity (EDM4U) installed

## What’s Inside

This plugin only includes precompiled native `.aar` libraries:

- **play-services-ads-identifier:** `18.2.0`
- **play-services-appset:** `16.1.0`
- Plus related transitive dependencies required by these Google Play Services libraries

## Installation

To integrate the WiseTrack Identifier Unity Package into your Unity project, follow these steps:

1. **Install External Dependency Manager for Unity (EDM4U)**:
   The WiseTrack Unity Package requires EDM4U to manage Android and iOS dependencies. Follow the installation instructions provided in the [EDM4U GitHub repository](https://github.com/googlesamples/unity-jar-resolver).

2. **Add the WiseTrack Identifier Package**:
   You can add the package via Unity Package Manager (UPM) or directly from a Git URL.

   ### Option 1: Via Unity Package Manager (UPM)

   - Open Unity and navigate to `Window > Package Manager`.
   - Click the `+` button in the top-left corner and select `Add package from git URL`.
   - Enter the following URL (replace with the actual GitHub URL for your package):
     ```
     https://github.com/wisetrack-io/unity-identifier.git
     ```
   - Click `Add`. Unity will download and install the package.
   - If prompted, resolve dependencies using EDM4U by navigating to `Assets > External Dependency Manager > Android Resolver > Force Resolve`.

   ### Option 2: Via GitHub (Manual Import)

   - Clone or download the WiseTrack Identifier package repository from [GitHub](https://github.com/wisetrack-io/unity-identifier).
   - Extract the contents to your project’s `Assets/Plugins/WiseTrackIdentifier` folder.
   - Open Unity, and EDM4U will automatically detect and resolve dependencies. If not, manually trigger resolution via `Assets > External Dependency Manager > Android Resolver > Resolve`.

3. **Configure Android**:
   Ensure your `minSdkVersion` is set to 21 or later

4. **Rebuild the Project**:
   Build your project to ensure all dependencies are correctly integrated:
   - In Unity, go to `File > Build Settings` and select your target platform.
   - Click `Build` or `Build and Run`.

## License

The WiseTrack Unity Package is licensed under the WiseTrack SDK License Agreement. See the [LICENSE](LICENSE) file for details.

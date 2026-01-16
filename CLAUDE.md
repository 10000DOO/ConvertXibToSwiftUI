# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

ConvertXibToSwiftUI is a macOS application built with SwiftUI. The project appears to be in its initial setup phase with a standard SwiftUI app template.

## Build Commands

**Build the project:**
```bash
xcodebuild -project ConvertXibToSwiftUI.xcodeproj -scheme ConvertXibToSwiftUI -configuration Debug build
```

**Build for Release:**
```bash
xcodebuild -project ConvertXibToSwiftUI.xcodeproj -scheme ConvertXibToSwiftUI -configuration Release build
```

**Clean build artifacts:**
```bash
xcodebuild -project ConvertXibToSwiftUI.xcodeproj -scheme ConvertXibToSwiftUI clean
```

**Open in Xcode:**
```bash
open ConvertXibToSwiftUI.xcodeproj
```

## Project Structure

- **ConvertXibToSwiftUI/**: Main application source directory
  - `ConvertXibToSwiftUIApp.swift`: App entry point using `@main` attribute
  - `ContentView.swift`: Main view of the application
  - `Assets.xcassets/`: Asset catalog for images, colors, and app icon

- **DerivedData/**: Xcode build artifacts (excluded from version control via .gitignore)

## Technical Configuration

- **Platform**: macOS (MACOSX_DEPLOYMENT_TARGET = 26.2)
- **Swift Version**: 5.0
- **Xcode Version**: 26.2 (LastSwiftUpdateCheck = 2620)
- **Bundle Identifier**: com.10000DOO.ConvertXibToSwiftUI
- **App Sandbox**: Enabled
- **SwiftUI Previews**: Enabled
- **Swift Concurrency**: Uses MainActor isolation by default

## Development Notes

- The project uses SwiftUI for UI development
- App sandbox is enabled with read-only user-selected files permission
- The project generates Info.plist automatically (GENERATE_INFOPLIST_FILE = YES)
- Build targets are built independently in parallel (BuildIndependentTargetsInParallel = 1)

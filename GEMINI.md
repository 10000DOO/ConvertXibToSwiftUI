# ConvertXibToSwiftUI - Project Context

## Project Overview
**ConvertXibToSwiftUI** is a native macOS application developed using SwiftUI. 
Based on the project name, the intended functionality is likely a utility to convert legacy Interface Builder (XIB) files into modern SwiftUI code. 
Currently, the project is in the initial setup phase, utilizing the standard Xcode SwiftUI app template.

## Technology Stack
- **Language:** Swift 5.0+
- **UI Framework:** SwiftUI
- **Platform:** macOS (Deployment Target: 15.2+)
- **IDE:** Xcode 16.2+

## Project Structure
The project follows a standard Xcode project layout:

- **`ConvertXibToSwiftUI/`**: Main source directory.
  - `ConvertXibToSwiftUIApp.swift`: The application entry point (marked with `@main`).
  - `ContentView.swift`: The initial root view of the application.
  - `Assets.xcassets/`: Resource catalog containing app icons, colors, and images.
- **`ConvertXibToSwiftUI.xcodeproj`**: The Xcode project bundle containing build settings and project configuration.
- **`DerivedData/`**: Contains build artifacts and intermediate files (ignored by git).

## Building and Running

### CLI Commands
You can build the project directly from the terminal using `xcodebuild`:

*   **Build (Debug):**
    ```bash
    xcodebuild -project ConvertXibToSwiftUI.xcodeproj -scheme ConvertXibToSwiftUI -configuration Debug build
    ```

*   **Build (Release):**
    ```bash
    xcodebuild -project ConvertXibToSwiftUI.xcodeproj -scheme ConvertXibToSwiftUI -configuration Release build
    ```

*   **Clean:**
    ```bash
    xcodebuild -project ConvertXibToSwiftUI.xcodeproj -scheme ConvertXibToSwiftUI clean
    ```

### IDE
To open the project in Xcode for development and visual debugging:
```bash
open ConvertXibToSwiftUI.xcodeproj
```

## Development Conventions
*   **Architecture:** The project uses the standard SwiftUI App lifecycle.
*   **Concurrency:** Utilizes Swift Concurrency (likely `MainActor` for UI updates).
*   **Previews:** Xcode Previews are enabled and encouraged for UI development (see `#Preview` in `ContentView.swift`).
*   **Code Style:** Follows standard Swift API Design Guidelines.

# Hospital Management App (Flutter)



## Project Overview

This is a Flutter-based mobile application designed for hospital management. The current development focus is on implementing a robust authentication and registration system for various user roles within the hospital environment.

## User Roles

-   **Patients**: Can register and log in to the application.
-   **Doctors**: Can log in.
-   **Admins**: Can log in.
-   **Nurses**: Can log in.
-   **Secretaries**: Can log in.

## Features Implemented (Initial Phase)

### 1. Authentication (Login)

-   **Login Screen** (`lib/features/auth/screens/login_screen.dart`):
    -   Allows users (Patients, Doctors, Admins, Nurses, Secretaries) to log in.
    -   Input fields for Email and Password.
    -   Dropdown selector for User Type.
    -   Basic input validation.
    -   Navigation to the Signup screen for new patients.
    -   Modern UI design with clear visual elements.

    ![Singin](./images/Singin.png)

### 2. Patient Registration (Signup)

-   **Signup Screen** (`lib/features/auth/screens/signup_screen.dart`):
    -   Specifically for new patient registration.
    -   Input fields for:
        -   Full Name
        -   Email
        -   Password (with confirmation)
        -   Phone Number
        -   Date of Birth (with a native date picker)
        -   Gender (dropdown selector)
    -   Comprehensive input validation for all fields.
    -   Modern UI design consistent with the Login screen.
    -   Navigation back to the Login screen.

![Singup](./images/Singup.png)

### 3. Core Structure

-   **Authentication Service** (`lib/features/auth/services/auth_service.dart`):
    -   Contains placeholder methods for `signInUser` and `signUpPatient`.
    -   This service will eventually handle communication with the backend for authentication logic.
-   **Routing** (`lib/router.dart`):
    -   Manages navigation between screens (Login, Signup).
-   **Main Application Setup** (`lib/main.dart`):
    -   Initializes the Flutter application and sets the Login screen as the initial route.

## Project Structure (Key Directories)

```
lib/
├── features/
│   └── auth/
│       ├── screens/      # UI for login and signup
│       │   ├── login_screen.dart
│       │   └── signup_screen.dart
│       ├── services/     # Business logic for authentication
│       │   └── auth_service.dart
│       └── widgets/      # Reusable auth-related widgets (if any in future)
├── router.dart         # App navigation
└── main.dart           # Main application entry point
docs/
└── images/
    ├── Singin.png
    └── signup.png
```

## How to Run the Project

1.  **Ensure Flutter is installed and configured:**
    -   Follow the official Flutter installation guide: [https://flutter.dev/docs/get-started/install](https://flutter.dev/docs/get-started/install)
    -   Make sure the Flutter SDK `bin` directory is added to your system's PATH.
2.  **Connect a device or start an emulator/simulator.**
3.  **Open the project in your IDE (VS Code, Android Studio) or a terminal.**
4.  **Navigate to the project root directory.**
5.  **Run the command:** `flutter run`


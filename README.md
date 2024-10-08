# To-Do List App

This is a **Flutter-based To-Do List App** where users can manage their daily tasks efficiently. The app allows users to create, edit, delete, and mark tasks as complete. The app also includes a static profile picture for the user within the interface.

## Table of Contents
- [Features](#features)
- [Screenshots](#screenshots)
- [Installation](#installation)
- [How to Use](#how-to-use)
- [Customization](#customization)
  - [Setting Profile Picture](#setting-profile-picture)
- [Dependencies](#dependencies)
- [Contributing](#contributing)
- [License](#license)

## Features
- **Add To-Do Items**: Users can add new to-do items.
- **Edit To-Do Items**: Update existing tasks.
- **Delete To-Do Items**: Remove tasks that are no longer needed.
- **Mark Complete**: Check-off tasks when done.
- **Profile Picture**: Static profile picture is displayed inside the app.
- **Clean UI**: Intuitive user interface for easy task management.

## Screenshots
| Home Screen | Adding a Task | Task Completed |
| --- | --- | --- |
| ![Home Screen](path/to/home_screenshot.png) | ![Add Task](path/to/add_task_screenshot.png) | ![Task Completed](path/to/task_completed_screenshot.png) |

## Installation

### Prerequisites
- Ensure that you have [Flutter](https://flutter.dev/docs/get-started/install) installed on your machine.
- Android Studio or Visual Studio Code is recommended for development.
- An emulator or physical device to run the app.

### Steps
1. **Clone the Repository**:
    ```bash
    git clone https://github.com/yourusername/todo_list_app.git
    ```
2. **Navigate to Project Directory**:
    ```bash
    cd todo_list_app
    ```
3. **Install Dependencies**:
    Run the following command to install all the necessary packages:
    ```bash
    flutter pub get
    ```
4. **Run the App**:
    To start the app on an emulator or physical device, run:
    ```bash
    flutter run
    ```

## How to Use
1. **Add a Task**: Tap the `+` button at the bottom right to add a new to-do item. Type in your task and save.
2. **Mark Complete**: Check the box next to any task to mark it as completed.
3. **Delete a Task**: Tap the red trash icon to delete a task.
4. **Static Profile Picture**: A static profile picture is displayed on the top right inside the app interface.

## Customization

### Setting Profile Picture
To set your static profile picture:

1. **Prepare the Image**: Place your profile image in the `assets/images/` folder. Ensure the image name matches the one you want to use, for example, `profile_picture.png`.

2. **Register the Asset**: Ensure that `pubspec.yaml` includes:
   ```yaml
   flutter:
     assets:
       - assets/images/profile_picture.png
   ```

3. **Code Reference**: In your code, set the image source as:
   ```dart
   CircleAvatar(
     backgroundImage: AssetImage('assets/images/profile_picture.png'),
   );
   ```

## Dependencies
This project uses the following Flutter dependencies:
- `flutter` SDK
- `provider`: Used for state management.
- `flutter_local_notifications`: To add reminders/notifications.
- `shared_preferences`: For persisting to-do items.

Make sure these dependencies are listed in `pubspec.yaml`:
```yaml
dependencies:
  flutter:
    sdk: flutter
  provider: ^6.0.0
  shared_preferences: ^2.0.6
  flutter_local_notifications: ^9.2.0
```

## Contributing
Contributions are welcome! Feel free to fork the repository and submit a pull request. Please ensure your changes follow the standard Flutter coding practices and are well-tested.

1. Fork the project.
2. Create your feature branch:
    ```bash
    git checkout -b feature/YourFeature
    ```
3. Commit your changes:
    ```bash
    git commit -m 'Add YourFeature'
    ```
4. Push to the branch:
    ```bash
    git push origin feature/YourFeature
    ```
5. Open a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE] file for details.

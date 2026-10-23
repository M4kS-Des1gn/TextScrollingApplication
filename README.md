# ScrollingText

## 📱 About the Project

**ScrollingText** is a simple Android application developed in Java using Android Studio. The application displays an article about *Beatles Anthology Vol. 1* in a vertically scrollable layout.

The app demonstrates how to use Android UI components such as `ScrollView`, `LinearLayout`, `TextView`, and `Button`. It also shows how to handle button clicks and display a short confirmation message using a `Toast`.

## ✨ Features

- **Scrollable content:** Read the entire article by scrolling vertically.
- **Article title:** Displays the main title in large, bold text.
- **Article subtitle:** Displays a subtitle alongside the article text.
- **Readable layout:** Uses padding, margins, line spacing, and text styling.
- **Submit Comment button:** Displays a confirmation message when clicked.
- **Edge-to-edge layout support:** Handles system bar insets to position the content correctly.

## 🛠️ Technologies Used

- **Language:** Java
- **UI Design:** Android XML
- **IDE:** Android Studio
- **Android Components:** `ScrollView`, `LinearLayout`, `TextView`, `Button`, and `Toast`
- **Android Libraries:** AndroidX AppCompat and AndroidX Core

## 📂 Project Structure

```text
ScrollingText/
├── app/
│   └── src/
│       └── main/
│           ├── java/
│           │   └── com/example/
│           │       └── textscrollingapplication/
│           │           └── MainActivity.java
│           ├── res/
│           │   ├── layout/
│           │   │   └── activity_main.xml
│           │   └── values/
│           │       └── strings.xml
│           └── AndroidManifest.xml
├── build.gradle
├── settings.gradle
└── README.md
```

*Note: The exact Gradle file locations may vary depending on the Android Studio project configuration.*

## ⚙️ How It Works

### 1. Scrollable Article

The main layout uses a `ScrollView` to allow users to scroll through the article. Since a `ScrollView` supports one direct child, a vertical `LinearLayout` contains the title, subtitle, article text, and button.

### 2. Article Content

The article title, subtitle, article text, and button labels are stored in `strings.xml`. This separates the displayed text from the XML layout and makes the content easier to maintain.

### 3. Submit Comment Button

When the user clicks the **Submit Comment** button, Android calls the `submitComment(View view)` method in `MainActivity.java`.

The method displays a short confirmation message:

```java
Toast.makeText(
    this,
    R.string.comment_submitted,
    Toast.LENGTH_SHORT
).show();
```

The button currently displays a confirmation message only. It does not send or save an actual comment.

### 4. System Bar Insets

The application uses AndroidX edge-to-edge support and a window insets listener to adjust the layout for system bars.

## 🚀 Getting Started

1. Clone or download this repository.
2. Open Android Studio.
3. Select **Open** and choose the project folder.
4. Wait for Gradle synchronization to finish.
5. Connect an Android device or start an Android emulator.
6. Click **Run** to build and launch the application.

## 🎯 Learning Objectives

This project demonstrates how to:

- Create Android layouts using XML.
- Arrange UI components vertically and horizontally with `LinearLayout`.
- Display long text inside a `ScrollView`.
- Customize text size, style, padding, margins, and line spacing.
- Store UI text in Android string resources.
- Handle button clicks using the `android:onClick` attribute.
- Display feedback messages using `Toast`.
- Apply edge-to-edge layout handling with AndroidX.

<img width="432" height="891" alt="Screenshot1" src="https://github.com/user-attachments/assets/fb88f406-44c0-4993-8e1a-7253a9dc3879" />
<img width="438" height="892" alt="Screenshot3" src="https://github.com/user-attachments/assets/e508cc0f-7b81-417c-af96-8ef093c38bd9" />
<img width="442" height="886" alt="Screenshot2" src="https://github.com/user-attachments/assets/7caad8b9-1c46-49b5-a2e5-e452a4a1edf2" />


## 👨‍💻 Author
Maks Rakuša


Created as an Android development learning project.

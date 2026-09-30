# MAD Experiment 8 – WebView and Menu Application

## Student Details

**Name:** Md Atiullah Ansari  
**USN:** [25MCAR0108]  
**Course:** Mobile Application Development  
**Experiment:** 8 – WebView and Menu Application  

---

## Aim

To develop an Android application using Kotlin that demonstrates the use of WebView, Options Menu, Popup Menu, Fragments, image display, and bottom navigation.

---

## Objective

The objective of this experiment is to understand how Android applications can:

- Display images in an application.
- Use Fragments for different screens.
- Display a website using WebView.
- Create and use an Options Menu.
- Create and use a Popup Menu.
- Navigate between different fragments.
- Load a website such as JAIN University inside the application.

---

## Concept / Technology Used

### 1. WebView

WebView is an Android component used to display web pages inside an Android application without opening an external browser.

In this experiment, WebView is used to load the JAIN University website:

`https://www.jainuniversity.ac.in/`

### 2. Options Menu

The Options Menu is displayed from the top-right menu of the application.

It contains:

- Select All
- Share

### 3. Popup Menu

The Popup Menu is displayed from the Image Options button.

It contains:

- Select All
- Share
- Edit
- Delete

### 4. Fragments

The application uses fragments to separate different screens:

- Images Fragment
- WebView Fragment

### 5. Bottom Navigation

The application can use bottom navigation to switch between the Images and WebView sections.

---

## Scenario

Develop an Android application that demonstrates image handling, menus, fragments, and WebView.

The first screen displays images in the Images Fragment. The application provides image options such as Select All, Share, Edit, and Delete using a Popup Menu.

The application also provides an Options Menu at the top-right corner with Select All and Share options.

When the WebView section is selected, the second fragment opens and displays the JAIN University website inside the application using WebView.

---

## Requirements

### Software Requirements

- Android Studio
- Kotlin
- Android SDK
- Gradle
- Internet Connection

### Hardware Requirements

- Computer/Laptop
- Android Emulator or Android Smartphone

---

## Main Features

1. Images Fragment
2. Multiple image display
3. Popup Menu
4. Options Menu
5. WebView Fragment
6. JAIN University website loading
7. Fragment navigation
8. Internet permission

---

## Application Screens

### 1. Images Fragment

The Images Fragment displays the images used in the application.

![Images Fragment](./Screenshots/01_images_fragment.png)

---

### 2. Images Selected / Menu Output

This screen demonstrates the image selection/menu functionality.

![Images Selected](./Screenshots/02_images_selected.png)

---

### 3. WebView Fragment

The WebView Fragment displays a web page inside the Android application.

![WebView Fragment](./Screenshots/03_webview_fragment.png)

---

### 4. JAIN University WebView

The JAIN University website is loaded inside the application's WebView.

![JAIN University WebView](./Screenshots/04_jain_university_webview.png)

---

## Procedure

1. Open Android Studio.
2. Create an Android project using Kotlin.
3. Create the required Activities and Fragments.
4. Add the required images to the drawable resources.
5. Create the Images Fragment.
6. Display the images using ImageView.
7. Create an Options Menu using a menu XML file.
8. Add Select All and Share options.
9. Create a Popup Menu.
10. Add Select All, Share, Edit, and Delete options.
11. Create the WebView Fragment.
12. Add WebView to the fragment layout.
13. Add Internet permission in AndroidManifest.xml.
14. Enable JavaScript if required.
15. Load the JAIN University website using WebView.
16. Run the application on an emulator or Android device.
17. Test all menu and WebView operations.

---

# Test Cases

## Test Case 1 – Images Fragment

**Test Case:** Verify that the Images Fragment displays the required images.

**Steps:**
1. Launch the application.
2. Open the Images Fragment.
3. Check the displayed images.

**Expected Result:**  
The Images Fragment should open successfully and display the required images.

**Output:**  
Images are displayed correctly.

---

## Test Case 2 – Popup Menu

**Test Case:** Verify that the Popup Menu displays the required options.

**Steps:**
1. Open the Images Fragment.
2. Click the Image Options button.
3. Check the Popup Menu.

**Expected Result:**  
The Popup Menu should display:

- Select All
- Share
- Edit
- Delete

**Output:**  
All Popup Menu options are displayed correctly.

---

## Test Case 3 – WebView

**Test Case:** Verify that the WebView loads the JAIN University website.

**Steps:**
1. Open the WebView section.
2. Wait for the webpage to load.
3. Check the displayed webpage.

**Expected Result:**  
The JAIN University website should be displayed inside the Android application.

**Output:**  
JAIN University website is successfully loaded in WebView.

---

## Options Menu

The top-right Options Menu provides the following options:

| Option | Function |
|---|---|
| Select All | Selects all available images |
| Share | Shares the selected images |

---

## Popup Menu

The Image Options Popup Menu provides:

| Option | Function |
|---|---|
| Select All | Selects all images |
| Share | Shares the images |
| Edit | Provides edit functionality |
| Delete | Provides delete functionality |

---

# Folder Structure

```text
MAD-Experiment-8-WebView-Menu-Final/
│
├── .idea/
│
├── app/
│   └── src/
│       └── main/
│           ├── java/
│           │   └── com/
│           │       └── example/
│           │           └── webviewmenuapp/
│           │               ├── MainActivity.kt
│           │               ├── ImagesFragment.kt
│           │               └── WebViewFragment.kt
│           │
│           ├── res/
│           │   ├── drawable/
│           │   │   ├── phone_image_1.jpg
│           │   │   ├── phone_image_2.jpg
│           │   │   ├── phone_image_3.jpg
│           │   │   ├── storage_image_1.jpg
│           │   │   ├── storage_image_2.jpg
│           │   │   ├── storage_image_3.jpg
│           │   │   ├── url_image_1.jpg
│           │   │   ├── url_image_2.jpg
│           │   │   └── url_image_3.jpg
│           │   │
│           │   ├── layout/
│           │   │   ├── activity_main.xml
│           │   │   ├── fragment_images.xml
│           │   │   └── fragment_web_view.xml
│           │   │
│           │   └── menu/
│           │       ├── main_menu.xml
│           │       └── bottom_nav_menu.xml
│           │
│           └── AndroidManifest.xml
│
├── gradle/
│
├── Screenshots/
│   ├── 01_images_fragment.png
│   ├── 02_images_selected.png
│   ├── 03_webview_fragment.png
│   └── 04_jain_university_webview.png
│
├── .gitignore
├── README.md
├── build.gradle.kts
├── gradle.properties
├── gradlew
├── gradlew.bat
└── settings.gradle.kts

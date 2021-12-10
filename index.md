# Notifications / Firebase Cloud Messaging – Android

## Overview

This tutorial is a simple application that uses the user interface of Notifications from Android, and Cloud Messaging services from Firebase in Kotlin. Firebase – Cloud Messaging (FCM) is a solution for sending messages across devices, and notification across platforms for free. In this project, we will show how to create a notification and send a message using this service.

<p align="center">
  <img src="images/virtual_phone.JPG" width="252" alt="Sublime's custom image" />
  <img src="images/virtual_phone2.JPG" width="250" />
</p>

<p align="center">
  Figure 1. Final product. Notification box on the left, and notification layout on the right.
</p>

## Getting Started

We will be using Android Studio. To download it, go to this link: (https://developer.android.com/studio)

**Step 1:** Open Android Studio. Create a new project by clicking on New Project. Then select *Empty Activity.*

<p align="center">
  <img src="images/Android_studio2.JPG" width="800" alt="Sublime's custom image" />
</p>
<p align="center">
  Figure 2. Select Empty Activity
</p>

**Step 2:** Give it a name, which in this case I chose *NotificationFirebaseMessagingDemo*. A desired Package name. Choose Language Kotlin, and a Minimum SDK of API 28: Android 9.0 (Pie), and press Finish.

**Step 3:** Connect our app to Firebase. Simply go to (https://console.firebase.google.com) with your google account and create a new project. Follow the steps until you get a message saying: *“Your new project is ready”*, and press the Continue button.

**Step 4:** Once your project is created click on the Android logo near the middle level of “Project Overview” page.

**Step 5:** Now, let’s give it a desired package name. I chose “CIS357FinalProject”. You can leave empty the fields of App nickname (optional), and Debug signing certificate SHA-1 (optional). Make sure it matches the package identifier in your project’s manifest.xml. Click on Register app button.

**Step 6:** Download the google-services.json file to your gradle build directory (the app sub-directory.) as shown in figure 3. Then, click on Next button.

<p align="center">
  <img src="images/Firebase3.JPG" width="700" alt="Sublime's custom image" />
</p>
<p align="center">
  Figure 3. Download the JSON file.
</p>

**Step 7:** Add the following to your Project-level **build.gradle.**

<p>classpath <span style="color:green"> 'com.google.gms:google-services:4.3.10'</span>.</p>

**Step 8:** Add the following at the bottom of your App-level build.graddle.
  <p>apply <span style="color:green"> plugin: 'com.android.application'</span>.</p>
  <p>apply <span style="color:green"> plugin: 'com.google.gms.google-services'</span>.</p>

**Step 9:** Add the following inside of the dependencies block of your App-level build.graddle.
  <p>implementation <span style="color:green"> 'com.google.firebase:firebase-messaging-ktx'</span>.</p>
  <p>implementation <span style="color:green">'com.google.firebase:firebase-messaging-ktx:23.0.0'</span>.</p>
  <p>implementation <span style="color:green">'com.google.firebase:firebase-analytics-ktx'</span>.</p>

**Step 10:** Finally, press “Sync now” at the top right corner in the bar that appears in the IDE. Then, press the Next and Continue to console buttons. Now we are ready to start coding.
  
## Step-by-step Coding Instructions
 
Let’s begin by modifying the layout file.

**Step 11:** Open activity_main.xml, which can be found within the layout folder. Let’s customize the default Text View with the following values:

```kotlin
<TextView
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:text="Welcome to Final Demo App!"
    android:textSize="40dp"
    android:padding="20dp"
    android:textColor="#6320EE"
    android:textStyle="bold"
    app:layout_constraintBottom_toBottomOf="parent"
    app:layout_constraintLeft_toLeftOf="parent"
    app:layout_constraintRight_toRightOf="parent"
    app:layout_constraintTop_toTopOf="parent" />
```

```Android
<TextView
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:text="Welcome to Final Demo App!"
    android:textSize="40dp"
    android:padding="20dp"
    android:textColor="#6320EE"
    android:textStyle="bold"
    app:layout_constraintBottom_toBottomOf="parent"
    app:layout_constraintLeft_toLeftOf="parent"
    app:layout_constraintRight_toRightOf="parent"
    app:layout_constraintTop_toTopOf="parent" />
```
Of course, customize it with your desired text and textColor. You will obtain this:
<p align="center">
  <img src="images/Android_studio3.JPG" width="700" alt="Sublime's custom image" />
</p>
 
 
 
 
```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/JhosephR/CIS357_FinalProjectDemo/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.

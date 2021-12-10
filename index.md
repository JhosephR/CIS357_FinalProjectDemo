# Notifications / Firebase Cloud Messaging – Android

## Overview

This tutorial is a simple application that uses the user interface of Notifications from Android, and Cloud Messaging services from Firebase in Kotlin. Firebase – Cloud Messaging (FCM) is a solution for sending messages across devices, and notification across platforms for free. In this project, we will show how to create a notification and send a message using this service.

<p float="left">
  <img src="images/virtual_phone.JPG" width="252" />
  <img src="images/virtual_phone2.JPG" width="250" />
</p>
**Figure 1. Final product. Notification box on the left, and notification layout on the right.** 

## Getting Started

We will be using Android Studio. To download it, go to this link: (https://developer.android.com/studio)

**Step 1:** Open Android Studio. Create a new project by clicking on New Project. Then select *Empty Activity.*

<p float="center">
  <img src="images/Android_studio2.JPG" width="800" alt="Sublime's custom image" />
</p>
**Figure 2. Select Empty Activity**

**Step 2:** Give it a name, which in this case I chose *NotificationFirebaseMessagingDemo*. A desired Package name. Choose Language Kotlin, and a Minimum SDK of API 28: Android 9.0 (Pie), and press Finish.

**Step 3:** Connect our app to Firebase. Simply go to (https://console.firebase.google.com) with your google account and create a new project. Follow the steps until you get a message saying: *“Your new project is ready”*, and press the Continue button.

Step 4: Once your project is created click on the Android logo near the middle level of “Project Overview” page.

Step 5: Now, let’s give it a desired package name. I chose “CIS357FinalProject”. You can leave empty the fields of App nickname (optional), and Debug signing certificate SHA-1 (optional). Make sure it matches the package identifier in your project’s manifest.xml. Click on Register app button.

Step 6: Download the google-services.json file to your gradle build directory (the app sub-directory.) as shown in figure 3. Then, click on Next button.



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

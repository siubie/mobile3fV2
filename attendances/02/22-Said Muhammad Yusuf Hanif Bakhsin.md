Rangkuman Pertemuan 2


W01 Intro Android and Android Fundamentals

Android is a Software Stack for mobile devices SDK provides tools and APIs to develop apps Application is Ships with core set of apps written in java.
Main Components of Android :
- Activities 
- Services 
- Content Providers 
- Broadcast Receivers

W02 Activities and Intents

What is an Activity?
- An Activity is an application component
- Represents one window, one hierarchy of views
- Typically fills the screen, but can be embedded in other activity or a appear as floating window
- Java class, typically one activity in one file
What does an Activity do?
- Represents an activity, such as ordering groceries, sending email, or getting directions
- Handles user interactions, such as button clicks, text entry, or login verification
- Can start other activities in the same or other apps
- Has a life cycle—is created, started, runs, is paused, resumed, stopped, and destroyed
Implement new Activities
1. Define layout in XML
2. Define Activity Java class
    - extends AppCompatActivity
3. Connect Activity with Layout
    - Set content view in onCreate()
4. Declare Activity in the Android manifest

What is an Intent?
An intent is a description of an operation to be performed.
An Intent is an object used to request an action from another app component via the Android system. 
What can intents do?
● Start activities
  - A button click starts a new activity for text entry
  - Clicking Share opens an app that allows you to post a photo
● Start services
  - Initiate downloading a file in the background
● Deliver broadcasts
  - The system informs everybody that the phone is now charging

## NGO - Cordova Activity 1
ITCC 41 - MOBILE APPLICATION DEVELOPEMENT 



# Project Description
The Student Profile app is a mobile project made with Apache Cordova. It also uses HTML, CSS, and JavaScript.

With this app, students can make their own profile. They can open it later and change details when they need to. The screens are kept simple so users do not get stuck.

On the main screen, the app shows key info. This includes the student name, course, year level, profile photo, a short bio, and a list of skills. There is also an Edit Profile button for updating these items.

JavaScript runs the main actions. It reads what the user types, checks the form, saves changes, and handles canceling. After saving, it refreshes what the user sees on the screen.

To keep the data, the app uses localStorage. The profile stays on the device even if the app is closed. When the app opens again, the saved info is still there.

The layout uses responsive CSS. The design can fit different screens. It works on desktop, tablets, and phones.

In general, this Student Profile project shows how web tools plus Cordova can create a working mobile app. It includes profile editing, saved data, and a layout that adjusts to screen size.




# Application Pages

Profile

This Profile page is the main screen in the app. It shows the student’s basic details. You can see the name, course, year level, a profile image, and a short personal note. The page also lets the student change those details and save updates.

About

The About page shares more about the student. It has a short write-up. It talks about the student’s background, what they like, their aims, and other personal facts.

Skills

The Skills page lists what the student is good at. It can include both technical and social skills. Examples are programming, web work, database tasks, communication, teamwork, and solving problems.

Projects

The Projects page shows what the student has done. Each project or activity has a short summary. This part also helps show how the student uses their skills and technical knowledge.

Contact

The Contact page is for reaching the student. It may show an email address, a phone number, or other contact details that fit the situation.


# Profile Editing


The app lets a student change items in their profile. This includes the name, course, year level, a short bio, and a list of skills.  
When the student taps Edit Profile, a form shows up. It already has the saved values.  
The student can update the fields. Then they choose Save to keep the changes, or Cancel to leave everything as it was.

Local Data Storage

The app uses localStorage to hold the profile details. The data is saved inside the browser or the device.  
After the student clicks Save, JavaScript writes the new profile values to localStorage.  
Later, when the app is opened again, it pulls the stored data back and shows it.  
So the profile stays there even after closing the app and starting it again.

#  Camera Integration

The app relies on a Cordova camera plugin. It lets the person open the device camera and take a picture for the student profile.

When the user taps the camera option, the app asks for permission to use the camera. Once the photo is taken, the app stores the captured image so it can be used as the student profile photo.

The camera work is done in JavaScript. It uses the Cordova Camera API and then handles what the device sends back. This shows that Cordova can let web code like HTML, CSS, and JavaScript reach native device features.

The user taps the option to change their profile photo.  

Next, the Cordova camera plugin brings up the device camera.  

Then the user takes a picture with the camera.  

After that, the app receives the photo and shows it as the new profile picture.


# Device Feature Integration

Cordova lets the app use the phone camera. It does this by letting a web app made with HTML, CSS, and JavaScript tap into device features that normally belong to native apps.

With the Cordova Camera plugin, the app can talk to the built in camera. It can then take a picture and save it for use in the app.

That is why the Student Profile app can do things like launch the camera, take a photo, and change the user profile image. It can offer these options without having to build the whole app with native mobile code.

# Image Handling

When the user takes a photo with the camera, the Cordova Camera plugin sends that image back to the app. Then JavaScript takes the data and changes the profile photo that the Profile page shows.

The app also stores the same image in localStorage. Because of that, the chosen picture stays after the user closes the app. When the app is opened again, JavaScript loads the saved image and shows it as the current profile picture.

# Error Handling

The app is built with error checks so the camera flow stays stable on the device.

If the camera permission is blocked, the app notices the denial and shows a clear message. It does not crash.

If the camera screen opens and then the user backs out without a photo, nothing changes. The current profile image stays as it was.

If a camera problem happens that the app did not expect, it catches the issue and tells the user the picture could not be saved. The profile image also stays the same.

 # Responsive Design

 The app uses responsive CSS so the Student Profile page displays well on different screens.

Desktop: The design makes use of the full screen. Sections, images, buttons, and text keep good sizes for larger displays.

Tablet: The page changes its width and spacing as the screen gets smaller. Elements resize so the content stays readable and simple to use.

Mobile: The layout is flexible for small screens. Buttons, text, images, and profile parts shift to avoid side scrolling. Navigation stays easy.

With responsive layout rules, flexible sizing, and CSS media queries, the app aims for a steady, smooth experience on desktop, tablet, and mobile.


# How to Run

Follow the below steps to install, configure, build, and run the Student Profile Cordova application.

1. Installing Dependencies

First, make sure the computer has Node.js and Apache Cordova installed.

To test the installation, open the command prompt and execute the below commands.

node --version

npm --version

cordova --version

Change the directory to the project folder.

cd C:\CordovaProjects\Ong_Project_Cordova

Finally, run the below command to install the project dependencies

npm install

2. Configuring the Cordova Project

The project structure should have the following files and folders

config.xml – This file has the application Cordova configuration and platform details

package.json – This file has the project dependencies

www – This folder contains the project source code

index.html – This file has the HTML code for the application

css – This folder contains the CSS files for the application

js – This folder contains the JavaScript files for the application

img – This folder has the project images

3. Installing and Configuring the Camera Plugin

Run the below command to install the Cordova Camera plugin

cordova plugin add cordova-plugin-camera

Verify the plugin by running the below command

cordova plugin list

The Camera plugin will enable the application to access the device camera, take photos, and update the profile picture.

4. Adding the Android Platform

Run the below command to add the android platform

cordova platform add android

View the list of available platforms by executing the command below

cordova platform list

5. Building the Application

Execute the command below to build the Android application

cordova build android

If the command runs successfully, it will generate the android application file in the project folder/platforms/android.

6. Running the Application

Connect the android device to the computer using a USB cable. Additionally, make sure the device has enabled USB Debugging mode.

Alternatively, launch the android emulator from android studio and run the below command.

cordova run android

The command will build and run the application on the connected device.

7. Testing the Camera

Launch the application and perform the below tasks to confirm that the camera works.

Go to the Profile tab and click on Change Profile Picture tab

Grant the camera permission and capture a photo

Verify that the captured photo is the new profile picture

Close the application and reopen it to confirm that the profile picture has changed

If the camera permission is declined or the camera capture function is canceled, the application should retain the previous profile picture.


# Application Screenshots

<img width="1075" height="531" alt="Screenshot 2026-09-23 214153" src="https://github.com/user-attachments/assets/5b58aa2b-3136-43da-aa19-cfad03b133d1" />
<img width="1075" height="528" alt="Screenshot 2026-09-23 214144" src="https://github.com/user-attachments/assets/e5f65f6b-30b6-4b04-8fed-9a2879259eb1" />
<img width="1287" height="1007" alt="Screenshot 2026-09-23 214315" src="https://github.com/user-attachments/assets/13c28b27-9471-4a6a-9631-729cb492bde1" />
<img width="1293" height="1007" alt="Screenshot 2026-09-23 214308" src="https://github.com/user-attachments/assets/d27b5124-7af3-42fc-83e8-b7ba86123d80" />
<img width="1056" height="483" alt="image" src="https://github.com/user-attachments/assets/228b47e8-0ea9-4b36-9e75-576f4245f0a9" />


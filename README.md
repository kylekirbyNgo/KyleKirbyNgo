# Project Description
My project contains the complete Cordova project, and all five pages, and the necessary HTML,CSS, JAVASCRIPT, and the most important is the cordova project file.

## Application Pages
This app page has these parts.

- Profile
  Shows the student’s main details. You can see the photo, full name, course, and year level. There is also an **Edit Profile** button. It lets the student change their info.

- About 
  Gives a brief write-up of the student. It includes their interests, background, and goals.

- Skills 
  Lists the student’s skills in two types: technical and personal. Each skill is shown as its own item. This makes the list easier to scan.

- Projects  
  Displays the student’s projects that were made or finished. Every project has a title and a short description.

- Contact 
  Shows contact details like email and phone number. This helps users figure out how to reach the student fast.

  # Profile Editing

  The app includes an Edit Profile option. It lets a student change their own profile details inside the system.

When the student taps the Edit Profile button, the normal profile screen is replaced by an edit form.

The form lets the student update these items:
- Full Name
- Course
- Year Level
- About Me
- Skills

After the student fills in the form, JavaScript checks the required fields. It does this before the data is saved.

If the student chooses the Save button, the new details are stored in the browser’s localStorage. After that, the updated profile shows right away.

If the student presses Cancel, they can close the edit form. No changes are kept.

# JavaScript Functionality

JavaScript helps the Student Profile app respond to user actions. It also supports the Edit Profile feature.

First, JavaScript reads what the user types in the edit form. This includes the full name, course, year level, About Me, and the listed skills.

Next, it checks the required fields. If any required item is left blank, the app stops the save action and shows an error message.

After that, if the input is complete, the page updates the profile shown to the user. The app does not need to be restarted for the changes to appear.

Then, when the user clicks Save, the updated details get written to `localStorage`. Because of this, the information is still there after the app is closed and opened again.

Finally, if the user clicks Cancel, the edit form just closes. No new data is stored, so the last saved profile stays as it was.

 # Local Data Storage

 The app named Student Profile relies on the browser feature called `localStorage` to keep profile data.  

When you press the **Save** button, the JavaScript code turns the edited profile into JSON. Then it writes that JSON into `localStorage` under the key `studentProfile`.  

On load, the script looks in `localStorage` to see if `studentProfile` is already there. If it finds saved data, it pulls it out and shows it on the page. If nothing is found, it shows the default student profile instead.  

Because `localStorage` stores data in the browser, the saved profile stays there even if you close the app and open it again later.

# Responsive Design

The Student Profile app relies on responsive CSS so the pages look right on many screen sizes.

On a desktop, the screen has more room. The cards sit in the center, the spacing feels relaxed, and the profile photo looks bigger for quick reading.

On a tablet, the layout shifts to match the width you have. Text blocks may break into new lines. Even so, the cards and form controls stay clear and simple to use.

On a phone, the design gets tighter. The profile area uses smaller pieces, and the content stacks from top to bottom. The buttons stretch to fit the screen, so the Edit Profile form is easier to tap and read.

Media queries handle these changes. They update the layout and styles based on screen width.

 # How to Run

 Here is how to set up and start the Student Profile Cordova app.

1) Copy the repo to your machine

```bash
git clone 
cd 
```

2) Install what the project needs

```bash
npm install
```

3) Add the Android platform to the project

```bash
cordova platform add android
```

4) Compile the Android build

```bash
cordova build android
```

5) Start it on an emulator or a real phone

First, make sure you have an Android emulator running or an Android device connected. Then run:

```bash
cordova run android
```

If you prefer, you can open the Android project in Android Studio once the Android platform has been added.

This is the same set of steps you completed successfully earlier: `cordova platform add android` and `cordova run android`. 

# Application Screenshots
<img width="922" height="575" alt="image" src="https://github.com/user-attachments/assets/92a43162-501c-4f04-a04e-2226b0dd934b" />
<img width="922" height="571" alt="image" src="https://github.com/user-attachments/assets/b8e7cbe0-1767-4b73-b979-dea90c642525" />
<img width="1208" height="745" alt="image" src="https://github.com/user-attachments/assets/f64423b4-13e0-4714-beaa-7454649a4212" />
<img width="1277" height="366" alt="image" src="https://github.com/user-attachments/assets/c4a12418-dac6-47fd-a734-f8067fae176b" />





# Welcome to the ArtVista app 👋

  

This is an app created for the cross-platform exam at Kristiania College

  

**This app has been tested on iOS-simulator and web (Google Chrome)**


## Key feautures 🔑

  

* User Authentication: Secure login functionality for both loggin in, and creating a new user

  

* Upload artwork with title and description

  

* View userposts: browse through users posts to get a better view of the artwork, description and date of upload

  

  

## How to get started 🚦

  

**1.** Run this command in the terminal, to install the dependencies

  

```bash

npm  install

```

**Should the message "ConfigError: The expected package.json ´filename´.json does not exist" appear, simply right click the "x" circle in the terminal, and press "rerun command". This should allow for "npm i" to run successfully**
  

**2.** Start the app

  

```bash

npx  expo  start

```

  

**3.** Choose your browser

  

```bash

  

Press  "i"  to  open  the  iphone  simulator

  

```

  

```bash

  

Press  "w"  to  open  the  app  on  the  web

  

```

  

```bash

  

Press  "a"  to  open  the  app  on  the  android  simulator

  

```

  

**4.** Log in with verified credentials

  

For the purpose of viewing the app, log in to the app with the following credentials:

  

```bash

  

Username:  Test@gmail.com

  

Password:  Test123

  

```

  

## Features and functionality 🧰

  

### Authentication

* Authentication with the use of Firebase Authentication

* Each user is stored in the Firebase backend, with their email and date for registration

  

### Upload artwork

* Navigate to the Profile page, and find the image from your device, enter a title and description. **NOTE!** You will not be able to upload an image without filling in all three items (image, title, description)

* Wait for 2-3 seconds, and (if successful) the image will get uploaded into the Firebase Storage / Firestore database, and be available for viewing on the Home page

  

### View artworks

* All the uploads will be available from on the Home page. Press the artwork you would like to learn more about.

* Should the uploader like to delete the post, they can do so by pressing the "Delete post"-button. An alert will appear, notifying the user of the successful deletion of the post, and they will be redirected to the Home-page. **NOTE!** The deletion will also delete the post from Firebase, meaning it will not be able to recover the deleted post, should the user regret the decision.

  
  

## Dependencies 🛠

This app are using these dependencies:

*  **React Native**: Framework for developing cross-platform apps

*  **Expo**: Framework for creating React Native apps, with an extensive useful library

*  **Firebase**: Backend-as-a-Service (Baas) for the authentication, storage of posts and images

*  **Expo-Image-Picker**: Allowing users to chose images from their gallery

  

# References 📖

  

GitHub reference for code in ***firebaseConfig.js***

```bash

let  persistence;

if (Platform.OS  ===  "web") {

persistence  =  browserSessionPersistence;

} else {

persistence  =  getReactNativePersistence(ReactNativeAsyncStorage);

}

```

https://github.com/firebase/firebase-js-sdk/issues/7615

  

* Firebase documentation: https://firebase.google.com/docs

  

* Expo documentation: https://docs.expo.dev/

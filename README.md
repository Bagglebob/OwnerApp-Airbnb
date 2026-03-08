# OWNER_APP-Airbnb

A React Native mobile application for property owners to manage real estate listings. Built with Expo and Firebase, this app allows users to create, view, and manage property listings with ease.

## Overview

OWNER_APP-FAWAD is a property listing management application designed for property owners. It provides a user-friendly interface for creating new property listings, viewing existing listings, and managing account information.

## Features

- **User Authentication**: Secure login system using Firebase Authentication
- **Create Listings**: Add new property listings with details including:
  - Property title
  - Address and city
  - Number of rooms
  - Pool availability
  - Property images
  - Rental price
- **View Listings**: Browse and manage all property listings
- **User Profile**: View and manage user profile information
- **Responsive Design**: Optimized for mobile devices

## Tech Stack

- **Framework**: React Native (Expo)
- **Navigation**: React Navigation (Stack & Drawer)
- **Backend**: Firebase
  - Firebase Authentication
  - Cloud Firestore
- **Location Services**: Expo Location API
- **Language**: JavaScript

## Project Structure

```
OWNER_APP/
+-- App.js                    # Main application component, navigation setup
+-- index.js                  # Entry point
+-- firebaseConfig.js         # Firebase configuration
+-- app.json                  # Expo configuration
+-- package.json              # Project dependencies
+-- screens/
   +-- Login.js             # User authentication screen
   +-- CreateListing.js     # Property listing creation form
   +-- ViewListings.js      # Property listings display
+-- assets/                   # Images and static assets
```

## Prerequisites

- Node.js (v14 or higher)
- npm or yarn
- Expo CLI
- A Firebase project with Authentication and Firestore enabled

## Installation

1. **Clone the repository**
   `ssh
   git clone <repository-url>
   cd OWNER_APP-FAWAD
   `

2. **Install dependencies**
   `ssh
   npm install
   `

3. **Configure Firebase**
   - Add your Firebase credentials to firebaseConfig.js
   - Ensure Firebase Authentication and Cloud Firestore are enabled in your Firebase project

4. **Install Expo Go** (optional, required to preview on device)
   - Download from App Store or Google Play Store

## Running the Application

### Start the Expo development server
`ssh
npm start
`

### Run on Android
`ssh
npm run android
`

### Run on iOS
`ssh
npm run ios
`

### Run on Web
`ssh
npm run web
`

Once the server is running, scan the QR code with Expo Go app (mobile) or press the corresponding key in the terminal to run on your preferred platform.

## Key Dependencies

- expo: Framework and runtime environment
- react: Core React library
- react-native: React Native framework
- @react-navigation/native: Navigation library
- @react-navigation/drawer: Drawer navigation component
- @react-navigation/stack: Stack navigation component
- firebase: Firebase SDK
- expo-location: Device location services
- react-native-gesture-handler: Gesture handling for navigation

## Authentication Flow

1. User opens the app
2. If not logged in, user is directed to the Login screen
3. User enters email and password credentials
4. Firebase Authentication validates credentials
5. On successful login, user is granted access to the drawer navigation with:
   - Create Listing screen
   - View Listings screen

## Configuration

### Environment Variables
Create a .env.local file in the root directory with your Firebase configuration (optional for local development):
`
FIREBASE_API_KEY=your_api_key
FIREBASE_AUTH_DOMAIN=your_auth_domain
FIREBASE_PROJECT_ID=your_project_id
FIREBASE_STORAGE_BUCKET=your_storage_bucket
FIREBASE_MESSAGING_SENDER_ID=your_sender_id
FIREBASE_APP_ID=your_app_id
`

## Current Development Status

- Authentication structure implemented
- Navigation structure implemented
- Firebase integration
- Login functionality scaffolded
- Create Listing form in development
- View Listings functionality in development
- Firestore integration for data persistence

## TODO Items

- Implement complete form submission for property listings
- Add image upload functionality
- Implement property listing retrieval from Firestore
- Add profile management features
- Add property editing and deletion features
- Implement search and filter functionality

## Debugging

- Enable Element Inspector: Shake device and select "Show Element Inspector"
- Open Debugger: Shake device and select "Open Debugger"
- View Console Logs: Use the Expo developer menu to view logs
- Enable Fast Refresh: Automatically reload on file changes (enabled by default)

## License

This project is private. Unauthorized copying or distribution is prohibited.

## Author

Created by Fawad

## Support

For issues and bug reports, please create an issue in the project repository.

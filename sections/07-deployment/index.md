---
title: Deployment
has_children: false
nav_order: 8
---

# Deployment
The deployment of the **NewsNowBot** application requires specific steps and configurations before users can access it.
 
**Technologies Used**
 
-  **Frontend**: HTML, JavaScript, CSS
-  **Backend**: Firebase Authentication & Firestore (Serverless Architecture)
-  **Database**: Cloud Firestore
-  **Hosting**: Firebase Hosting
 
**System Requirements**
 
-  Node.js
-  Git
-  Visual Studio Code
-  Firebase CLI
 
**Prerequisites**
 
Before starting, ensure you have the following installed:
 
1. **Node.js**: Download and install from the [official Node.js website](https://nodejs.org/).
2. **Firebase CLI**: Install via npm:
```yaml
npm install -g firebase-tools
```
3. **Git**: Ensure Git is installed for version control.
 
**Deployment Instructions**
 
**1st Step: Clone the Repository**
 
Clone the GitHub repository using the following command:
```yaml
git clone <https://github.com/your-repo/newsnowbot.git>
cd newsnowbot
```
 
**2nd Step: Install Dependencies**
 
Run the following command to install the required dependencies:
```yaml
npm install
```
**3rd Step: Configure Firebase**
 
If you haven't already, initialize Firebase in your project:
```yaml
firebase login
firebase init
```
Select **Firestore, Authentication, and Hosting** during the setup process.
 
**Running the Application Locally**
 
To test the application locally, start a development server:
```yaml
firebase emulators:start  # Runs Firestore and Authentication locally
npm start  # Starts the front-end
```
 
**Deploying to Firebase Hosting**
 
To deploy the application to Firebase Hosting, use:
 
Once completed, Firebase provides a hosting URL where the application is accessible.
 
**Troubleshooting**
 
**1\. Firebase CLI Not Found**
 
If you receive a "command not found" error, try reinstalling Firebase CLI:
```yaml
npm install -g firebase-tools
```
 
**2\. Firestore Rules Issues**
 
Ensure Firestore security rules allow read/write access for authenticated users. Modify firestore.rules as needed:
 
```yaml
rules_version = '2';
service cloud.firestore {
 match /databases/{database}/documents {
   match /users/{userId} {
     allow read, write: if request.auth != null;
   }
 }
}
```
Deploy the updated rules with:
```yaml
firebase deploy --only firestore
```
 
**3\. Port Conflicts**
 
If port 5000 is already in use, start the local server on a different port:
 
```yaml
  npm start --port 5001
```
 
At this point, **NewsNowBot** should be fully operational, allowing users to browse news, comment, and interact with the platform.

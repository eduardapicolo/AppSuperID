# SuperID

**Integrative Project 3**  
_PUC Campinas – Software Engineering – 3rd Semester_

## Team Members:
- [Arthur Azevedo Locce Baptista](https://github.com/arthurlocce)  
- [Eduarda Picolo Barboza](https://github.com/eduardapicolo)  
- [Felipe Nonato Leoneli](https://github.com/lipeleoneli)  
- [Henrique Martins](https://github.com/HenriqueMartins2502)  
- [Sophia Franco de Godoy](https://github.com/sophiagodoy)

## About the Project

**SuperID** is a native Android application developed in Kotlin, with the main goal of providing secure and centralized credential management. Users can:

- Register and store encrypted passwords organized by categories (Websites, Applications, Devices, etc.).  
- Recover their “master password” via email in case of forgetting it.  
- Perform “passwordless login” on partner websites by scanning a QR Code.

To demonstrate the **passwordless login** flow, we created a **partner demonstration website** that generates the necessary QR Code and receives the authentication result, facilitating testing and validation.

## Technologies and Tools

### SuperID - Android Studio
- **Kotlin**  
- **Android Studio**  
- **Firebase Firestore**  
- **Firebase Authentication**  
- **Firebase Functions**  
- **VSCode**  
- **Git & GitHub**

### Partner Website - VSCode
- **TypeScript**  
- **JavaScript**  
- **HTML**  
- **CSS**

## How to Open and Run in Android Studio

1. **Clone the repository**
    ```bash
    git@github.com:sophiagodoy/PI3-Turma01-Grupo03.git
    ```

2. **Open Android Studio**  
   - Launch Android Studio and open the cloned project folder.

3. **Configure Firebase (Firestore + Authentication)**  
   - In the [Firebase Console](https://console.firebase.google.com/), create a new project.  
   - Enable **Firestore** and **Authentication**.  
   - Download the `google-services.json` configuration file and place it in the `app/` folder.

4. **Sync Gradle**  
   - In Android Studio, click **Sync Now** when prompted.  
   - Ensure there are no dependency errors.

5. **Run on emulator**  
   - Select an existing emulator or create a new one.  
   - Click **Run** to install and start the app on the emulator.

> **Note:** When creating or editing data in the app, you can monitor everything in real-time on Firestore and Authentication dashboards.

## How to Run on an Android Device

1. Connect an Android device via USB and enable **USB Debugging** in **Developer Options**;  
2. Select your device in Android Studio;  
3. Click **Run**; the app will be installed and executed directly on your device.

## Partner Website for Demonstration

1. Clone the first repository (Partner site which displays a login screen, where clicking the "login with SuperID" button generates a QR code that, when scanned by our app’s camera, shows a "Login successful" message):  
    ```bash
    git@github.com:HenriqueMartins2502/Site-parceiro-PI.git
    ```

2. Clone the second repository (Firebase Functions repo responsible for generating the QR Code in base64 and querying the database when the QR Code is scanned. You will need to configure Firebase Functions according to your OS). Run these two commands in the terminal:  
    ```bash
    npm install firebase-admin firebase-functions qrcode
    npm install --save-dev @types/qrcode
    ```
    ```bash
    git@github.com:HenriqueMartins2502/Firebase-functions-PI.git
    ```

3. Open the project in VSCode.

## Enjoy!

Have fun organizing and protecting your passwords with SuperID! 🚀🔒

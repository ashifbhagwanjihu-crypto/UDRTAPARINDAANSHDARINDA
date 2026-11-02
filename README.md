# UDRTAPARINDAANSHDARINDA Android starter

Modern-dark Android chat UI prototype built with Kotlin and Jetpack Compose. The supplied couple image is used as the login-screen background.

## Build an installable APK using GitHub Actions
1. Create a GitHub account (or sign in) and create a **public or private** repository named `UDRTAPARINDAANSHDARINDA`.
2. Upload all files and folders from this project to the repository's `main` branch.
3. Open the repository's **Actions** tab and select **Build Android APK**.
4. Tap **Run workflow** if it has not started automatically.
5. When the run finishes successfully, open that run and download the artifact named `UDRTAPARINDAANSHDARINDA-debug-apk`.
6. Extract the downloaded artifact ZIP and tap `app-debug.apk` on your Android phone to install it. Android may ask you to allow installs from that browser/file manager.

The workflow is in `.github/workflows/build-apk.yml` and builds the debug APK in GitHub's hosted Android build environment.

## Important current limitations
- Gmail sign-in is currently a **preview button**, not real Google authentication.
- Chat list and messages are sample/local UI data. Messages are not sent to other phones.
- Real multi-user messaging needs a Firebase project, Google sign-in configuration, Firestore security rules, and (for media) Firebase Storage. No account password or OTP should be shared.

# English LEARNING point — Android APK project

This wraps the supplied HTML app in a native Android shell using Capacitor.

## Build the APK from an Android phone (using GitHub Actions)

1. Sign in to GitHub in your phone browser and create a new **public or private repository** named `english-learning-point`.
2. Upload **all files and folders** from this project ZIP into the repository. Make sure `.github/workflows/build-apk.yml` is included. GitHub's mobile website may hide dot-folders; if so, use GitHub's browser upload flow that preserves hidden folders, or create the workflow file manually at `.github/workflows/build-apk.yml` using the contents in this ZIP.
3. Open the repository's **Actions** tab. Select **Build Android APK** and tap **Run workflow** (or wait for the first push build to finish).
4. Open the completed workflow run. Under **Artifacts**, download `English-LEARNING-point-debug-apk`.
5. Extract the downloaded artifact ZIP. Install `app-debug.apk` on your Android phone. If Android asks, allow installation from that browser/file manager.

## Important current limitations

- This is a debug APK for testing, not a Play Store release-signed APK.
- The supplied HTML app currently falls back to browser `localStorage`. Data stays on the same device/app installation and does not synchronize across teacher and student phones.
- A secure online backend, account authentication, and cloud file storage are needed before using it as a real multi-device tuition-management system.
- Change the default admin password before real use. Do not store real student information in this test build.

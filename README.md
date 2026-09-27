# Y.A.P CITY Android project

This repository is ready for GitHub Actions to build a release APK.

## Repository structure

Upload this folder's contents to the root of a GitHub repository. Keep the `android/` directory and `.github/workflows/build-android.yml` exactly where they are.

```text
.github/workflows/build-android.yml
android/
  settings.gradle.kts
  build.gradle.kts
  gradle.properties
  app/
    build.gradle.kts
    proguard-rules.pro
    src/main/AndroidManifest.xml
    src/main/java/com/yapcity/app/MainActivity.java
    src/main/res/drawable/yap_city_icon.png
    src/main/res/values/styles.xml
```

## Build the APK on GitHub

1. Push the files to GitHub.
2. Open **Actions**.
3. Select **Build Y.A.P CITY Android APK**.
4. Click **Run workflow**.
5. Open the completed run.
6. Download the **yap-city-apk** artifact.
7. The artifact contains `app-release.apk`.

The app currently opens:

`https://principles-scale-porcelain-calgary.trycloudflare.com`

Change `START_URL` in `android/app/src/main/java/com/yapcity/app/MainActivity.java` when you have a permanent domain.

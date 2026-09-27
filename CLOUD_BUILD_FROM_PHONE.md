# C.P.D SUPER WIZARD AI — Build the APK from a phone

This project is prepared for a cloud build. You do not need a PC or Android Studio.

## Free option: GitHub Actions

GitHub documents that standard GitHub-hosted runners are free for public repositories. GitHub Free personal accounts also include a monthly Actions allowance for private repositories. See the official GitHub Actions billing documentation for current limits.

### 1. Create a GitHub account

Open GitHub in your phone browser and create/sign in to your account.

### 2. Create a new PUBLIC repository

Create a repository named:

`cpd-super-wizard-ai`

Choose **Public**. Do not upload secrets, broker passwords, API keys, or Exness credentials.

### 3. Upload this project

Upload the contents of this project to the repository so that these files/folders are at the repository root:

- `settings.gradle`
- `build.gradle`
- `app/`
- `.github/workflows/build-apk.yml`

Do not put the whole project inside another folder level.

### 4. Start the cloud build

On GitHub, open the repository → **Actions** → **Build C.P.D SUPER WIZARD AI APK** → **Run workflow** → **Run workflow**.

GitHub Actions will build the Android debug APK in the cloud.

### 5. Download the APK

When the workflow shows a green check:

1. Open the completed workflow run.
2. Scroll to **Artifacts**.
3. Tap `CPD-SUPER-WIZARD-AI-Manual-v1.4-APK`.
4. Download the artifact ZIP.
5. Extract it on the phone.
6. Tap `app-debug.apk` and install it.

Android's build system packages Android source/resources into APKs; the workflow performs that build on GitHub's cloud runner.

## What this APK does

- Manual Mode: active.
- Automatic Mode: visible but locked.
- No automatic orders are sent.
- No Exness password is required.
- No API key is required.
- No PC/VPS is required to build the APK.

## Important

This is a debug/test APK. It is not a Play Store release package. Automatic trading remains disabled in this version.

# C.P.D SUPER WIZARD AI — Manual Mobile v1.3

Manual-only Android version for phone-first use.

## Included
- C.P.D SUPER WIZARD AI / V10.35 SMART AGGRESSIVE branding
- Manual BUY/SELL trade planner
- Entry, stop loss, take profit and notes
- Local Android manual alert notification
- Signal Center and activity log
- No automatic order execution
- No Exness password, API token, MT5 bridge or paid trading service required

## Not included yet
Live Exness prices and automatic execution are intentionally disabled. A phone-only live connection needs a supported market-data/execution service, which can be added later.

## Build
The project includes a GitHub Actions workflow that can build a debug APK in the cloud, so a PC is not required for the build itself.


## Trading modes
- **Manual Mode — ACTIVE:** the current working mode. Trade plans and local alerts are available.
- **Automatic Mode — LOCKED:** the button is visible so the app structure is ready for future automatic trading, but this version contains no automatic execution path. Selecting it immediately returns to Manual Mode.
- No broker password, API key, MT5 bridge, or automatic order execution is required for this version.

The Android project can later be extended with a separate, explicitly enabled automatic-trading implementation. Android build variants can also be used to separate configurations when the feature is ready.

## Build the APK from a phone

See `CLOUD_BUILD_FROM_PHONE.md`. The project includes a GitHub Actions workflow at `.github/workflows/build-apk.yml` that builds `app-debug.apk` in the cloud.

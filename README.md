# Lauren Tracker — native iPhone app source

## Included
- Native SwiftUI app (iOS 17+): dashboard, relationship timer, monthly/yearly anniversary countdowns, notes, photos, favorites, dates, spending, editable custom counters.
- Dark UI, pink accents, original heart app icon.
- On-device JSON persistence in Application Support, with migration from previous UserDefaults prototype.
- Tap an entry to edit it; swipe to delete. Add photos using Photos picker.

## IMPORTANT
This is a source project, **not an IPA**, and has **not been compiled on macOS/Xcode**. Installing on iPhone requires a Mac-based build and Apple signing. Do not purchase cloud services until they confirm support for your workflow. A free Personal Team installation generally expires after seven days. Keep iPhone backups: deleting the app can delete local data. The app does not yet have Face ID or encrypted storage.

## Build with Xcode (Mac or remote macOS)
1. Install a current Xcode supporting iOS 17+ and your phone's iOS version.
2. Install XcodeGen (https://github.com/yonaskolb/XcodeGen) and run `xcodegen generate` in this folder. Open `LaurenTracker.xcodeproj` in Xcode.
   **Without XcodeGen:** Create a new iOS App project named LaurenTracker (SwiftUI, Swift), remove generated ContentView and app entry point, add `LaurenTracker/LaurenTrackerApp.swift` and `Assets.xcassets` to the target.
3. Under Signing & Capabilities, select your Apple Personal Team and change the bundle ID to something unique.
4. Build and run on an iPhone connected to a Mac, or use a compatible cloud build + Windows sideload signing workflow. Cloud builds do not automatically guarantee a sideloadable unsigned IPA.
5. If the iPhone requests it, enable Developer Mode in Settings > Privacy & Security.

## Privacy
All information is manually entered and saved on-device; there is no server or account. Ask Lauren before storing private photos or personal information about her. Backup before reinstalling or changing signing identities.

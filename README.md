<div align="center">
  <h1>Keyguard Rotation Unlocker</h1>
  <p>
    <strong>Unlock screen rotation on your Android Lock Screen (Keyguard).</strong>
  </p>
</div>

## Description

This LSPosed module forces the Android Keyguard (Lock Screen) to respect the user's system-wide rotation settings.

By default, AOSP and many custom ROMs force the lock screen orientation to `NOSENSOR` (portrait fixed), regardless of your accelerometer or "Auto-rotate" toggle. This module hooks into `WindowManagerImpl` to override this behavior, allowing the lock screen to rotate freely.

### Why this module?
* **Android 16 (Baklava)** and newer versions where traditional method hooks might fail.
* Tablets or car head units where landscape lock screen is essential.
* Users who want rotation without patching `SystemUI.apk` manually.

## Requirements

* Android 8.0+ (Tested on Android 16)
* Root Access (Magisk / KernelSU / APatch)
* **LSPosed**

## Disclaimer

This module modifies system behavior. While safe, I am not responsible for any bootloops or issues that may occur. Always have a backup.

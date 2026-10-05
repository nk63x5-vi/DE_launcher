# DE Launcher

DE Launcher is a desktop-style Android workspace built on Mozilla Firefox for Android (Fenix). This README describes the current ARM64 debug build, version `1.0.2640`.

## Current features

- Desktop-style home screen with app search and shortcuts.
- Firefox-powered browser inside the launcher, with tab management, multiple in-app browser windows, browser settings, and a desktop-site preference.
- Built-in file manager. Choose a folder through Android's Storage Access Framework, then browse, create, rename, delete, and open files.
- Built-in plain-text editor for creating, opening, and saving text files.
- Browser split view for displaying two tabs side by side.
- Launch installed Android apps in Android's native freeform mode where the device supports it.

## Current limitations

- The built-in browser, file manager, and text editor use DE Launcher's own desktop windows.
- Window controls for third-party Android apps depend on the device's system freeform implementation. On the Sony Xperia 1 IV's simulated external display, apps can open in freeform mode, but Sony does not show title-bar controls or touch resize handles. DE Launcher does not yet include the Shizuku-based window-control integration planned for a later version.
- This debug APK is signed with a development key and is intended for testing.

## APK

- Package: `com.nk63x5.launcher_de`
- Version: `1.0.2640` (debug)
- ABI: `arm64-v8a`
- Minimum Android API: 26
- Target SDK: 37
- File: `de-launcher-arm64-debug.apk`
- SHA-256: `2e043b3cdb04f73bba7fb3557883b5113693f21a2e0a837dc2d761a428a1bd92`

Install from a computer with ADB:

```sh
adb install -r de-launcher-arm64-debug.apk
```

The APK is about 165 MiB, above GitHub's 100 MiB limit for a regular Git file. Publish it as a GitHub Release asset (or use Git LFS) rather than committing it directly to the repository.

## Source and license

The application is based on Mozilla Firefox for Android. Mozilla source files retain their Mozilla Public License 2.0 notices. Check the included `LICENSE` and third-party notices for the licenses that apply to the source and bundled dependencies.

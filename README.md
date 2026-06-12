# BookPlayer iOS 12

This is an unofficial fork of BookPlayer.

It is for personal maintenance and iOS 12 support.

It is not affiliated with, endorsed by, or maintained by BookPlayer LLC or TortugaPower.

It is not intended for App Store distribution.

## Build and install on a device

You need:

1. A Mac with macOS.
2. Xcode.
3. Your Apple ID added in Xcode.
4. A Lightning cable.
5. An iPhone, iPad, or iPod touch running iOS 12 or later.

Steps:

1. Connect the device to the Mac with the cable.
2. Unlock the device and tap Trust if iOS asks.
3. Open Terminal in this folder.
4. Run:

```sh
cp BuildConfiguration/Debug.template.xcconfig BuildConfiguration/Debug.xcconfig
open BookPlayer.xcodeproj
```

5. In Xcode, open `BuildConfiguration/Debug.xcconfig`.
6. Change `BP_BUNDLE_IDENTIFIER` to something unique, for example:

```text
com.yourname.bookplayerios12
```

7. Open Xcode account settings and add your Apple ID.
8. Select the BookPlayer scheme.
9. Select your connected device as the run device.
10. Open the project settings.
11. Select the BookPlayer target.
12. Open Signing and Capabilities.
13. Select your Apple ID team.
14. Repeat the same team choice for the extension targets if Xcode asks.
15. Press Run.
16. If the device blocks the app, open Settings, then General, then Device Management, then trust your Apple ID.
17. Press Run again.

The app should install on the iPod and open.

## If signing fails

Use a unique bundle identifier. Do not use the original BookPlayer bundle identifier.

If Xcode says a profile cannot be created, remove extra capabilities from the debug build or use a paid Apple Developer account.

If you use a free Apple Developer account, the installed app may stop opening after a few days. Build and run it again from Xcode.

## License

This fork keeps the original GPLv3 license.

See LICENSE for details.

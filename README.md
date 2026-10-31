# ბასი · BUS — download page

The public download page for ბასი (BUS), a free, nonprofit marshrutka app for Georgia by lunaviolab:
**https://zukajirashvili.github.io/basi/**

The app's source code is not here; this repository holds only the page, and each version's Android file is attached to a [release](https://github.com/zukajirashvili/basi/releases).

The download button always points to the newest release's `basi.apk`:
https://github.com/zukajirashvili/basi/releases/latest/download/basi.apk

## Publishing a new version

Build the APK (`eas build --profile preview --platform android` in the app folder), download it as `basi.apk`, then run in this folder:

```bash
gh release create v1.2.0 basi.apk --title "ბასი 1.2.0" --notes "What changed"
```

The page, the poster's QR code and every shared link pick it up at once; nothing else changes. Small fixes that ship as instant updates (`eas update`) need no new release.

Help: lunaviolab@gmail.com

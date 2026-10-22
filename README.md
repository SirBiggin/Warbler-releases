# Warbler — releases

Public download page for **Warbler**, a touch-first Monero wallet for Android.
Warbler is an unofficial fork of [Feather](https://github.com/feather-wallet/feather):
it reuses Feather's C++ wallet core and replaces the desktop UI with a mobile
Qt Quick interface. Not affiliated with or endorsed by the Feather project.

The source code is kept in a private repository; this repository only publishes builds.

## What it does

- Open, create or restore (from seed) Monero wallets; multiple accounts per wallet
- All network traffic goes through a **bundled Tor** — no Orbot needed, no clearnet fallback
- Connects to public remote nodes with automatic failover; sync keeps running while the phone is locked
- Send (with sweep-all), receive with a QR code, scan QR codes with the camera, transaction history
- XMR/USD price shown next to the balance

## Install

1. Open the latest entry under **Releases** and download the `.apk`.
2. Open it on your phone and allow installs from your browser or file manager if asked.
3. Updates install over the top of the previous version — no uninstall needed.

Requires Android 7.0 (API 24) or newer, 64-bit ARM (`arm64-v8a`). Built 16 KB
page-size compliant for Android 15+ devices.

For best results on Samsung phones, set Warbler's battery usage to
**Unrestricted** so background sync is not killed.

## Automatic updates

Add this repository's URL to [Obtainium](https://github.com/ImranR98/Obtainium) and it will
notify you when a new release appears.

## Notes

- This is early software. Test with small amounts first.
- Current builds are debug-signed; a future release will switch to a release key, which
  will require a one-time uninstall/reinstall.
- The wallet password is stored on-device (app-private storage) so the last wallet can
  reopen automatically; use **Close wallet** to forget it.

## Feedback

Open an issue here for bugs or requests.

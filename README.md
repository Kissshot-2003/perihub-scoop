# PeriHub Scoop Bucket

A [Scoop](https://scoop.sh) bucket for [PeriHub](https://github.com/hex-dump/perihub), an
open-source app to configure gaming peripherals on Windows and Linux without SteelSeries GG
or Logitech G HUB.

## Apps in this bucket

| App | Description |
| --- | --- |
| [perihub](bucket/perihub.json) | Configure the SteelSeries Apex 3 TKL keyboard and the Logitech G502 HERO mouse: lighting, key remapping, DPI, buttons and onboard profiles |

## How do I install these manifests?

```pwsh
scoop bucket add perihub-scoop https://github.com/Kissshot-2003/perihub-scoop
scoop install perihub-scoop/perihub
```

## How do I contribute new manifests?

Read the [Contributing Guide](https://github.com/ScoopInstaller/.github/blob/main/.github/CONTRIBUTING.md)
and the [App Manifests](https://github.com/ScoopInstaller/Scoop/wiki/App-Manifests) wiki page.

## Notes

PeriHub needs access to your HID devices, so it needs the WebView2 runtime. Windows 11 ships
it already; on Windows 10 install it with:

```pwsh
scoop install webview2
```

Update PeriHub through Scoop rather than its in-app updater, so the package stays managed
by Scoop:

```pwsh
scoop update perihub
```

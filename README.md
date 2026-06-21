# Sklink Smartboard Android Public Feed

This repository is the public update feed for the Android smartboard app.

## Purpose

- Host public APK files for installed smartboards
- Host `latest.json` consumed by the in-app updater
- Keep release distribution public without exposing private source code

## Update Contract

- Manifest path: `latest.json`
- APK path pattern: `releases/<version>/smartboard-sklink-debug.apk`
- Download model: installed apps fetch `latest.json`, compare version, download APK, verify SHA-256, then open Android install flow

## Repositories

- Private source code: local/private source repo
- Public update feed: https://github.com/Capular/smartboard-sklink-android

## Publishing

Use the helper script from the Android project:

```powershell
F:\Sklink\smartboard-sklink-android\scripts\publish-public-release.ps1 -Version 1.0.0 -Changelog "Initial Android smartboard release"
```

Then commit and push this repository.


<div align="center">

# SmartHouse

### A fast, friendly Home Assistant client — that can also **run Home Assistant on your phone**

[![Platform](https://img.shields.io/badge/platform-Android%20%7C%20iOS-lightgrey)](#-download)
[![Flutter](https://img.shields.io/badge/built%20with-Flutter-02569B?logo=flutter&logoColor=white)](https://flutter.dev)
[![Downloads](https://img.shields.io/github/downloads/nesror/SmartHouse/total?label=downloads&color=success)](https://github.com/nesror/SmartHouse/releases)
[![Stars](https://img.shields.io/github/stars/nesror/SmartHouse?label=stars&color=yellow)](https://github.com/nesror/SmartHouse/stargazers)
[![Issues](https://img.shields.io/github/issues/nesror/SmartHouse?label=issues)](https://github.com/nesror/SmartHouse/issues)

**English** · [简体中文](README-CN.md)

[Website](https://191005.xyz/smarthouse/) · [App Store](https://apps.apple.com/app/id6753762531) · [Google Play](https://play.google.com/store/apps/details?id=cn.yzapp.flutter.ha) · [Download APK](https://github.com/nesror/SmartHouse/releases/latest) · [Video tutorial](https://www.bilibili.com/video/BV16WCbYwEaH/)

</div>

---

| Home | Sensors | Settings |
| :---: | :---: | :---: |
| <img src="doc/Screenshot_20240930_152432.webp" width="260"> | <img src="doc/Screenshot_20240930_152523.webp" width="260"> | <img src="doc/Screenshot_20240930_152537.webp" width="260"> |

---

## 💡 Why SmartHouse

Most Home Assistant apps just show you a dashboard. **SmartHouse can also *be* the server.**

Grab a spare 64-bit Android phone, tap once, and you get a 24/7 Home Assistant hub — no PC, no NAS, no cloud server, no root. Your old phone stops collecting dust and starts running your home.

- ⚡ **Faster startup, friendlier UI** — a purpose-built Flutter client, not a WebView wrapper
- 📦 **Skip the hardware** — run Home Assistant locally on the phone in your pocket
- 🎙️ **Real voice control** — Assist pipelines with system STT/TTS or offline Sherpa ONNX
- 🔋 **Deep Android integration** — sensors, notifications and push actions wired into HA
- 🌍 **6 languages** — 简体中文 / English / Français / 日本語 / Русский / العربية
- 🔒 **Private by design** — everything talks to *your* Home Assistant, nothing to a third party

## 📥 Download

| Platform | Channel | Notes |
| --- | --- | --- |
| Android | [Google Play](https://play.google.com/store/apps/details?id=cn.yzapp.flutter.ha) | Recommended for most users, keeps itself updated |
| Android | [GitHub Releases](https://github.com/nesror/SmartHouse/releases/latest) | Direct APK (arm64-v8a / armeabi-v7a / x86_64). Supports in-app self-update. Uses its own app ID, so it can be installed alongside the store build |
| iOS | [App Store](https://apps.apple.com/app/id6753762531) | Requires iOS 15.6 or later |
| iOS | [GitHub Releases](https://github.com/nesror/SmartHouse/releases/latest) | Unsigned IPA for self-signing / sideloading |

## ⚡ Run Home Assistant on your phone (Android)

The feature that makes SmartHouse different: Home Assistant runs **locally on your device**, no external server required.

- **One-tap install** — downloads the official container image, extracts it and starts it, entirely through the UI. No command line, no Terminal, no Docker knowledge
- **No root** — built on `proot` containers, so your system partition is never touched
- **China-network friendly** — ships with multiple mirror sources, automatic fallback and custom mirror support; interrupted downloads resume instead of restarting
- **Transparent progress** — download / extract / start stages are shown live in the notification shade, cancellable at any time
- **One-tap takeover** — after install, set the local instance as your app server address and start configuring your home
- **LAN access** — any other device on the same network can open `http://<phone-ip>:8123`
- **Always there** — boot auto-start and app-launch auto-start, plus per-brand battery-optimization guides to keep the service alive
- **Image updates** — check for a new version in seconds and upgrade in place, keeping your configuration intact

> Headless 24/7 operation? Plug in the phone, disable battery optimization, and it becomes a silent home server.

## 🏠 Features

**Every device at your fingertips**

- Entities sync from Home Assistant and are organized into rooms (tabs); newly added entities are detected and can be added in one tap
- Rich support for lights, fans, climate, covers, media players, cameras, vacuums, weather, sensors and more
- Card editing and reordering, pinned message entities, quick swipe-to-control cards
- Whole-house overview mode with per-room summaries
- Multiple server addresses with automatic LAN/WAN switching — log in via WebView password login or a long-lived access token

**Assist voice assistant**

- Text and voice conversations through Home Assistant Assist pipelines
- System STT/TTS, plus offline recognition via Sherpa ONNX
- Switch pipelines and voice engines freely

**Sensors & notifications (Android)**

- Foreground service periodically reports battery, Wi-Fi, steps, Bluetooth and location to HA — perfect for home/away automations
- Notification listener forwards your phone's notifications into HA
- Push actions can open entities, play media or call services

**Media & history**

- Browse Home Assistant media sources and play in-app or externally
- Entity history charts

**Personalization**

- Dark mode and switchable theme colors
- Dashboard configuration sync and local backup, restorable when you reinstall
- Immersive mode, and optional use of Home Assistant's built-in Lovelace page as the home screen
- Six UI languages: 简体中文, English, Français, 日本語, Русский, العربية

**VIP**

- An optional in-app purchase that supports continued development and unlocks advanced features such as voice conversation

## 🎬 Learn & watch

| | |
| --- | --- |
| Website & introduction | <https://191005.xyz/smarthouse/> |
| Video tutorial | <https://www.bilibili.com/video/BV16WCbYwEaH/> |
| Changelog video | <https://www.bilibili.com/video/BV1Y8411179b/> |
| Release notes (WeChat article) | <https://mp.weixin.qq.com/s/Fce0EhnMYU-uy96yIH9_0A> |

## 📌 Requirements & notes

- **Android**: Android 7.0+ · **iOS**: 15.6+
- **Local HA install**: 64-bit Android device with at least **6 GB free storage**. The first Home Assistant start initializes its database and takes roughly **1–3 minutes**
- Running HA on a phone long-term? Keep it plugged in and turn off battery optimization for the app
- To connect to a remote Home Assistant you need a reachable server address; SmartHouse does not provide one
- Unlike the Android build, the iOS build does not include the local HA runtime or the Android sensor/notification bridge

## ❓ Help, feedback & feature requests

Found a bug or missing a feature? This repository is the place for **usage help and issue tracking**.

- 🐞 [Report a bug or request a feature](https://github.com/nesror/SmartHouse/issues/new/choose)
- 💬 [Browse existing issues](https://github.com/nesror/SmartHouse/issues)

When filing a report, please include:

1. SmartHouse version
2. Device type and OS version (Android / iOS)
3. Home Assistant version
4. Screenshots if possible, and for entity-control problems the full state attributes of the device

That information usually turns a "doesn't work" into a fix within one round trip.

## ⭐ Support the project

If SmartHouse is useful to you, a ⭐ star on this repo genuinely helps — it makes the project easier for other Home Assistant users to find.

- ⭐ [Star this repository](https://github.com/nesror/SmartHouse/stargazers)
- 📝 [Tell us what's missing](https://github.com/nesror/SmartHouse/issues/new/choose)
- ☕ In-app VIP purchase also directly funds continued development

## 📄 Disclaimer

SmartHouse is an independent third-party client and is **not affiliated with, endorsed by, or sponsored by** Home Assistant or the Open Home Foundation. "Home Assistant" is a trademark of its respective owner. A Home Assistant server and its configuration remain the user's own responsibility.

---

<div align="center">

**SmartHouse** · Let every phone become the brain of your smart home

</div>

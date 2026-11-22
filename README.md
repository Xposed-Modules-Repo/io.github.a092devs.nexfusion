# NexFusion

**NexFusion** is an open-source runtime patch manager and LSPosed framework featuring a clean Material You interface. It applies in-memory bytecode hooks dynamically using **libxposed** and **DexKit** to popular Android applications without modifying the original APKs, breaking Play Store signatures, or losing official update paths.

---

## What Makes NexFusion Different?

Unlike traditional patching tools that require compiling and repacking modified APKs:
- **Zero APK Repacking**: Modifies bytecode purely in RAM at app startup via LSPosed. Original apps stay untouched and can be updated normally through Google Play.
- **Modular Patch Bundles (`.nxb`)**: Patches and hooks are distributed as lightweight, independently updatable bundles. Update patch features without reinstalling the manager app.
- **Dynamic Target Discovery**: Only targets applications supported by your installed patch bundles—no hardcoded app clutter.
- **Automatic Background Updates**: Optionally checks for and installs patch bundle updates in the background for a seamless set-it-and-forget-it experience.
- **Built-in Stealth Cloak**: Shields target apps from detecting root or Xposed module presence.

---

## Supported Apps & Capabilities

NexFusion pairs with the official **NexFusion Unified Patches** bundle to enhance:

| App | Key Features |
|---|---|
| **YouTube** | Ad-blocking, background playback, SponsorBlock, Return YouTube Dislike, custom playback speeds |
| **YouTube Music** | Background playback, audio-only mode, premium bar removal, ad-free listening |
| **Telegram** | Anti-deleted messages (subtly marked with trash indicators), anti-expiring media saving, restriction bypass |
| **Reddit** | Ad-free browsing, promoted content removal, clean feed |
| **Instagram** | Sponsored post & ad filtering, media download capabilities |
| **Gboard & System** | Customization options and dynamic theming enhancements |

---

## Quick Setup Guide

1. **Install Module:** Download and install `NexFusion.apk` from the [Releases](https://github.com/Xposed-Modules-Repo/io.github.a092devs.nexfusion/releases) tab or LSPosed Manager.
2. **Enable in LSPosed:** Enable the NexFusion module in your LSPosed framework.
3. **Open NexFusion:** Launch the app. Go to the **Patches** tab and tap **Install** on the *NexFusion Unified Patches* source.
4. **Configure Scope & Hooks:** Return to the **Home** tab to configure options for your installed apps. Grant LSPosed scope when prompted.
5. **Restart Target Apps:** Force-close and reopen target apps for the in-memory hooks to take effect.

---

## Links & Community

- **Source Code**: [github.com/a092devs/NexFusion](https://github.com/a092devs/NexFusion)
- **Patch Bundles**: [github.com/a092devs/Nexfusion-Patches](https://github.com/a092devs/Nexfusion-Patches)
- **Bug Reports & Feature Requests**: [GitHub Issues](https://github.com/a092devs/NexFusion/issues)

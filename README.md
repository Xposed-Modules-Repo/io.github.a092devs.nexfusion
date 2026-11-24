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

## Supported Applications Matrix

NexFusion pairs with the official **NexFusion Unified Patches** bundle (`a092devs/Nexfusion-Patches`) to enhance **17+ supported application targets**:

<details>
<summary><b>🎥 Video, Audio & Streaming (4 Targets)</b> — <i>YouTube, YouTube Music, Crunchyroll, Stremio</i></summary>
<br>

| Application | Package Identifier | Key Patch Capabilities |
|---|---|---|
| **YouTube** | `com.google.android.youtube` | Ad-free playback, SponsorBlock, background audio, DeArrow replacement, custom speed/quality dialogs, swipe volume/brightness, miniplayer, ambient mode, Litho node bypass, channel search fix. |
| **YouTube Music** | `com.google.android.apps.youtube.music` | Background playback, audio ad removal, exclusive audio stream playback, hide upgrade buttons, suppress promotional banners, SoundProof AI blocker, Playlist tags, offline fullscreen player, mark downloaded songs, third-party lyrics enhancement. |
| **Crunchyroll** | `com.crunchyroll.crunchyroid` | Native Picture-in-Picture mode with contextual Skip Intro and Skip Credits controls; remove titles from Continue Watching feed. |
| **Stremio** | `com.stremio.one` | Auto & manual intro/credits skipping using embedded chapters and stream metadata; auto-pick best stream; hide episode spoilers (synopses & thumbnails); avoid SDH subtitles; audio & subtitle track language memory; smoother playback buffer expansion; seamless binge watching; external player progress & subtitle hand-off. |

</details>

<details>
<summary><b>💬 Social Networks & Messaging (5 Targets)</b> — <i>Instagram, X (Twitter), Reddit, Discord, LinkedIn</i></summary>
<br>

| Application | Package Identifier | Key Patch Capabilities |
|---|---|---|
| **Instagram** | `com.instagram.android` | Media downloader for feed posts, Reels, Stories, Highlights, and profile pictures; remove sponsored feed posts, Reels, and Story ads; anonymous Story and Live viewing; anonymous DM viewing & disappearing media viewing; strip tracking parameters; remove build expired lockout; hide Meta AI. |
| **X (Twitter)** | `com.twitter.android` | Promoted post and ad removal; video and GIF media downloader; bypass Compose sensitive media blur interstitials without tap-to-reveal; block forced updates; telemetry blackholing. |
| **Reddit** | `com.reddit.frontpage` | Feed and comment ad removal; guest browsing mode; sanitize shared URLs; suppress screenshot sharing bottom sheet; unmute Redgifs streams; custom feed sorting. |
| **Discord** | `com.discord` | Suppress crash telemetry, analytics, touch logging, and advertising identifiers; native system font typography support across chat and UI surfaces. |
| **LinkedIn** | `com.linkedin.android` | 1-tap media downloader for photos, carousel images, and progressive MP4 videos; sanitize share links; direct URL navigation bypassing redirects; hide suggested posts, promoted jobs, and premium upsells; feed filters; Material You dynamic theme. |

</details>

<details>
<summary><b>🛠️ System, Productivity & Utilities (7 Targets)</b> — <i>Google Photos, Google Maps, Gboard, Gmail, Google App (Discover), Proton VPN, 1.1.1.1</i></summary>
<br>

| Application | Package Identifier | Key Patch Capabilities |
|---|---|---|
| **Google Photos** | `com.google.android.apps.photos` | Device spoofing for unlimited original-quality Google Photos cloud storage backups; DCIM folder backup control. |
| **Google Maps** | `com.google.android.apps.maps` | Sponsored pin and search ad suppression, high refresh rate unlock (90/120 Hz), telemetry blocking, hide AI clutter, AMOLED black theme. |
| **Gboard** | `com.google.android.inputmethod.latin` | Rounded keycaps; Google Sans Flex typography & GM3 Expressive styling; proactive post-correction undo controls; Quick & Magic Emoji (Emojify); expanded AI writing tools; spellchecker chips UI; scan text OCR; spacebar cursor trackpad. |
| **Gmail** | `com.google.android.gm` | Suppress sponsored promotional and advertising cards in personal inboxes. |
| **Google App (Discover)** | `com.google.android.googlequicksearchbox` | Filter sponsored cards, shopping ads, and promotional recommendations in the Discover feed. |
| **Proton VPN** | `ch.protonvpn.android` | Suppress upgrade banners and nag dialogs; unlock NetShield UI toggles; disable telemetry and background observability workers. |
| **1.1.1.1** | `com.cloudflare.onedotonedotonedotone` | Spoof WARP+ Unlimited account tier in UI, disable telemetry, and optionally bypass SSL certificate pinning. |

</details>

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

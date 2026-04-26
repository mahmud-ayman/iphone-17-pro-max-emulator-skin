# iPhone 17 Pro Max — Android Emulator Skin

Preview iOS UI directly in Android Studio. A pixel-perfect iPhone 17 Pro Max device skin for the Android Emulator, built for Flutter and React Native developers who need realistic iOS frames without a Mac.

![Platform](https://img.shields.io/badge/Platform-Android%20Studio-blue)
![Flutter](https://img.shields.io/badge/Flutter-Ready-02569B)
![React Native](https://img.shields.io/badge/React%20Native-Ready-61DAFB)
![License](https://img.shields.io/badge/License-MIT-green)

---

## ✨ Features

- **True-to-size iPhone 17 Pro Max frame** — 1410×2962 skin, 1320×2868 display area
- **Dynamic Island support** — accurate cutout via mask
- **Transparent PNGs** — clean edges, no white background
- **Works on Windows, macOS, Linux** — no Xcode required
- **Perfect for**: Flutter, React Native, screenshots, demos, client presentations

## 📸 Preview

> Add your screenshot here after installation

```
your_app_running_in_iphone_frame.png
```

## 📦 What's Included

```
iphone17promax/
├── iphone bg.png    # Device frame (transparent)
├── Notch.png        # Dynamic Island mask
└── layout           # Skin layout file
```

## 🚀 Installation

### Install directly from Android Studio (no manual folder copy)

1. **Download** this repo as ZIP and extract it anywhere (e.g., Desktop)
   - You should have a folder containing: `iphone bg.png`, `Notch.png`, `layout`

2. **Open Android Studio** → **Tools > Device Manager**

3. Click **Create Device** → **New Hardware Profile**

4. Fill in the specs:
   - **Device Name:** iPhone 17 Pro Max
   - **Screen Size:** 6.9"
   - **Resolution:** 1320 × 2868
   - **RAM:** 2048 MB (or more)
   - **Has Play Store:** No

5. Scroll down to **Custom Skin Definition** → click the folder icon → **select the extracted folder**

6. Click **Finish**, then select your new AVD and hit **Cold Boot Now**

That's it — the skin loads directly from the folder, no need to copy files into `.android`.

## ⚙️ Technical Specs

| Property | Value |
|----------|-------|
| Skin Size | 1410 × 2962 px |
| Display Area | 1320 × 2868 px |
| Offset X/Y | 45 / 47 px |
| Format | PNG-32 with alpha |
| Dynamic Island | Included in mask |

## 💡 Usage Tips

- **Flutter**: Use `flutter run` and select the AVD — your app renders inside the iPhone frame
- **React Native**: `npx react-native run-android` works the same
- For perfect screenshots: Device Manager → Camera icon → Save
- Cold Boot after first install to apply skin changes

## 🛠️ Troubleshooting

**White background around frame?**
→ Ensure you're using the transparent PNGs from this repo, not the white versions.

**Screen misaligned?**
→ Check `layout` has `x 45 y 47`. If still off, adjust by ±1px for your display scaling.

**Emulator crashes?**
→ Verify resolution matches exactly 1320×2868 in hardware profile.

## 🤝 Contributing

PRs welcome! If you make skins for other iPhone models, open an issue or submit a pull request.

## 📄 License

MIT License — free for personal and commercial use.

---

**Made for developers who build iOS experiences on non-Apple hardware.**

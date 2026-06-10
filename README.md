# Depth Locator

A Blender addon for creating depth-controlled empties on camera rays.

**Youtube Addon Demo:** [Youtube](https://youtu.be/SEUtsn3_g6g)
**Latest Version:** 1.0.0  
**Download:** [Gumroad](https://gumroad.com)  
**Support:** [Report Issues](https://github.com/vinodh-vfxartist/depth_locator/issues)  
**Author:** [The Vin Lab](https://www.thevinlab.in)

---

## Features

✨ **Create empties on camera→object rays** — Position objects along the camera-to-target direction  
📏 **Real-time depth adjustment** — Slide the empty along the ray with a simple slider  
⚡ **Pure-driver approach** — No constraints, clean rotation (0,0,0 in all spaces)  
🔧 **Simple & lightweight** — Fast, efficient, zero overhead  

---

## Installation

### Quick Start (Blender 4.1+)
1. Download `depth_locator.zip`
2. Drag the ZIP into your Blender window
3. Click **"Install"**
4. Restart Blender
5. ✅ Done!

### Manual Install (All Blender Versions)
1. Download `depth_locator.zip`
2. Go to **Edit > Preferences > Add-ons**
3. Click **"Install from File"**
4. Select `depth_locator.zip`
5. Enable the addon
6. Restart Blender

---

## Quick Start

1. **Press `N`** in the 3D Viewport to open the sidebar
2. **Find "Depth Locator"** tab on the right panel
3. **Select your camera** + a target object
4. **Click "Create Depth Locator"**
5. **Adjust the "Depth" slider** to move the empty along the ray


---

## What It Does

Creates a **depth-controlled empty** on the ray from your camera to any object.

**Formula:**
```
world_position = camera_position + normalize(target_position - camera_position) * depth
```

**Perfect for:**
- Quick VFX reference positioning
- Depth validation
- Camera/object relationship testing
- Animation reference

---

## Requirements

- **Blender:** 3.6.0 or higher
- **Python:** 3.10+ (built-in with Blender)
- **OS:** Windows, macOS, Linux

---

## Support & Issues

### Found a bug?
→ [Report it on GitHub](https://github.com/vinodh-vfxartist/depth_locator/issues)

### Contact
- 📧 Email: vinodh.vfxartist@gmail.com
- 🌐 Website: https://www.thevinlab.in
- 💬 GitHub Issues: [Open issue](https://github.com/vinodh-vfxartist/depth_locator/issues)

---

## Changelog

### Version 1.0.0 (June 2026)
- Initial release
- Depth-controlled empty creation
- Real-time depth adjustment
- Support for Blender 3.6+

[Full changelog →](CHANGELOG.md)

---

## Technical Details

**Addon ID:** `depth_locator`  
**Operator:** `bpy.ops.dl.create_depth_locator()`  
**Panel Category:** Depth Locator (Sidebar)  
**License:** GPL-3.0

---

## License

This project is licensed under the **GNU General Public License v3.0** — see the [LICENSE](LICENSE) file for details.

**Summary:** You can use, modify, and distribute this addon freely, as long as you include the license and share modifications under the same license.

---

## Author

**Vinod Kumar Padakantoju** — [The Vin Lab](https://www.thevinlab.in)

Created for the VFX & motion graphics community.

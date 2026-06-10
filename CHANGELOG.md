# Changelog

All notable changes to Depth Locator will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [1.0.0] - 2026-06-10

### Added
- ✨ Initial release of Depth Locator
- Create depth-controlled empties on camera rays
- Real-time depth adjustment with slider (0-500 scene units)
- Scripted drivers for smooth position calculation
- Automatic "Depth_Locators" collection for organization
- Support for Blender 3.6.0 and higher
- Pure-driver approach (no constraints, clean rotation)
- Full documentation and troubleshooting guides
- GitHub issue tracking for bug reports

### Features
- **Create Locator Operator** (`bpy.ops.dl.create_depth_locator()`)
  - Creates empties on camera→object rays
  - Automatic unique naming (Depth_Locator, Depth_Locator.001, etc.)
  - Organized in "Depth_Locators" collection

- **Depth Property**
  - Adjustable from 0 to 500 scene units
  - Soft max at 500 (can exceed)
  - Real-time updates
  - Keyframeable for animation

- **UI Panel**
  - Located in sidebar (press N in 3D Viewport)
  - Shows active camera status
  - Shows track object status
  - "Create Depth Locator" button

### Technical Details
- **Addon ID:** depth_locator
- **Category:** Camera
- **Author:** Vinod Kumar Padakantoju
- **License:** GPL-3.0
- **Python:** 3.10+
- **Blender:** 3.6.0+

### Known Limitations
- Currently works with single camera per scene
- Depth values are linear (no curved paths)
- Requires camera to be set as active scene camera

---

## Planned Features (Future Releases)

- [ ] Multiple camera support
- [ ] Curved path support
- [ ] Advanced driver options
- [ ] Batch locator creation
- [ ] Export depth values
- [ ] 3D cursor snap options
- [ ] Animation tools

---

## How to Report Bugs

Found an issue? Help us improve!

1. Check [TROUBLESHOOTING.md](docs/TROUBLESHOOTING.md) first
2. [Open an issue on GitHub](https://github.com/vinodh-vfxartist/depth_locator/issues)
3. Include:
   - Blender version
   - Operating system
   - Steps to reproduce
   - Expected vs actual behavior
   - Error messages (if any)

---

## How to Request Features

Want something new? Tell us!

[Open a feature request](https://github.com/vinodh-vfxartist/depth_locator/issues)

---

## Version History

| Version | Date | Status |
|---------|------|--------|
| 1.0.0 | 2026-06-10 | ✅ Released |

---

**Made with ❤️ by [The Vin Lab](https://www.thevinlab.in)**

[← Back to README](README.md)

# Changelog

All notable changes to Brushtily will be documented in this file.

## [1.2.0] - 2025-01-20

### Added
- **Descriptive object naming**: Objects are now named based on the selected file (e.g., `Japanese_Maple_Tree_G02` instead of `stamped_object_0`)
  - Makes objects easier to identify in Tiled's object list
  - Uses same-name strategy for simpler grouping during TMX-to-text conversion

- **Quick reselect last object**: Added "Reselect Last" button in Select Object dialog
  - Remembers the last selected object (image or tile)
  - Shows current selection at the top of the dialog
  - Faster workflow when reusing the same object

### Changed
- **Auto-enable stamping on object selection**: Object Stamping Mode now enables automatically when selecting an object on an object layer
- **Auto-disable stamping on brush selection**: Object Stamping Mode disables automatically when selecting a brush texture on an image layer
- **Auto-toggle on layer switch**: Automatically toggles stamping mode when switching between layer types
  - Object layer → auto-enables (if object is selected)
  - Image layer → auto-disables
  - Mode stays aligned with the current layer type

### Improved
- Streamlined workflow with automatic mode switching based on context
- Better object identification and naming for easier management
- Seamless transitions between object stamping and texture brushing

---

## [1.1.0] - 2025-01-19

### Fixed
- **Fixed artifacting issues causing discoloration** when erasing or adding image layers
  - Resolved color shift problems related to premultiplied alpha handling
  - Improved color accuracy during brush operations and erase functions

### Changed
- Removed redundant button from toolbar to streamline interface
- Improved overall stability and performance

### Technical Improvements
- Enhanced image layer compositing to prevent color artifacts
- Better handling of premultiplied alpha channels during brush operations

---

## [1.0.0] - 2025-01-19

### Added
- Initial public release
- Freeform, non-grid-aligned brush strokes
- Custom brush textures (PNG/JPG) and tileset tile brushes
- Adjustable brush properties (size, opacity, softness, texture scale, rotation)
- Advanced features: blend modes, mask modes, pressure sensitivity, fill mode
- Object stamping system with library browser
- Right-click erase functionality
- Auto-smoothing brush layers
- Native layer blending
- Brush presets and layer brush memory

# Brushtily v1.2.0 - Workflow Improvements & Smart Mode Switching

## ✨ New Features

### Descriptive Object Naming
- **Objects are now named based on the selected file**
  - Example: `Japanese_Maple_Tree.G02.png` → objects named `Japanese_Maple_Tree_G02`
  - Example: `Maple_red_yellow_v2.G15.png` → objects named `Maple_red_yellow_v2_G15`
  - **Benefit**: Much easier to identify objects in Tiled's object list
  - Uses same-name strategy (no counters) for simpler grouping during TMX-to-text conversion

### Quick Reselect Last Object
- **"Reselect Last" button** in the Select Object dialog
  - Remembers the last selected object (image or tile)
  - Shows current selection at the top of the dialog
  - **Benefit**: Faster workflow when reusing the same object

## 🔄 Smart Mode Switching

### Auto-Enable Stamping on Object Selection
- When selecting an object (image file or tile) on an object layer, **Object Stamping Mode enables automatically**
- **Benefit**: One less step - start stamping immediately after selection

### Auto-Disable Stamping on Brush Selection
- When selecting a brush texture (file or tile) on an image layer, **Object Stamping Mode disables automatically**
- **Benefit**: Prevents accidental object stamping while brushing textures

### Auto-Toggle on Layer Switch
- **Automatically toggles stamping mode** when switching layer types:
  - **Object layer** → auto-enables (if object is selected)
  - **Image layer** → auto-disables
- **Benefit**: Mode stays aligned with the current layer type - no manual toggling needed

## 📊 Summary

These changes reduce manual steps and make the workflow smoother:
- ✅ Automatic mode switching based on context
- ✅ Better object identification and naming
- ✅ Quick reselection of frequently used objects
- ✅ Seamless transitions between object stamping and texture brushing

## 📦 Installation

1. **Download** `brushtily.mjs` from this release
2. **Copy to Tiled extensions folder**:
   - **Windows**: `%LOCALAPPDATA%\Tiled\extensions\`
   - **macOS**: `~/Library/Preferences/Tiled/extensions/`
   - **Linux**: `~/.config/tiled/extensions/`
3. **Restart Tiled**
4. Find "Brushtily" in the Tools toolbar

## 📋 Requirements

- Tiled 1.8 or later
- JavaScript extensions enabled (default)

## 🐛 Known Issues

- Freeform brush strokes may show visual rendering appearances during painting (does not affect final result)
- Object stamping precision may vary slightly in isometric maps due to design considerations

## 🙏 Credits

**Created by:** Leo Louvar  
**Developed with:** [PersistenceAI](https://persistence-ai.github.io/Landing/) using model GLM 4.7 and human review and refinement.

---

Enjoy creating beautiful maps with Brushtily! 🎨

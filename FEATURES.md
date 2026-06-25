# Features Guide

## Core Features

### 📤 Upload & Management
- Drag-and-drop SVG upload
- Multi-file support (up to 10 figures recommended)
- Auto-detection of SVG dimensions
- Real-time thumbnail preview

### 🎯 Smart Alignment
- **Magnetic Snapping**: Figures automatically snap to alignment when dragged close
- **Three Alignment Modes**:
  - Top Aligned: All figures in a row align to top
  - Center Aligned: Vertically centered
  - Bottom Aligned: All figures align to bottom
- **Dead Zone**: 25px tolerance prevents flickering

### 🎨 Flexible Labeling
- **Three Label Formats**:
  - `A. B. C.` (Letter with period)
  - `A B C` (Letter only)
  - `1 2 3` (Numbers)

- **Customizable Position**:
  - Left of figure (default)
  - Right of figure
  - Above figure
  - Below figure

- **Size & Distance**:
  - Label size: 8-32 pixels
  - Distance from figure: 0-80 pixels

### 🧲 Smart Layout Modes

#### Auto Wrap (Recommended)
- Automatically detects aspect ratio
- Very wide (>2:1) → 1 per row
- Wide (>1.1:1) → 2 per row
- Square (0.7-1.1) → 2 per row
- Tall (<0.7) → 1 per row

#### Force Row
- All figures in a single row
- Automatically sized to fit

#### Force Column
- All figures in a single column
- Each figure at full width

### 📐 Advanced Grid
- **Grid Display**: Toggle grid reference lines
- **Grid Snapping**: Optional snap-to-grid for precise alignment
- **Customizable Spacing**: 0-50px between figures

### 💾 Auto-Save & History

#### Automatic Saving
- Every change is automatically saved to browser localStorage
- No manual save needed
- Persists across browser sessions

#### Undo/Redo
- Ctrl+Z / Cmd+Z: Undo last action
- Ctrl+Y / Cmd+Y: Redo
- Up to 50 actions in history
- Visual history panel shows all steps

#### Layout Export/Import
- Download layout as JSON file
- Share layout with colleagues
- Import saved layout to restore configuration
- Perfect for creating templates

### 📥 Export Formats

#### PDF Export
- **Resolution**: 300 DPI (publication quality)
- **File Format**: Standard PDF
- **Best For**: Academic papers, publications
- **Features**: 
  - Preserves all formatting
  - Editable in most PDF tools
  - High quality printing

#### SVG Export
- **Format**: Scalable Vector Graphics
- **Quality**: Full vector, infinitely scalable
- **Best For**: Further editing in design software
- **Features**:
  - Fully editable in Illustrator, Inkscape, etc.
  - Editable text labels
  - Lossless quality
  - Small file size

#### PNG Export
- **Format**: Raster image
- **Quality**: High-quality bitmap
- **Best For**: Presentations, web use
- **Features**:
  - Universal compatibility
  - Optimized file size
  - Perfect for PowerPoint/Google Slides

### ⌨️ Keyboard Shortcuts

| Shortcut | Action | Note |
|----------|--------|------|
| `Ctrl+Z` / `Cmd+Z` | Undo | Works on drag/resize |
| `Ctrl+Y` / `Cmd+Y` | Redo | Redo undone actions |
| `Ctrl+S` / `Cmd+S` | Export SVG | Triggers download |
| `Ctrl+P` / `Cmd+P` | Export PDF | Triggers download |
| `Delete` | Remove figure | Reserved for future |

### 🖱️ Mouse Gestures

| Action | Result |
|--------|--------|
| Click & drag figure | Move figure (with auto-snap) |
| Drag bottom-right corner | Resize (preserves aspect ratio) |
| Scroll in preview | Navigate large layouts |

## Advanced Features

### Magnetic Snapping
- Activates automatically when dragging
- 50px activation radius
- 25px dead zone to prevent flickering
- Stays "stuck" until you pull 25px away
- Works with all figures in the layout

### Grid Display
- Faint gray grid overlay
- 20px grid spacing (hardcoded)
- Helps with visual alignment
- Toggle on/off for clarity

### History Management
- Shows up to 50 recent steps
- Click any step to jump to that state
- Current step highlighted
- Useful for exploring different layouts

### Data Persistence
All data stored in **browser localStorage**:
- Figure positions and sizes
- User settings (alignment, labels, spacing)
- Complete undo/redo history
- Survives browser restart
- Survives accidental page reload

⚠️ **Important**: Clearing browser cache will erase all saved data. Export layouts regularly!

## Tips & Tricks

### Pro Tips
1. **Pre-size your SVGs**: Resize source SVGs to similar scales before upload for better results
2. **Use Grid Mode**: Enable grid when you need precise alignment
3. **Regular Backups**: Export your layout as JSON frequently
4. **Test Before Export**: Always verify preview before exporting
5. **Adjust One Parameter**: Change one setting at a time to see effects

### Common Workflows

#### Quick Panel Creation
1. Upload 4 SVGs → Auto-arranged
2. Drag any misaligned → Auto-snaps
3. Export → Done in 2 minutes

#### Detailed Layout
1. Upload figures
2. Enable grid display
3. Fine-tune each position
4. Adjust label positions
5. Export multiple formats

#### Template Creation
1. Arrange a layout you like
2. Export layout as JSON
3. Share with team → Everyone can import
4. Apply to new figures quickly

### Troubleshooting Tips

**Figures not snapping?**
- Make sure alignment mode is set (not just auto)
- Try dragging closer to target figure
- Check if figures are actually in same row

**Export quality poor?**
- Use PDF for publications (300 DPI)
- Use SVG for editing (vector format)
- Use PNG for presentations

**Layout keeps changing?**
- Undo (Ctrl+Z) to revert
- Check which alignment mode is active
- Disable auto-alignment if needed

**Missing labels?**
- Ensure label size > 8px
- Check label position doesn't go off-canvas
- Verify label distance is appropriate

## Browser Support

| Browser | Support | Notes |
|---------|---------|-------|
| Chrome | ✅ Full | Best performance |
| Firefox | ✅ Full | Excellent |
| Safari | ✅ Full | Works on iPad |
| Edge | ✅ Full | Chromium-based |
| IE | ❌ No | Use modern browser |

## Storage Limits

- **Per Figures**: 5MB per SVG file
- **Total Storage**: 5-10MB browser limit
- **History Depth**: Last 50 actions
- **Recommended**: Max 10 figures per session

## Future Features (Roadmap)

- [ ] Drag-to-reorder in thumbnail list
- [ ] Custom colors for labels
- [ ] Rotate figures
- [ ] Mirror/flip figures
- [ ] Add text annotations
- [ ] Batch operations
- [ ] Cloud sync (optional)

---

**Questions?** Open an issue on GitHub!

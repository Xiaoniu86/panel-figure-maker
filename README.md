# Panel Figure Maker

A web-based tool for creating and organizing scientific panel figures with automatic alignment, drag-and-drop support, and high-quality exports.

## Features

- 📤 **Upload Multiple SVGs** - Import multiple SVG files at once
- 🎯 **Smart Auto-Alignment** - Magnetic snapping keeps figures perfectly aligned
- 🎨 **Flexible Labeling** - A. B. C. / A B C / 1 2 3 label formats with customizable size and position
- 🧲 **Drag & Resize** - Intuitive drag-and-drop editing with preserving aspect ratios
- 💾 **Auto-Save** - Automatically saves layout to browser localStorage
- ↩️ **Undo/Redo** - Ctrl+Z / Ctrl+Y to revert changes
- 📐 **Grid Snapping** - Optional grid reference for alignment (toggle in settings)
- 📥 **Export Formats** - High-quality PDF, SVG, and PNG exports
- ⚙️ **Customization** - Adjust alignment, spacing, label style, and more
- 🌐 **No Backend** - Completely client-side, no server required

## Getting Started

### Direct Usage

1. Download `index.html` and open it in any modern browser (Chrome, Firefox, Safari, Edge)
2. Start uploading SVG files
3. Drag to arrange, resize to fit, and export when ready

### Deploy to Vercel

#### Option 1: Automatic (Recommended)

1. Fork this repository on GitHub
2. Go to [Vercel](https://vercel.com)
3. Click "Add New..." → "Project"
4. Select your forked repository
5. Click "Deploy"
6. Done! Your app is live

#### Option 2: Manual

```bash
# Clone the repository
git clone https://github.com/yourusername/panel-figure-maker.git
cd panel-figure-maker

# Install Vercel CLI
npm install -g vercel

# Deploy
vercel
```

## How to Use

### Basic Workflow

1. **Upload SVGs**
   - Click the upload area or drag-and-drop SVG files
   - Figures are automatically arranged with smart layout

2. **Edit Layout**
   - **Drag** figures to reposition (auto-snaps to alignment)
   - **Right-click corner** or drag from bottom-right to resize
   - Settings update in real-time

3. **Configure**
   - **Alignment Mode**: Top / Bottom / Center aligned
   - **Layout Mode**: Auto wrap / Force row / Force column
   - **Label Style**: Choose format, size, and distance from figures
   - **Spacing**: Adjust gaps between figures

4. **Export**
   - **PDF**: High-resolution (300 DPI) for publications
   - **SVG**: Editable vector format with all elements preserved
   - **PNG**: Raster format for presentations
   - **Save/Import Layout**: Store configuration as JSON

### Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl+Z` / `Cmd+Z` | Undo |
| `Ctrl+Y` / `Cmd+Y` | Redo |
| `Ctrl+S` / `Cmd+S` | Export SVG |
| `Ctrl+P` / `Cmd+P` | Export PDF |
| `Delete` | Remove selected figure |

## Advanced Settings

- **Label Position**: Choose left, right, top, bottom, or corner positioning
- **Alignment Tolerance**: Adjust magnetic snapping sensitivity
- **Grid Display**: Toggle grid reference lines
- **Auto-Save**: Automatically saves every change to localStorage
- **Layout Restore**: Auto-loads previous session on browser refresh

## Data Storage

- All settings and layouts are stored in **browser localStorage**
- No data is sent to any server
- Works completely offline
- Exported layouts can be downloaded as JSON for backup

## Browser Compatibility

- Chrome/Edge: ✅ Full support
- Firefox: ✅ Full support
- Safari: ✅ Full support
- IE: ❌ Not supported

## File Size Limits

- Individual SVG: Up to 5MB
- Total figures: Up to 10 (recommended)
- localStorage: ~5-10MB per browser

## Troubleshooting

**Figures not snapping?**
- Ensure alignment mode is enabled
- Try increasing tolerance in settings

**Export quality is poor?**
- Use PDF export for publications (highest quality)
- SVG export preserves vector information for editing

**Layout not saving?**
- Check browser's localStorage is enabled
- Try exporting as JSON backup

**Memory issues with many figures?**
- Reduce SVG complexity before uploading
- Consider splitting into multiple sessions

## Tips & Tricks

1. **Pre-size SVGs**: Resize your SVG files to similar scales before uploading for better layout
2. **Use Grid**: Enable grid mode for precise alignment
3. **Backup Layouts**: Regularly export your layout as JSON
4. **Batch Operations**: Create multiple panels and export separately

## Browser Storage Info

- Auto-save writes to localStorage after each change
- Storage persists across browser sessions
- Clearing browser data will erase saved layouts (always export backup)
- Use "Import Layout" to restore from JSON

## License

MIT License - Feel free to use and modify

## Contributing

Found a bug or have a feature request? Open an issue on GitHub!

## Support

For issues or questions:
- Check the [GitHub Issues](https://github.com/yourusername/panel-figure-maker/issues)
- Open a new issue with details about your problem

---

**Made with ❤️ for researchers and scientists**

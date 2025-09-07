# PNG to JPG Converter

A client-side web application for converting PNG images to JPG format with adjustable quality settings. No server required, no data leaves your browser.

## Features

- **Batch conversion** - Process multiple PNG files simultaneously
- **Quality control** - Adjustable compression from 10% to 100%
- **Real-time preview** - See before and after comparison
- **Drag & drop interface** - Simple file upload experience
- **Compression statistics** - Track file size reduction and savings
- **Individual or bulk download** - Download files one by one or all at once
- **Responsive design** - Works on desktop and mobile devices
- **Privacy-focused** - All processing happens locally in your browser

## Demo

[Live Demo](https://ADS2001.github.io/png-to-jpg-converter)

## Usage

1. **Open the application** - Simply open `index.html` in any modern web browser
2. **Upload PNG files** - Drag and drop or click to select one or more PNG files
3. **Adjust quality** - Use the slider to set JPG compression (85% recommended for most use cases)
4. **Convert** - Click "Convert Selected" to process all files
5. **Download** - Download individual files or use "Download All" for batch download

## Quality Settings Guide

| Quality | Use Case | File Size | Image Quality |
|---------|----------|-----------|---------------|
| 90-100% | Print/archival | Largest | Excellent |
| 80-90% | High-quality web | Medium-large | Very good |
| 70-80% | Standard web | Medium | Good |
| 50-70% | Email/sharing | Small | Acceptable |
| 10-50% | Thumbnails | Smallest | Poor |

## Technical Details

### How It Works
- Uses HTML5 Canvas API for image processing
- Converts PNG transparency to white background (JPG doesn't support transparency)
- All processing happens client-side using JavaScript
- No external dependencies or build tools required

### Browser Compatibility
- Chrome 4+
- Firefox 3.6+
- Safari 4+
- Edge 12+
- Mobile browsers (iOS Safari, Chrome Mobile)

### File Size Optimization
The converter typically achieves:
- **30-70% size reduction** from PNG to JPG at 85% quality
- **50-90% size reduction** at 70% quality
- Results vary based on image content (photos compress better than graphics with text)

## Installation

### Option 1: Direct Use
1. Download or clone this repository
2. Open `index.html` in your web browser
3. Start converting files immediately

### Option 2: Local Server (Optional)
```bash
# For development or if you prefer a local server
git clone https://github.com/yourusername/png-to-jpg-converter.git
cd png-to-jpg-converter
python -m http.server 8000
# Open http://localhost:8000 in your browser
```

### Option 3: GitHub Pages
Fork this repository and enable GitHub Pages in settings for instant hosting.

## Use Cases

- **Web development** - Optimize images for faster loading
- **Email attachments** - Reduce file sizes for email limits
- **Social media** - Convert images for platforms that prefer JPG
- **Batch processing** - Convert multiple product photos or assets
- **Storage optimization** - Reduce disk space usage
- **Legacy system compatibility** - Convert for systems that don't support PNG

## Limitations

- **Transparency loss** - PNG transparency becomes white background in JPG
- **File size limits** - Very large images (>50MB) may cause browser performance issues
- **Internet Explorer** - Not supported (modern browsers only)
- **Lossless conversion** - JPG is always lossy; some quality degradation is inevitable

## Privacy & Security

- **No data transmission** - Files never leave your device
- **No server dependency** - Works completely offline after initial page load
- **No tracking** - No analytics, cookies, or data collection
- **Open source** - Full code transparency

## Contributing

Contributions welcome! Areas for improvement:

- Additional output formats (WebP, AVIF)
- Batch ZIP download functionality
- Progressive Web App (PWA) features
- Advanced compression options
- Error handling improvements

### Development Setup
1. Fork the repository
2. Make changes to `index.html`
3. Test in multiple browsers
4. Submit pull request

## License

MIT License - see [LICENSE](LICENSE) file for details.

## Changelog

### v1.0.0
- Initial release
- Basic PNG to JPG conversion
- Quality control slider
- Batch processing
- Download functionality
- Responsive design

## FAQ

**Q: Why do my transparent PNGs have white backgrounds after conversion?**
A: JPG format doesn't support transparency. The converter fills transparent areas with white, which is the standard approach.

**Q: What's the best quality setting?**
A: 85% provides excellent quality with significant file size reduction for most use cases.

**Q: Can I convert other formats?**
A: Currently only PNG input is supported. JPG output only.

**Q: Is there a file size limit?**
A: No hard limit, but very large files (>50MB) may slow down your browser.

**Q: Does this work offline?**
A: Yes, once the page loads, no internet connection is required.

---

**Made for developers, designers, and anyone who needs quick PNG to JPG conversion without the hassle of online tools or desktop software.**
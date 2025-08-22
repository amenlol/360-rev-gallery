# 360° Rotating Image Gallery

A beautiful and interactive 360-degree rotating image gallery built with HTML, CSS, and JavaScript. This project creates a 3D carousel effect where images rotate around a central axis, providing an engaging way to showcase multiple images.

## ✨ Features

- **3D Rotating Gallery**: Images rotate around a central axis in 3D space
- **Automatic Rotation**: Gallery automatically rotates every 3 seconds
- **Manual Navigation**: Previous and Next buttons for manual control
- **Smooth Animations**: CSS transitions for smooth rotation effects
- **Responsive Design**: Works on different screen sizes
- **Dark Theme**: Sleek black background with modern styling

## 🚀 Live Demo

Open `gallery.html` in your web browser to see the rotating gallery in action!

**🌐 View more of my projects:** [Portfolio](https://ameneb.netlify.app/)

## 📁 Project Structure

```
360-rev-gallery/
├── gallery.html          # Main HTML file
├── assets/
│   ├── gallery.js        # JavaScript functionality
│   └── csss/
│       └── gallery.css   # Styling and animations
├── im/                   # Image directory
│   ├── g1 (1).jpg
│   ├── g1 (2).jpg
│   ├── g1 (3).jpg
│   ├── g1 (4).jpg
│   ├── g1 (5).jpg
│   ├── g1 (6).jpg
│   ├── g1 (7).jpg
│   └── g1 (8).jpg
└── README.md
```

## 🛠️ Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/amenlol/360-rev-gallery.git
   cd 360-rev-gallery
   ```

2. **Open in browser**:
   - Simply open `gallery.html` in any modern web browser
   - No additional dependencies or setup required!

## 🎮 Usage

### Automatic Mode
- The gallery automatically rotates every 3 seconds
- Each rotation moves 45 degrees to show the next image

### Manual Control
- Click **"Prev"** button to rotate counter-clockwise
- Click **"Next"** button to rotate clockwise
- Manual interaction resets the automatic timer

## 🎨 Customization

### Adding More Images
1. Add your images to the `im/` directory
2. Update the HTML structure in `gallery.html`:
   ```html
   <span style="--i: 9">
     <img src="im/your-new-image.jpg" />
   </span>
   ```
3. Adjust the rotation angle in `gallery.js`:
   ```javascript
   // Change 45 to 360/number_of_images
   x = x + 45; // For 8 images: 360/8 = 45
   ```

### Styling Changes
- Modify `assets/csss/gallery.css` to change colors, sizes, and animations
- Adjust the `translateZ(400px)` value to change the radius of the rotation
- Modify the `perspective(1000px)` value to change the 3D depth effect

### Timing Adjustments
- Change the automatic rotation interval in `gallery.js`:
   ```javascript
   timer = setTimeout(() => {
     x = x - 45;
     updateGallery();
   }, 3000); // Change 3000ms to your preferred interval
   ```

## 🔧 Technical Details

### Technologies Used
- **HTML5**: Structure and semantic markup
- **CSS3**: Styling, animations, and 3D transforms
- **Vanilla JavaScript**: Interactive functionality

### Key CSS Properties
- `transform-style: preserve-3d`: Enables 3D transformations
- `perspective()`: Creates depth for 3D effects
- `rotateY()`: Rotates elements around the Y-axis
- `translateZ()`: Positions elements in 3D space

### JavaScript Features
- Event listeners for button interactions
- `setTimeout()` for automatic rotation
- Dynamic CSS transform updates
- Timer management for smooth transitions

## 📱 Browser Compatibility

- ✅ Chrome (recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ⚠️ Internet Explorer (limited 3D support)

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- Inspired by modern web design trends
- Built with pure web technologies for maximum compatibility
- Perfect for showcasing product images, portfolios, or photo collections

---

**Enjoy the rotating gallery! 🎉** 

# Universal Unit Converter

A modern, responsive web-based unit converter built with HTML, CSS, and JavaScript. Convert between different units across multiple categories with precision and ease.

## 🌟 Features

- **7 Conversion Categories** - Length, Weight, Temperature, Area, Volume, Speed, and Energy
- **Real-time Conversions** - Instant results as you type
- **Bidirectional Conversion** - Convert between any units within a category
- **Swap Functionality** - Quickly swap between "from" and "to" units
- **Formula Display** - Shows conversion formulas and factors for educational purposes
- **Responsive Design** - Works seamlessly on desktop, tablet, and mobile devices
- **Modern UI** - Clean, intuitive interface with smooth animations
- **High Precision** - Accurate conversions with proper decimal handling

## 🚀 Demo

Open `index.html` in any modern web browser to start using the converter.

## 📊 Supported Units

### Length
- Millimeters (mm)
- Centimeters (cm)
- Meters (m)
- Kilometers (km)
- Inches (in)
- Feet (ft)
- Yards (yd)
- Miles (mi)

### Weight
- Milligrams (mg)
- Grams (g)
- Kilograms (kg)
- Ounces (oz)
- Pounds (lb)
- Metric Tons (ton)

### Temperature
- Celsius (°C)
- Fahrenheit (°F)
- Kelvin (K)

### Area
- Square Millimeters (sq mm)
- Square Centimeters (sq cm)
- Square Meters (sq m)
- Square Kilometers (sq km)
- Square Inches (sq in)
- Square Feet (sq ft)
- Acres

### Volume
- Milliliters (ml)
- Liters (l)
- Cubic Inches (cu in)
- Cubic Feet (cu ft)
- US Gallons
- UK Gallons

### Speed
- Meters per Second (m/s)
- Kilometers per Hour (km/h)
- Miles per Hour (mph)
- Knots

### Energy
- Joules (J)
- Kilojoules (kJ)
- Calories (cal)
- Kilocalories (kcal)
- Watt Hours (Wh)
- Kilowatt Hours (kWh)

## 🛠️ Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Yash-Naikwadi/UnitConvertor_OpenSource.git
   ```

2. **Navigate to the project directory:**
   ```bash
   cd UnitConvertor_OpenSource
   ```

3. **Open in browser:**
   ```bash
   open index.html
   # or simply double-click the index.html file
   ```

No build process or dependencies required! It's a pure HTML/CSS/JavaScript application.

## 💻 Usage

1. **Select a Category**: Click on one of the category tabs (Length, Weight, Temperature, etc.)
2. **Enter a Value**: Type the number you want to convert in the "From" field
3. **Choose Units**: Select the source and target units from the dropdown menus
4. **View Results**: The conversion appears instantly in the "To" field and result display
5. **Swap Units**: Use the swap button (⇅) to quickly reverse the conversion direction
6. **View Formula**: Check the formula display to understand the conversion calculation

## 🔧 Technical Details

### Architecture
- **Pure Frontend**: No server dependencies, runs entirely in the browser
- **Responsive Design**: Built with CSS Flexbox and Grid for optimal layout
- **Modern JavaScript**: Uses ES6+ features for clean, maintainable code
- **Progressive Enhancement**: Graceful degradation for older browsers

### Browser Compatibility
- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

### Performance
- **Lightweight**: ~15KB total file size
- **Fast Loading**: Single HTML file with embedded CSS and JavaScript
- **Smooth Animations**: Hardware-accelerated CSS transitions
- **Efficient Calculations**: Optimized conversion algorithms

## 🎨 Customization

### Adding New Units

To add a new unit to an existing category, modify the `conversions` object in the JavaScript:

```javascript
conversions.length.units.newUnit = {
    name: "Display Name",
    factor: conversionFactorToMeters
};
```

### Adding New Categories

1. Add the category to the `conversions` object:
   ```javascript
   conversions.newCategory = {
       name: "Category Name",
       units: {
           unit1: { name: "Unit 1", factor: 1 },
           unit2: { name: "Unit 2", factor: conversionFactor }
       }
   };
   ```

2. Add a new tab in the HTML:
   ```html
   <div class="category-tab" data-category="newCategory">Category Name</div>
   ```

### Styling

The CSS uses CSS custom properties for easy theming. Key variables include:
- `--primary-gradient`: Main gradient colors
- `--accent-color`: Accent color for highlights
- `--text-color`: Main text color
- `--background-color`: Background color

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

### Development Setup

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Make your changes
4. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
5. Push to the branch (`git push origin feature/AmazingFeature`)
6. Open a Pull Request

### Contribution Guidelines

- Ensure cross-browser compatibility
- Follow the existing code style and structure
- Add appropriate comments for complex logic
- Test thoroughly across different devices and screen sizes
- Update documentation as needed

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Inspired by the need for a simple, accurate unit converter
- Built with modern web standards and best practices
- Icons and design elements follow Material Design principles

---

## 🚀 Future Enhancements

- [ ] Currency conversion with live exchange rates
- [ ] Scientific notation support
- [ ] Conversion history
- [ ] Offline PWA functionality
- [ ] Voice input support
- [ ] Keyboard shortcuts
- [ ] Export conversion results
- [ ] Additional unit categories (pressure, frequency, etc.)
- [ ] Dark/light theme toggle
- [ ] Localization support

---

**Made with ❤️ for developers and everyday users who need quick, accurate unit conversions.**
# Glass Price Calculator

A desktop application for glass businesses to instantly calculate pricing for custom-cut glass sheets.
I built this for a glass business in Strand, Somerset West just outside of Cape Town called Cubed Glass.

## Features

- **Custom Dimensions**: Enter any length and width for precise quotes
- **Flexible Units**: Choose between millimeters, centimeters, or meters
- **Adjustable Pricing**: Set your price per square meter for different glass types
- **Instant Calculations**: Real-time area and price calculations
- **Professional Interface**: Clean, easy-to-use design
- **Offline Ready**: Works without an internet connection

## Installation

### For Users

1. Download `Glass Price Calculator Setup 1.0.0.exe`
2. Double-click to install
3. Follow the installation prompts
4. Launch the app from your desktop or start menu

**Note**: Windows may show a security warning since the app isn't code-signed. Click "More info" → "Run anyway" to proceed with installation.

## Usage

1. **Set Your Rate**: Click the settings icon (⚙️) to set your price per square meter
2. **Choose Unit**: Select mm, cm, or m depending on your preference
3. **Enter Dimensions**: Input the length and width of the glass piece
4. **Get Price**: The total price calculates automatically

### Example

- Price per m²: R850
- Dimensions: 1200mm × 800mm
- Area: 0.960 m²
- **Total Price: R816.00**

## Building from Source

### Prerequisites

- [Node.js](https://nodejs.org) (v16 or higher)
- npm (comes with Node.js)

### Setup

1. Clone or download this repository
2. Navigate to the project folder:
   ```bash
   cd glass-calculator-app
   ```

3. Install dependencies:
   ```bash
   npm install
   ```

### Development

Run the app in development mode:
```bash
npm start
```

### Building the Installer

Create a Windows installer:
```bash
npm run build-win
```

The installer will be created in the `dist` folder.

## Project Structure

```
glass-calculator-app/
├── icon.ico          # Application icon
├── icon.png          # Window icon
├── package.json      # Project configuration
├── main.js           # Electron main process
├── index.html        # Application interface
├── node_modules/     # Dependencies
└── dist/             # Build output
```

## Technologies Used

- **Electron**: Desktop application framework
- **React**: UI library
- **Tailwind CSS**: Styling
- **electron-builder**: Application packaging

## Customization

### Changing the Default Price

Edit `index.html` and modify this line:
```javascript
const [pricePerSqm, setPricePerSqm] = useState(850);
```

You can also modify the price per m² in the actual app via the Settings icon in the top right corner.

### Changing Window Size

Edit `main.js` and modify the `createWindow` function:
```javascript
width: 1000,  // Change window width
height: 800,  // Change window height
```

## Support

For issues or questions, feel free to contact me.

## License

MIT License - Free to use and modify for your business needs.

## Version History

### Version 1.0.0 (2024)
- Initial release
- Basic pricing calculator functionality
- Custom dimension input
- Multiple unit support
- Settings panel for price adjustment

---

**Built specifically for Cubed Glass** 🇿🇦

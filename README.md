# Prayer Map - Islamic Prayer Times World Map Visualization

A web application that visualizes Islamic prayer times across the world in real-time, showing where each of the 5 daily prayers (plus the Ishraq period) is currently being observed.

## Features

- **Interactive World Map**: Displays the entire world divided into 6 colored sections representing different prayer times
- **Prayer Zones**:
  1. **Fajr** (Pre-dawn prayer) - Dark Blue
  2. **Ishraq** (Sunrise to Solar Noon) - Orange
  3. **Dhuhr** (Midday prayer) - Yellow
  4. **Asr** (Afternoon prayer) - Green
  5. **Maghrib** (Sunset prayer) - Red
  6. **Isha** (Night prayer) - Purple

- **Customizable Options**:
  - **Projection**: Choose map projection (Mercator default, Equirectangular)
  - **Time Selection**: Choose any specific date and time, or use slider to adjust (default: current time)
  - **Asr Method**: Select between Standard (Shafi'i, Maliki, Hanbali) or Hanafi calculation methods
  - **Calculation Method**: Choose from multiple Islamic prayer time calculation methods:
    - Muslim World League (MWL)
    - Islamic Society of North America (ISNA)
    - Egyptian General Authority
    - Umm Al-Qura University, Makkah
    - University of Islamic Sciences, Karachi
    - Institute of Geophysics, University of Tehran

## How to Use

1. **Open the Application**: Simply open `index.html` in a modern web browser
2. **View Prayer Zones**: The map automatically displays the current prayer times across the world
3. **Adjust Time**: 
   - Use the datetime picker to select a specific date and time
   - Or use the time slider for quick hour adjustments
4. **Change Settings**: 
   - Select your preferred Asr calculation method
   - Choose a prayer time calculation method
   - Click "Update Map" to apply changes
5. **Navigate**: Zoom and pan the map to explore different regions

## Technical Details

- **Built with**: HTML5, CSS3, JavaScript
- **Mapping Library**: Leaflet.js
- **Prayer Calculations**: Custom astronomical calculations based on sun position
- **Responsive Design**: Works on desktop and mobile devices

## Installation

No installation required! This is a standalone HTML file that runs entirely in the browser.

### Option 1: Local File
1. Download `index.html`
2. Open it in any modern web browser

### Option 2: Web Server
1. Host the `index.html` file on any web server
2. Access it via HTTP/HTTPS

### Option 3: GitHub Pages
This repository can be served directly via GitHub Pages.

## Browser Compatibility

- Chrome/Edge (recommended)
- Firefox
- Safari
- Opera

## License

MIT License

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
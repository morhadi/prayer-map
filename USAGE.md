# Prayer Map Usage Guide

## Quick Start

1. **Open the Application**
   - Simply open `index.html` in any modern web browser
   - Or serve it with any web server and navigate to it

2. **View Prayer Zones**
   - The map automatically displays the current prayer times across the world
   - Each color represents a different prayer time:
     - **Dark Blue**: Fajr (pre-dawn prayer)
     - **Orange**: Ishraq (sunrise to solar noon period)
     - **Yellow**: Dhuhr (midday prayer)
     - **Green**: Asr (afternoon prayer)
     - **Red**: Maghrib (sunset prayer)
     - **Purple**: Isha (night prayer)

## Controls

### Map Projection
- **Mercator** (default): Standard web map projection
- **Equirectangular**: Equal-area projection showing true relative sizes

### Time Selection
- **DateTime Picker**: Select any specific date and time
- **Time Slider**: Quickly adjust the hour (0-23.5 hours in 30-minute increments)
- Default: Current system time in UTC

### Asr Calculation Method
- **Standard**: Used by Shafi'i, Maliki, and Hanbali schools (shadow = object length + 1)
- **Hanafi**: Used by Hanafi school (shadow = object length + 2)

### Prayer Time Calculation Method
Choose from multiple recognized Islamic calculation methods:
- **Muslim World League (MWL)**: Widely used globally
- **ISNA**: Islamic Society of North America
- **Egyptian General Authority**: Used in Egypt and nearby regions
- **Umm Al-Qura, Makkah**: Used in Saudi Arabia
- **University of Islamic Sciences, Karachi**: Used in Pakistan
- **Tehran**: Institute of Geophysics method

### Update Map Button
Click to refresh the map with new settings or after changing parameters.

## Navigation

- **Pan**: Click and drag on the map to move around
- **Zoom In**: Click the `+` button or use mouse wheel up
- **Zoom Out**: Click the `−` button or use mouse wheel down

## Time Display

The current selected time is shown in the top-left corner of the map in UTC format.

## Tips

- The boundaries between prayer zones show where each prayer time is beginning
- The zones move westward as time progresses (following the sun)
- At any given moment, different parts of the world are in different prayer times
- Use the time slider to see how prayer zones change throughout the day
- Polar regions may show simplified prayer times due to extreme day/night cycles

## Examples

### See Current Prayer Times
1. Keep default settings
2. Observe which prayer zone your location is in

### See Prayer Times at Specific Time
1. Use the datetime picker to select a time
2. Click "Update Map"
3. View the global prayer distribution at that moment

### Compare Different Calculation Methods
1. Set a specific time
2. Select one calculation method and note the zones
3. Switch to another method and click "Update Map"
4. Observe the slight differences in boundaries

## Deployment

### GitHub Pages
1. Enable GitHub Pages in repository settings
2. Set source to the main/master branch
3. Access at `https://yourusername.github.io/prayer-map/`

### Local Server
```bash
# Python 3
python3 -m http.server 8080

# Python 2
python -m SimpleHTTPServer 8080

# Node.js (with http-server package)
npx http-server -p 8080
```

Then navigate to `http://localhost:8080/index.html`

## Technical Notes

- The application uses **real OpenStreetMap tiles** for authentic geographic data
- **Leaflet.js** provides professional-grade interactive mapping
- Prayer times are calculated based on astronomical sun angles relative to the horizon
- All calculations are performed in the browser (no server required)
- Prayer zones are rendered as a Canvas overlay on top of the real map
- Times are displayed in UTC; users should mentally convert to their local timezone
- Requires internet connection to load map tiles (first time and when panning/zooming)

## Browser Requirements

- Modern browser with HTML5 Canvas support
- JavaScript enabled
- Recommended: Chrome, Firefox, Safari, or Edge (latest versions)

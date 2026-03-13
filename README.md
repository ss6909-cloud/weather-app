# Weather App

A beautiful, responsive weather application built with vanilla HTML, CSS, and JavaScript. Get current weather for any city using the free Open-Meteo API.

## Features

✨ **Dark Theme with Glassmorphism** - Modern card design with blur effects
🌍 **Global Weather Data** - Search weather for any city worldwide
📊 **Detailed Weather Info** - Temperature, wind speed, humidity, and feels-like temperature
⚡ **Real-time Updates** - Instant weather data using Open-Meteo APIs
📱 **Fully Responsive** - Works perfectly on mobile, tablet, and desktop
🎨 **Smooth Animations** - Elegant fade-in and transitions
🚀 **No Dependencies** - Single HTML file, no frameworks, no npm required

## Setup Instructions

### macOS
1. **Download the file**: Save `index.html` to your computer
2. **Open in browser**: Double-click the `index.html` file in Finder
3. **Or use terminal**:
   ```bash
   open index.html
   ```

### Windows
1. **Download the file**: Save `index.html` to your computer
2. **Open in browser**: Double-click the `index.html` file in File Explorer
3. **Or right-click** and select "Open with" → your preferred browser

### Linux
1. **Download the file**: Save `index.html` to your computer
2. **Open in browser**: Double-click the file or use:
   ```bash
   xdg-open index.html
   ```

## Usage

1. Open `index.html` in any modern web browser
2. Enter a city name in the search bar
3. Click the "Search" button or press Enter
4. View the current weather conditions

**Examples**: London, New York, Tokyo, Sydney, Paris, Dubai

## APIs Used

This app uses free APIs with no authentication required:

- **Open-Meteo Geocoding API** - Converts city names to coordinates
  - Endpoint: `https://geocoding-api.open-meteo.com/v1/search`
- **Open-Meteo Weather API** - Fetches current weather and hourly data
  - Endpoint: `https://api.open-meteo.com/v1/forecast`

## Hosting on GitHub Pages

### Option 1: Single File Repository
1. Create a new GitHub repository named `weather-app` (or any name)
2. Upload the `index.html` file to the repository
3. Enable GitHub Pages:
   - Go to **Settings** → **Pages**
   - Select **Source**: "Deploy from a branch"
   - Select **Branch**: `main` → `/root`
   - Click **Save**
4. Your app will be live at: `https://yourusername.github.io/weather-app/`

### Option 2: Using Your Username Repository
1. Create a repository named `yourusername.github.io` (replace with your GitHub username)
2. Upload `index.html` as `index.html` in the root
3. Rename it or place it in a folder like `weather/index.html`
4. Access at: `https://yourusername.github.io/` (or `/weather/` if in subfolder)

### Option 3: Using a Docs Folder
1. Create any repository
2. Create a `docs/` folder
3. Place `index.html` inside
4. Enable GitHub Pages:
   - Settings → Pages
   - Source: `main` → `/docs`
   - Click **Save**

**Tips:**
- GitHub Pages updates within 1-2 minutes
- HTTPS is automatically enabled
- Custom domain support available (in Settings → Pages)

## Browser Compatibility

Works on:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## WMO Weather Codes

The app automatically converts WMO (World Meteorological Organization) weather codes to readable descriptions:
- 0: Clear sky
- 45: Fog
- 61: Slight rain
- 63: Moderate rain
- 80: Rain showers
- 95: Thunderstorm
- And 19+ more conditions

## File Structure

```
project/
├── index.html          # Single file containing HTML, CSS, and JavaScript
└── README.md          # This file
```

## Technical Details

### Technologies
- **HTML5** - Semantic structure
- **CSS3** - Glassmorphism design, animations, media queries
- **Vanilla JavaScript** - No frameworks, pure ES6+
- **Google Fonts** - Outfit typeface for modern design

### CSS Features
- CSS Grid for responsive layouts
- Backdrop filters for glassmorphism effect
- CSS animations for smooth transitions
- Media queries for mobile responsiveness

### JavaScript Features
- Async/await for API calls
- Fetch API for HTTP requests
- Dynamic DOM manipulation
- Event listeners for search functionality

## Customization

### Change Font

Replace the font link in the `<head>`:
```html
<!-- From: Outfit -->
<link href="https://fonts.googleapis.com/css2?family=Outfit:wght@400;500;600;700&display=swap" rel="stylesheet">

<!-- To: Syne -->
<link href="https://fonts.googleapis.com/css2?family=Syne:wght@400;500;600;700&display=swap" rel="stylesheet">
```

### Change Colors

Modify the CSS gradient colors:
```css
background: linear-gradient(135deg, #64f4ef, #8dd9ff); /* Cyan to blue */
```

### Change Default Temperature Unit

The app uses Celsius. To use Fahrenheit, modify in JavaScript:
```javascript
// Change this line:
temperature.textContent = `${Math.round(weatherData.temperature)}°C`;
// To this (multiply by 9/5 and add 32):
temperature.textContent = `${Math.round(weatherData.temperature * 9/5 + 32)}°F`;
```

## Troubleshooting

### "City not found" error
- Check spelling of the city name
- Try a larger city or add country name
- Some very small towns may not be in the database

### No results loading
- Check your internet connection
- The APIs may be temporarily unavailable (rarely)
- Try a different city
- Clear browser cache and reload

### App looks broken on mobile
- Update your browser to the latest version
- Some older Android browsers may have limited CSS support
- Use Chrome or Firefox for best compatibility

## Performance

- **Zero external dependencies** - No npm install needed
- **Instant load time** - Single HTML file (< 30KB)
- **Fast API calls** - Open-Meteo servers respond in < 500ms
- **Lightweight** - No build process, no bundler overhead

## Privacy & Data

- No data is stored locally or on servers
- No tracking or analytics
- All API calls are made directly from your browser
- No login or registration required

## License

This project is open source and free to use. Feel free to modify and redistribute.

## Contributing

Found a bug or want to improve the app? You're welcome to:
1. Report issues
2. Suggest features
3. Fork and create improvements
4. Share with others

## Credits

- **Open-Meteo** - Free weather API data
- **Google Fonts** - Outfit typeface
- **Inspiration** - Modern glassmorphism design trends

---

**Enjoy your weather app!** 🌦️

For questions or support, feel free to open an issue or contact the developer.

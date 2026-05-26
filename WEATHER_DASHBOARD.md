# 🌤️ Weather Dashboard

A modern, responsive weather dashboard that fetches real-time weather data from the Open-Meteo public weather API.

## Features

✅ **Real-Time Weather Data**
- Current temperature, humidity, wind speed, and pressure
- Weather condition with descriptive text
- "Feels like" temperature calculation

✅ **Multi-Location Support**
- Track weather for multiple cities simultaneously
- Add/remove locations with ease
- All locations displayed in a responsive grid

✅ **Comprehensive Forecasts**
- 24-hour hourly forecast with temperatures and conditions
- 7-day weather forecast with high/low temperatures
- Detailed precipitation and wind data

✅ **Smart Location Search**
- Search by city name globally
- Quick-access buttons for popular cities (London, New York, Tokyo, Paris, Sydney)
- Automatic geocoding to coordinates

✅ **Data Persistence**
- Auto-saves weather data to browser localStorage
- Locations persist across browser sessions
- Automatic timezone detection

✅ **Modern UI Design**
- Clean, intuitive interface
- Weather emoji indicators for conditions
- Responsive design (mobile, tablet, desktop)
- Smooth animations and hover effects
- Color-coded information (red for hot, blue for cold)

✅ **No API Key Required**
- Uses free Open-Meteo public API
- No registration needed
- Unlimited requests

## How to Use

1. **Open the Dashboard**
   - Open `weather-dashboard.html` in any modern web browser

2. **Search for a City**
   - Type a city name in the search box
   - Press Enter or click the Search button
   - Example: "London", "New York", "Tokyo"

3. **Use Quick Buttons**
   - Click any of the quick location buttons for instant results
   - Pre-configured: London, New York, Tokyo, Paris, Sydney

4. **View Weather Data**
   - Current conditions with temperature and emoji indicator
   - Detailed metrics: humidity, wind speed, pressure
   - 24-hour hourly forecast
   - 7-day weekly forecast

5. **Manage Locations**
   - Click "Delete" on any weather card to remove it
   - Add new locations anytime
   - All data saves automatically

## API Details

### Geocoding API
- **Endpoint**: `https://geocoding-api.open-meteo.com/v1/search`
- **Purpose**: Convert city names to coordinates
- **No authentication required**

### Weather API
- **Endpoint**: `https://api.open-meteo.com/v1/forecast`
- **Data provided**:
  - Current conditions (temperature, humidity, wind, pressure, weather code)
  - Hourly forecast (24 hours)
  - Daily forecast (14 days)
  - Automatic timezone detection
- **No authentication required**

## Weather Condition Codes

The app automatically converts WMO weather codes to emoji and descriptions:

- **0-3**: Clear to Overcast ☀️☁️
- **45-48**: Fog 🌫️
- **51-82**: Rain/Drizzle 🌧️
- **71-86**: Snow ❄️
- **95-99**: Thunderstorm ⛈️

## Data Storage

- **LocalStorage Key**: `weather_locations`
- **Format**: JSON array of weather objects
- **Persistence**: Data survives browser restarts
- **Privacy**: All data stored locally (no cloud sync)

## Technical Stack

- **HTML5**: Semantic markup
- **CSS3**: Modern styling with CSS Grid and Flexbox
- **Vanilla JavaScript**: No dependencies
- **Fetch API**: For HTTP requests
- **Open-Meteo API**: Free weather data

## Browser Compatibility

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Features Roadmap

- ⏳ Weather alerts for severe conditions
- ⏳ UV index and air quality data
- ⏳ Sunrise/sunset times
- ⏳ Historical weather data
- ⏳ Custom favorite cities list
- ⏳ Temperature unit toggle (°C/°F)
- ⏳ Map view integration

## Troubleshooting

**"Location not found" error**
- Double-check spelling
- Use English city names
- Try a larger city name (small towns may not be in the database)

**No data appears**
- Check internet connection
- Try a different city
- Clear browser cache and try again

**Weather data is old**
- Data is updated in real-time from Open-Meteo
- Try refreshing the page

## License

Free to use and modify.

## Credits

- Weather data: [Open-Meteo.com](https://open-meteo.com/)
- Geocoding data: [Open-Meteo Geocoding API](https://geocoding-api.open-meteo.com/)

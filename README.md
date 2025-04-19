# Weather Forecast Application

A modern, responsive weather application that provides real-time weather information and 5-day forecasts for cities worldwide, powered by OpenWeatherMap API and enhanced with Google Analytics 4 for user behavior tracking.

## Features

### Core Functionality
- Real-time weather data for any city worldwide
- 5-day weather forecast with hourly breakdowns
- Current temperature, wind speed, and humidity data
- Intelligent city search with autocomplete suggestions
- Support for international cities and multiple languages
- Automatic geolocation detection (optional)

### User Interface
- Modern, responsive design that works on all devices
- Dynamic weather backgrounds based on conditions
- Animated weather icons and transitions
- Error handling with user-friendly messages
- Loading indicators for better UX

### Analytics Implementation
- Google Analytics 4 integration for detailed usage tracking
- Custom event tracking for user interactions
- Performance monitoring
- Geographical usage statistics
- User retention tracking

## Technologies Used

- **Frontend:**
  - HTML5
  - CSS3 (Flexbox/Grid)
  - JavaScript (ES6+)
  - Font Awesome icons

- **APIs:**
  - OpenWeatherMap API
  - Google Analytics 4
  - Geolocation API

## Prerequisites

Before you begin, ensure you have:
- A modern web browser (Chrome, Firefox, Safari, Edge)
- An OpenWeatherMap API key (get one at [OpenWeatherMap](https://openweathermap.org/api))
- A Google Analytics 4 property (for analytics features)

## Setup and Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your_username/your_repository_name
   cd weather-app
   ```

2. **Configure API Keys**
   - Open `script.js`
   - Locate the configuration section at the top:
     ```javascript
     const API_KEY = 'your_openweathermap_api_key';
     const BASE_URL = 'https://api.openweathermap.org/data/2.5';
     const HOURLY_ITEMS_TO_SHOW = 24;
     ```
   - Replace `'your_openweathermap_api_key'` with your OpenWeatherMap API key
   - Get your API key from [OpenWeatherMap](https://openweathermap.org/api)

3. **Set Up Google Analytics**
   - In `index.html`, locate the GA4 tracking code:
     ```html
     <!-- Google Analytics 4 -->
     <script async src="https://www.googletagmanager.com/gtag/js?id=G-1RKT6F7578"></script>
     <script>
         window.dataLayer = window.dataLayer || [];
         function gtag(){dataLayer.push(arguments);}
         gtag('js', new Date());
         gtag('config', 'G-1RKT6F7578');
     </script>
     ```
   - Replace `G-1RKT6F7578` with your GA4 tracking ID

4. **Deploy to GitHub Pages**

   ```bash
   # Initialize git repository (if not already done)
   git init

   # Add all files
   git add .

   # Commit your changes
   git commit -m "Initial commit"

   # Create a new repository on GitHub
   # Go to github.com and create a new repository named: username.github.io
   # Replace 'username' with your GitHub username

   # Add remote repository
   git remote add origin https://github.com/username/username.github.io.git

   # Push to GitHub
   git push -u origin main
   ```

5. **Configure GitHub Pages**
   - Go to your GitHub repository
   - Click Settings → Pages
   - Under "Source", select main branch
   - Click Save
   - Your site will be published at `https://username.github.io`

6. **Verify Deployment**
   - Wait a few minutes for GitHub Pages to deploy
   - Visit your site at `https://username.github.io`
   - Check that:
     - Weather data loads correctly
     - Search functionality works
     - Analytics are tracking properly

7. **Updating Your Site**
   ```bash
   # Make your changes to the code
   
   # Stage changes
   git add .
   
   # Commit changes
   git commit -m "Description of your changes"
   
   # Push to GitHub
   git push origin main
   ```

8. **Troubleshooting**
   - If weather data doesn't load:
     - Check your API key in `script.js`
     - Verify API key is active at OpenWeatherMap
     - Check browser console for errors
   - If analytics aren't working:
     - Verify GA4 tracking ID in `index.html`
     - Check for ad blockers
     - Use GA4 Debug View to verify tracking

## Usage

1. **Basic Weather Search**
   - Enter a city name in the search box
   - Click the search icon or press Enter
   - View current weather and forecast

2. **Using Location Suggestions**
   - Start typing a city name
   - Wait for suggestions to appear
   - Click on a suggestion to view weather

3. **Viewing Detailed Weather**
   - Current conditions are shown at the top
   - Scroll down for hourly forecast
   - View 5-day forecast at the bottom

## Analytics Features

### Tracked Metrics
1. **Page Views & User Interactions**
   - Page visits
   - Search attempts
   - Feature usage
   - Time on page

2. **Custom Events**
   - Weather searches
   - City selections
   - Forecast views
   - Error occurrences

3. **Performance Metrics**
   - Page load time
   - API response time
   - Search response time
   - Resource timing

4. **Geographical Data**
   - User locations
   - Searched cities
   - Popular regions
   - Usage patterns

### Viewing Analytics
1. Access your GA4 dashboard
2. Navigate to Reports > Realtime
3. View custom events under Events
4. Check performance under Tech > Web Vitals

## Troubleshooting

### Common Issues
1. **API Key Issues**
   - Verify your API key in `script.js`
   - Check API usage limits
   - Ensure proper key formatting

2. **Analytics Not Working**
   - Verify GA4 tracking ID
   - Check for ad blockers
   - Enable JavaScript in browser

3. **Search Problems**
   - Check internet connection
   - Verify city name spelling
   - Try using suggestion feature

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request


## Acknowledgments

- OpenWeatherMap for weather data
- Google Analytics for tracking capabilities
- Font Awesome for weather icons
- Contributors and testers
# 🛰️ NASA AgriScan PRO

**Global Satellite Agriculture Intelligence Dashboard**

A comprehensive, real-time agricultural monitoring platform that leverages live satellite imagery, weather data, and advanced analytics to help farmers, researchers, and agricultural students make data-driven decisions.

![NASA AgriScan PRO](https://img.shields.io/badge/Status-Live-green) ![100% Live APIs](https://img.shields.io/badge/Data-100%25%20Live%20APIs-blue) ![HTML5](https://img.shields.io/badge/Built%20With-HTML5%2FCSS%2FJS-orange)

---

## 🌟 Features

### 📍 Location-Based Intelligence
- **GPS/Device Location Detection** - One-click location access via browser geolocation
- **Worldwide Search** - Search and analyze any location on Earth
- **Real-time Coordinate Resolution** - Nominatim-powered reverse geocoding

### 🛰️ Live Satellite Data Integration
- **NASA GIBS Satellite Tiles** - Real NASA satellite products including:
  - MODIS Terra/Aqua NDVI (Normalized Difference Vegetation Index)
  - MODIS Land Surface Temperature
  - NASA FIRMS VIIRS Active Fires (375m real-time)
  - GPM Precipitation Data
- **Multi-Layer Mapping** - Toggle between street, satellite, NDVI, land temp, precipitation, and fire detection views
- **Sentinel-2 & MODIS Integration** - Professional-grade Earth observation data

### 🌦️ Advanced Weather Analytics
- **48-Hour Hourly Forecasts** - Temperature, precipitation, wind, humidity trends
- **7-Day Extended Forecast** - Comprehensive weather outlook
- **Real-time Conditions** - Current temperature, feels-like, air quality, pressure, cloud cover
- **Open-Meteo Weather API** - Continuously updated live meteorological data

### 🌾 Crop Monitoring
- **Multi-Crop Support** - 15+ crop types including:
  - Wheat, Rice, Corn, Soybean, Cotton
  - Sugarcane, Barley, Potato, Tomato
  - Groundnut, Sunflower, Mustard, Chickpea, Millet, Sorghum
- **Live NDVI Analysis** - Satellite-derived vegetation health estimates
- **Growing Degree Days (GDD)** - 7-day trend for crop development tracking
- **Crop Coefficient Integration** - FAO-standard crop water requirement calculations

### 🧪 Soil Analysis Engine
- **Soil Parameters** - pH, Nitrogen (N), Phosphorus (P), Potassium (K), Organic Matter tracking
- **Soil Texture Classification** - Sandy, Loamy, Clay Loam, Silty, Clay categorization
- **Irrigation System Support** - Drip, Flood, Sprinkler, and Rainfed options
- **ET₀ Integration** - Reference evapotranspiration calculations for precision irrigation

### 🔬 Disease Risk Intelligence
- **Satellite-Based Risk Scoring** - Automated disease pressure models computed from:
  - Temperature & humidity patterns
  - Precipitation trends
  - Dew point & leaf wetness (VPD modeling)
  - NDVI anomalies
  - Cloud cover analysis
- **Pathogen-Specific Analysis** - Multi-disease pressure tracking
- **5-Minute Auto-Refresh** - Continuous, real-time risk monitoring
- **No Manual Upload Required** - Fully automated satellite-to-risk analysis pipeline

### 💧 Smart Irrigation Management
- **Precision Water Scheduling** - ET₀ vs. Precipitation analysis
- **48-Hour Soil Moisture Estimates** - Data-driven irrigation recommendations
- **Live Weather Integration** - Automatic adjustments based on current/forecast conditions

### 📈 Global Commodity Price Tracking
- **Real-Time FX Conversion** - EUR/USD live rates from ECB Frankfurter API (60-second updates)
- **CBOT/ICE Reference Prices** - Major agricultural commodities with live data
- **30-Day Price Trends** - Historical FX fluctuation tracking
- **Commodity Price Index** - Normalized, comparative market analysis

### 🚨 Real-Time Alert System
- **Satellite + Weather-Driven Alerts** - Dynamic alert generation based on:
  - Extreme weather events
  - Disease risk thresholds
  - Soil moisture anomalies
  - Market price movements
- **5-Minute Refresh Cycle** - Continuous monitoring for critical conditions

### 🛸 Satellite Constellation Intelligence
- **Global Coverage Tracking** - NASA, ESA, ISRO, NOAA satellite status
- **Pass Prediction** - Orbital mechanics-calculated satellite passes over your location
- **ISS Real-Time Tracking** - 5-second refresh ISS position updates (wheretheiss.at API)
- **Data Volume Estimates** - GIBS data acquisition volume tracking (GB/day)

---

## 📊 Live Data Sources

| Data Type | Source | Update Frequency | Coverage |
|-----------|--------|------------------|----------|
| **Weather** | Open-Meteo API | Real-time | Global |
| **Air Quality** | Open-Meteo AQ API | Live | Global |
| **Satellite Imagery** | NASA GIBS | Real-time (5-min) | Global |
| **Active Fires** | NASA FIRMS VIIRS | 375m Real-time | Global |
| **Vegetation Index** | MODIS Terra/Aqua | 8-day composite | Global |
| **Land Surface Temp** | MODIS | Real-time | Global |
| **Precipitation** | GPM | Real-time | Global |
| **FX Rates** | ECB Frankfurter | 60-second | EUR/USD |
| **ISS Position** | wheretheiss.at | 5-second refresh | Real-time |

---

## 🚀 Quick Start

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- Internet connection
- GPS/location access (optional, for device location feature)

### Access the Application
1. Visit: **https://rahulkneet2003-gif.github.io/Agri_scan/**
2. Allow browser location access (recommended)
3. Or search for any worldwide location
4. Start analyzing!

### No Installation Required
- 100% client-side web application
- Pure HTML5/CSS/JavaScript
- No backend server dependency
- No API keys needed (uses public APIs)

---

## 📁 Project Structure

```
Agri_scan/
├── index.html              # Main single-file application
├── README.md               # This file
└── .github/
    └── workflows/          # GitHub Pages deployment
```

---

## 🏗️ Architecture

### Frontend Stack
- **HTML5** - Semantic markup & structure
- **CSS3** - Responsive design & styling
- **Vanilla JavaScript** - No framework dependencies

### API Integrations
```
┌─────────────────────────────────────────────────────────────┐
│                   NASA AgriScan PRO                         │
├──────────┬──────────┬──────────┬──────────┬──────────────────┤
│ Location │ Weather  │ Satellite│ Market   │ Satellite Info   │
│ Services │ Services │ Services │ Services │ Services         │
├──────────┼──────────┼──────────┼──────────┼──────────────────┤
│Nominatim │Open-Meteo│NASA GIBS │ECB Frankf│wheretheiss.at   │
│ Geocoding│  Weather │ MODIS    │  FX API  │  ISS Position    │
│          │  AQ Data │ VIIRS    │          │  Orbital Calcs   │
└──────────┴──────────┴──────────┴──────────┴──────────────────┘
```

### Key JavaScript Features
- **Asynchronous API Calls** - Parallel data fetching
- **Real-Time Canvas Rendering** - Dynamic chart updates
- **WebGL Map Rendering** - Leaflet.js with NASA tile layers
- **Responsive Grid Layout** - Mobile-first design
- **localStorage Caching** - Session state persistence
- **GPS Geolocation API** - Device location access

---

## 📖 Usage Guide

### 1. **Select Your Location**
```
Click "Use GPS" → Allow location access
OR
Search → Enter location name → Press Enter
```

### 2. **View Live Satellite Map**
Switch between layers:
- 🗺️ Street (OpenStreetMap)
- 🛰️ Satellite (NASA/ESA)
- 🌿 NDVI (Vegetation health)
- 🌡️ Land Temp (Temperature)
- 🌧️ Precip (Precipitation)
- 🔥 Active Fire (Fire detection)

### 3. **Monitor Weather**
- View 48-hour trends
- Check 7-day forecast
- Track hourly conditions

### 4. **Analyze Crops**
1. Select your field location
2. Choose crop type from dropdown
3. View NDVI estimate
4. Track Growing Degree Days
5. Review stress indicators

### 5. **Manage Irrigation**
1. Enter soil parameters
2. Specify field details
3. System calculates ET₀ vs. Precipitation
4. Receive water scheduling recommendations

### 6. **Track Disease Risk**
- View pathogen-specific pressure scores
- Monitor humidity/temperature correlations
- 5-minute auto-refresh alerts

### 7. **Monitor Market Prices**
- Track commodity prices (live EUR/USD conversion)
- View 30-day FX trends
- Normalize prices across markets

---

## 🔄 Real-Time Data Pipeline

```
Every 5 Minutes:
├── Weather API → Open-Meteo
├── Satellite Tiles → NASA GIBS (new data layer download)
├── Disease Risk Models → Recalculation from new weather
├── Active Fire Detection → NASA FIRMS update
├── Alerts → Re-evaluation & push notification (if enabled)
└── ISS Position → wheretheiss.at (5-second sub-cycle)

Every 60 Seconds:
└── FX Rates → ECB Frankfurter EUR/USD update

Every Session:
├── Nominatim Geocoding → Location search
├── Satellite Pass Prediction → Orbital mechanics compute
└── localStorage → User preferences & session state
```

---

## 🎯 Use Cases

### For Farmers
- ✅ Precision irrigation scheduling
- ✅ Early disease detection
- ✅ Crop health monitoring via satellite
- ✅ Weather-based decision support
- ✅ Market price tracking for sales timing

### For Agricultural Researchers
- ✅ Multi-temporal NDVI analysis
- ✅ Climate-crop relationship studies
- ✅ Disease epidemiology research
- ✅ Soil-weather integration studies
- ✅ Global agricultural monitoring

### For Agricultural Students
- ✅ Real-world satellite data access
- ✅ Live weather integration learning
- ✅ Crop science practical application
- ✅ Precision agriculture concepts
- ✅ Professional-grade tools experience

### For Agribusiness
- ✅ Market commodity tracking
- ✅ Regional crop health assessment
- ✅ Risk management decision support
- ✅ Supply chain intelligence

---

## 🌐 Browser Compatibility

| Browser | Version | Status |
|---------|---------|--------|
| Chrome | 90+ | ✅ Full Support |
| Firefox | 88+ | ✅ Full Support |
| Safari | 14+ | ✅ Full Support |
| Edge | 90+ | ✅ Full Support |
| Mobile Chrome | Latest | ✅ Responsive |
| Mobile Safari | Latest | ✅ Responsive |

---

## 📱 Mobile Optimization

- **Responsive Design** - Works on smartphones, tablets, desktops
- **Touch-Friendly** - Optimized controls for mobile
- **GPS Integration** - Native device location access
- **Lightweight** - Single HTML file (~2MB with data)
- **Offline Capable** - Cached data loads without connectivity

---

## 🔐 Data & Privacy

- **No User Data Collection** - All processing client-side
- **No Account Required** - Completely anonymous usage
- **No Login Needed** - Immediate access to all features
- **Public APIs Only** - All data from public, free APIs
- **No Tracking** - No analytics or user tracking

---

## 🛠️ Technical Details

### API Endpoints Used

**Nominatim Geocoding**
```
https://nominatim.openstreetmap.org/search?format=json&q={query}
```

**Open-Meteo Weather**
```
https://api.open-meteo.com/v1/forecast?latitude={lat}&longitude={lon}&...
```

**Open-Meteo Air Quality**
```
https://air-quality-api.open-meteo.com/v1/air_quality?...
```

**NASA GIBS Tiles**
```
https://gibs.earthdata.nasa.gov/wmts-webmerc/{layer}/default/{date}/{tilematrixset}/...
```

**ECB Frankfurter FX**
```
https://api.frankfurter.app/latest?from=EUR&to=USD
```

**wheretheiss.at ISS**
```
https://api.wheretheiss.at/v1/satellites/25544
```

---

## 📊 Data Calculations

### Growing Degree Days (GDD)
```
GDD = Σ [(T_max + T_min)/2 - T_base]
where T_base = crop-specific base temperature (typically 10°C)
```

### Evapotranspiration (ET₀)
```
Standardized FAO-56 Penman-Monteith equation
Inputs: Temperature, Humidity, Wind Speed, Solar Radiation
```

### NDVI (Normalized Difference Vegetation Index)
```
NDVI = (NIR - Red) / (NIR + Red)
Range: -1 to +1
-1: Bare/Water, 0: No Vegetation, +1: Dense Vegetation
```

### Disease Risk Scoring
```
Risk = f(Temperature, Humidity, Precipitation, VPD, NDVI_anomaly, Cloud_cover)
Computed for: Fungal blights, mildews, leaf spots, rusts, etc.
```

---

## 🚨 Common Issues & Solutions

### "Satellite data not loading"
- **Cause**: NASA GIBS service may be temporarily offline
- **Solution**: Refresh page, check your internet connection, try different map layer

### "Location not found"
- **Cause**: Search location not recognized by Nominatim
- **Solution**: Use city name instead of coordinates, try broader search

### "GPS not working"
- **Cause**: Browser permission denied or device without GPS
- **Solution**: Allow location access in browser settings, or manually search location

### "Weather API timeout"
- **Cause**: Network latency or Open-Meteo service load
- **Solution**: Wait 30 seconds, refresh page, check internet speed

---

## 🤝 Contributing

Contributions are welcome! To contribute:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/AmazingFeature`)
3. **Commit** changes (`git commit -m 'Add AmazingFeature'`)
4. **Push** to branch (`git push origin feature/AmazingFeature`)
5. **Open** a Pull Request

### Contribution Ideas
- [ ] Add more crop types
- [ ] Implement soil moisture sensors integration
- [ ] Add regional language support
- [ ] Create historical data dashboard
- [ ] Add multi-field comparison tools
- [ ] Implement weather alerts push notifications
- [ ] Add export reports (PDF/CSV)
- [ ] Mobile app version

---

## 📝 License

This project is open-source and available under the **MIT License**.

---

## 👨‍💻 Author

**Rahul Kneet Singh** (rahulkneet2003-gif)
- GitHub: [@rahulkneet2003-gif](https://github.com/rahulkneet2003-gif)
- Project: [NASA AgriScan PRO](https://github.com/rahulkneet2003-gif/Agri_scan)

---

## 🙏 Acknowledgments

### Data Providers
- **NASA** - GIBS satellite imagery, MODIS, VIIRS, FIRMS
- **ESA** - Sentinel satellite data integration
- **ISRO** - Indian satellite constellation
- **NOAA** - Weather & climate data
- **Open-Meteo** - Weather & air quality APIs
- **OpenStreetMap/Nominatim** - Geocoding services
- **ECB Frankfurter** - Real-time FX data
- **wheretheiss.at** - ISS tracking API

### Libraries & Frameworks
- Leaflet.js - Interactive mapping
- Chart.js - Data visualization
- CORS Proxy - Cross-origin requests
- OpenStreetMap Contributors

---

## 📞 Support & Contact

- **Report Issues**: [GitHub Issues](https://github.com/rahulkneet2003-gif/Agri_scan/issues)
- **Suggest Features**: [GitHub Discussions](https://github.com/rahulkneet2003-gif/Agri_scan/discussions)
- **Email**: Contact via GitHub profile

---

## 📚 Learning Resources

### Satellite Agriculture
- [NASA GIBS Documentation](https://wiki.earthdata.nasa.gov/display/GIBS/)
- [MODIS Overview](https://modis.gsfc.nasa.gov/)
- [Precision Agriculture Guide](https://www.usda.gov/)

### Remote Sensing
- [NDVI Explained](https://www.usgs.gov/faqs/what-normalized-difference-vegetation-index)
- [Satellite Imagery Analysis](https://www.esa.int/Applications/Observing_the_Earth)

### Agricultural APIs
- [Open-Meteo API](https://open-meteo.com/)
- [NASA GIBS API](https://wiki.earthdata.nasa.gov/display/GIBS/)

---

## 🎓 Citation

If you use NASA AgriScan PRO in research, please cite:

```
Singh, Rahul Kneet. (2026). NASA AgriScan PRO: Global Satellite Agriculture Intelligence.
GitHub Repository: https://github.com/rahulkneet2003-gif/Agri_scan
```

---

## ⭐ Show Your Support

If you find this project helpful, please consider:
- ⭐ Starring the repository
- 🔗 Sharing with peers & colleagues
- 📢 Mentioning in articles/presentations
- 🤝 Contributing improvements

---

**Last Updated**: May 2026  
**Status**: ✅ Active Development  
**Deployment**: GitHub Pages (100% Live APIs)

---

*"Making professional satellite agriculture intelligence accessible to everyone."*

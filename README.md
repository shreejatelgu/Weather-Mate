# 🌦️ WeatherMate  
### *Your Smart Personal Weather Companion*

WeatherMate is a clean and modern weather dashboard that automatically detects your location and displays real-time weather conditions with an elegant UI. Built using **React, TypeScript, TailwindCSS, ShadCN UI, and React Query**, it delivers fast, accurate, and smooth weather updates.

---

## ✨ Features

- 📍 **Auto Location Detection** (via browser geolocation)
- 🌤️ **Current Weather Details**
  - Temperature  
  - Feels Like  
  - Humidity  
  - Wind Speed  
  - Weather Conditions
- 📅 **5-Day / 3-Hour Forecast**
- 🗺️ **Reverse Geocoding** → Get city, state, country automatically
- ⚡ **Instant Refresh** with loading animations
- 🎨 **Aesthetic UI** (Tailwind + ShadCN)
- 🧊 **Smooth Skeleton Loading Screens**
- ❌ **Friendly Error Handling** for:
  - Location disabled
  - Network issues
  - API errors

---

## 🛠️ Tech Stack

| Technology | Purpose |
|-----------|---------|
| **React + TypeScript** | Core UI logic |
| **Vite** | Fast development environment |
| **React Query** | Data fetching + caching |
| **TailwindCSS** | Styling |
| **ShadCN UI** | Prebuilt components |
| **Lucide Icons** | Icons |
| **OpenWeather API** | Weather, forecast, and geolocation |

---

## 📁 Project Structure

```bash
src/
│── api/
│   ├── weather.ts          # OpenWeather API wrapper
│   ├── config.ts           # API URLs + keys
│   └── types.ts            # TypeScript interfaces
│
│── hooks/
│   ├── use-geolocation.ts  # Browser geolocation logic
│   └── use-weather.ts      # React Query hooks
│
│── components/
│   ├── current-weather.tsx
│   ├── forecast.tsx
│   ├── loading-skeleton.tsx
│   └── ui/                 # ShadCN UI Components
│
└── pages/
    └── weather-dashboard.tsx

🌍 API Endpoints Used

Current Weather:
/weather

5-Day Forecast:
/forecast

Reverse Geocoding:
/geo/1.0/reverse

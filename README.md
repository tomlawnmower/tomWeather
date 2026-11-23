# TomWeather

A zero-dependency, single-page hourly weather application built with vanilla HTML, CSS, and JavaScript.

## Features

- **Location Search & Geocoding**:
  - Search by 5-digit US ZIP code (via [Zippopotam.us](https://api.zippopotam.us)) or city name (via [Open-Meteo Geocoding API](https://geocoding-api.open-meteo.com)).
  - Supports US state abbreviations (e.g., `Denver, CO` or `78701`).
  - Remembers recent searches as quick-access chips stored in `localStorage`.
- **Forecasts & Data Sources**:
  - Powered by the [Open-Meteo Weather Forecast API](https://open-meteo.com/).
  - Displays hourly temperature, precipitation probability, snowfall, and daily summaries (high/low temperatures, weather condition icons, precipitation sums, and sunrise/sunset times).
  - Client-side caching (30-minute TTL) in `localStorage` with offline fallback support.
- **Interactive Visualizations**:
  - Dynamic inline SVG charts for hourly temperature and precipitation/snowfall probabilities.
  - Day/night background bands calculated from solar sunrise and sunset times.
  - Real-time "now" line showing current local time relative to the forecast.
  - Crosshair scrubber with hover/touch tooltip displaying exact hourly readings.
  - Horizontal drag-to-scroll navigation for both mouse and touch input.
- **Controls & Theming**:
  - Unit toggle (°F / °C / Both) with dynamic conversion.
  - Forecast range toggle (7 days / 16 days).
  - Manual data refresh button.
  - Automatic light/dark mode support based on system settings (`prefers-color-scheme`).

## Getting Started

Because TomWeather has no external build steps or dependencies, simply open [index.html](file:///D:/gitwork/TomWeather/index.html) in any modern web browser:

```bash
# Open directly or run a lightweight local server:
python -m http.server
# or
npx serve .
```

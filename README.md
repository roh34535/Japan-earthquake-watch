# Japan Earthquake Watch

A live dashboard of earthquakes in and around Japan, built with plain HTML, CSS and JavaScript (no build step).

**Live demo:** https://roh34535.github.io/Japan-earthquake-watch/



## Why I built it
Earthquakes are part of daily life in Japan. I wanted a fast, readable view of what is happening right now, with the language switchable between English and Japanese.

## Features
- Live data from the USGS Earthquake Hazards Program API (no API key)
- Interactive Leaflet map: marker size and color show magnitude, popups show time, depth and a USGS link
- Filters: time range (24h / 7 days / 30 days) and minimum magnitude
- Stats: event count, strongest quake, average depth, time since the latest event
- Chart of earthquakes per day (Japan Standard Time)
- "Strongest events" list that flies the map to the selected quake
- English / 日本語 interface toggle
- Responsive layout, dark mode support, error and empty states

## Tech
HTML, CSS, vanilla JavaScript, [Leaflet](https://leafletjs.com), [Chart.js](https://www.chartjs.org), Esri map tiles.

## Run locally
Open `index.html` in a browser, or run `python3 -m http.server` in this folder and visit http://localhost:8000.

## Deploy
Push to GitHub, then Settings → Pages → deploy from the `main` branch root.

## What I would add next
- Official JMA data and Japanese place names
- Seismic intensity (shindo) scale instead of magnitude only
- Auto-refresh and notifications for large events
- Tests for the data-processing functions

## Limitations
Data is from USGS, not the Japan Meteorological Agency. This is a learning project, not an official warning system.

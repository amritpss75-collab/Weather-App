# Wayfinder — Weather, places & travel

React + TypeScript + Vite starter, ready for GitHub and Vercel.

## Features
- Worldwide place search (country, state, city and locality) using Open-Meteo geocoding.
- Current conditions, hourly outlook, 7-day forecast and an extended outlook.
- Nearby restaurants, museums, cinema, arts, music and family-friendly places using OpenStreetMap / Overpass.
- Approximate distance from the selected location centre and Google Maps directions links.
- Road, transit/train and flight search links.

## Run locally
Node.js 18+ is recommended.

```bash
npm install
npm run dev
```

## Deploy
1. Push this folder to a GitHub repository.
2. Import the repository in Vercel.
3. Select Vite, build command `npm run build`, output directory `dist`.
4. Deploy. Future GitHub pushes trigger deployments.

## Data and limitations
Weather: Open-Meteo (no API key for this demo). Places: OpenStreetMap via public Overpass API; coverage and availability vary. Maps and directions: Google Maps URLs.
The extended/monthly view summarises the available forecast window (up to 16 days); it is not a precise 30-day daily forecast. Transport links open search/directions pages. Live ticket prices are not fabricated: reliable road/train/flight prices need a date-specific fare provider/API and often API credentials. This starter does not send alerts or persist saved places between devices.
For production, consider Supabase for accounts and saved locations, a server-side cache for Overpass requests, and a transport fare API plus scheduled notification service.

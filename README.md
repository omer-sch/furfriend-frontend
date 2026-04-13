# FurFriend — Frontend

[![React](https://img.shields.io/badge/React_18-61DAFB?style=flat-square&logo=react&logoColor=black)](https://react.dev)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)](https://www.typescriptlang.org)
[![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)](https://vitejs.dev)
[![Google Maps](https://img.shields.io/badge/Google_Maps_API-4285F4?style=flat-square&logo=google-maps&logoColor=white)](https://developers.google.com/maps)

React + TypeScript frontend for **FurFriend** — a social platform for pet lovers. Share posts, connect with nearby pet owners on a map, and get local weather conditions.

> **Related:** [furfriend_Back](https://github.com/omer-sch/furfriend_Back) — Node.js + Express + MongoDB REST API

---

## Features

- 📸 **Post Feed** — browse, create, and interact with pet posts
- 💬 **Comments** — add and view comments on posts
- 👤 **User Profiles** — view and edit your profile
- 🗺️ **Interactive Map** — see nearby pet owners via Google Maps API
- 📍 **Live Location** — share and display user location on the map
- 🌦️ **Weather Widget** — real-time local weather via OpenWeather API
- 🔐 **Authentication** — register and login with JWT-based auth

---

## Project Structure

```
src/
├── App.tsx
├── main.tsx
├── components/
│   ├── Comments/
│   │   ├── AddComment.tsx       # Comment input form
│   │   └── PostComment.tsx      # Single comment display
│   ├── Map/
│   │   ├── GoogleMaps.tsx       # Google Maps embed with pet owner pins
│   │   └── UserLocation.tsx     # Get + broadcast current location
│   ├── NavBarLine/
│   │   └── BarLine.tsx          # Top navigation bar
│   ├── Posting/
│   │   ├── AddPost.tsx          # Create new post with image upload
│   │   ├── Post.tsx             # Single post card (image, likes, comments)
│   │   ├── PostsList.tsx        # Feed of all posts
│   │   └── MyPosts.tsx          # Current user's posts
│   ├── Profile/
│   │   └── Profile.tsx          # User profile page
│   ├── Registeration/
│   │   ├── Login.tsx            # Login form
│   │   └── Register.tsx         # Registration form
│   └── Weather/
│       ├── OpenWeather.tsx      # Weather data fetch + display
│       └── Rain.tsx             # Rain animation overlay
```

---

## Tech Stack

| | Technology |
|--|-----------|
| Framework | React 18 |
| Language | TypeScript |
| Build Tool | Vite |
| Routing | React Router |
| HTTP Client | Axios |
| Maps | Google Maps JavaScript API |
| Weather | OpenWeather API |

---

## Getting Started

```bash
git clone https://github.com/omer-sch/furfriend-frontend.git
cd furfriend-frontend
npm install
```

Create a `.env` file:

```env
VITE_API_URL=http://localhost:3000
VITE_GOOGLE_MAPS_API_KEY=your_key_here
VITE_OPENWEATHER_API_KEY=your_key_here
```

```bash
npm run dev      # → http://localhost:5173
npm run build    # production build
npm run preview  # preview production build
```

---

## Related

- **Backend:** [furfriend_Back](https://github.com/omer-sch/furfriend_Back) — Node.js + Express + MongoDB REST API

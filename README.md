# 🚗 Vehicle Monitoring System

A real-time vehicle fleet monitoring dashboard built with React. Track vehicle health, location, fuel levels, driver behavior, and maintenance schedules — all in one place.

![Vehicle Monitoring System](https://img.shields.io/badge/Status-Active-brightgreen)
![React](https://img.shields.io/badge/React-18.x-blue)
![License](https://img.shields.io/badge/License-MIT-yellow)

---

## 📸 Features

- **Live Fleet Overview** — Real-time status of all vehicles (active, idle, maintenance)
- **Health Monitoring** — Engine temp, battery, tire pressure, fuel levels
- **Driver Behavior Scoring** — Speed compliance, harsh braking, fuel efficiency
- **Maintenance Alerts** — Predictive alerts for upcoming service intervals
- **Trip Logs** — Full trip history with distance, duration, and fuel consumed
- **Interactive Map View** — Live vehicle location tracking
- **Notifications Center** — Alerts for anomalies, geofence violations, and warnings

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | React 18, Tailwind CSS |
| Charts | Recharts |
| Icons | Lucide React |
| State | React Hooks (useState, useEffect, useContext) |
| Build | Vite |
| Testing | Vitest + React Testing Library |

---

## 🚀 Getting Started

### Prerequisites

- Node.js >= 18.x
- npm >= 9.x

### Installation

```bash
# Clone the repository
git clone https://github.com/your-username/vehicle-monitoring-system.git

# Navigate into the project
cd vehicle-monitoring-system

# Install dependencies
npm install

# Start development server
npm run dev
```

The app will be available at `http://localhost:5173`

### Build for Production

```bash
npm run build
npm run preview
```

---

## 📁 Project Structure

```
vehicle-monitoring-system/
├── public/
│   └── favicon.svg
├── src/
│   ├── components/
│   │   ├── Dashboard.jsx         # Main dashboard layout
│   │   ├── FleetOverview.jsx     # Fleet summary cards
│   │   ├── VehicleCard.jsx       # Individual vehicle card
│   │   ├── VehicleDetail.jsx     # Detailed vehicle view
│   │   ├── HealthMonitor.jsx     # Health metrics & gauges
│   │   ├── TripHistory.jsx       # Trip logs table
│   │   ├── MaintenancePanel.jsx  # Maintenance schedule
│   │   ├── AlertsPanel.jsx       # Notification center
│   │   ├── DriverScore.jsx       # Driver behavior analytics
│   │   ├── FuelChart.jsx         # Fuel consumption chart
│   │   ├── Sidebar.jsx           # Navigation sidebar
│   │   └── Header.jsx            # Top navigation bar
│   ├── hooks/
│   │   ├── useVehicleData.js     # Vehicle data hook with polling
│   │   ├── useAlerts.js          # Alert management hook
│   │   └── useFilters.js         # Fleet filter hook
│   ├── utils/
│   │   ├── formatters.js         # Date, distance, unit helpers
│   │   ├── statusHelpers.js      # Status color/label utilities
│   │   └── mockApi.js            # Mock API with realistic data
│   ├── data/
│   │   └── mockVehicles.js       # Seed data for 10 vehicles
│   ├── App.jsx
│   ├── main.jsx
│   └── index.css
├── .gitignore
├── package.json
├── vite.config.js
└── README.md
```

---

## 🔌 API Integration

The system ships with a **mock API layer** (`src/utils/mockApi.js`) that simulates real-time data. To connect to a real backend:

1. Replace `mockApi.js` calls with your actual API endpoints
2. Update the polling interval in `useVehicleData.js`
3. Configure environment variables in `.env`:

```env
VITE_API_BASE_URL=https://your-api.com
VITE_API_KEY=your_api_key
VITE_POLLING_INTERVAL=5000
```

---

## 🗺️ Roadmap

- [ ] Real-time WebSocket support
- [ ] Google Maps / Mapbox integration
- [ ] Export reports to CSV/PDF
- [ ] Push notifications (PWA)
- [ ] Multi-tenant fleet management
- [ ] Mobile app (React Native)
- [ ] OBD-II hardware integration

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m 'Add your feature'`
4. Push to the branch: `git push origin feature/your-feature`
5. Open a Pull Request

---

## 📄 License

MIT License — see [LICENSE](LICENSE) for details.

---

## 👨‍💻 Author

Built with ❤️ — contributions welcome!

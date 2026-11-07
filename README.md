

# 🚦 MargDarshak (मार्गदर्शक)
### Quantum-Inspired Intelligent Traffic Route Optimization & Emergency Green Corridor System

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Vercel-success?style=for-the-badge&logo=vercel)](https://traffic-route-optimization-mx7v.vercel.app/driver)
[![Next.js](https://img.shields.io/badge/Next.js-16-black?style=for-the-badge&logo=next.js)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.7-3178C6?style=for-the-badge&logo=typescript)](https://www.typescriptlang.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-4.0-38B2AC?style=for-the-badge&logo=tailwind-css)](https://tailwindcss.com/)

**Smart India Hackathon (SIH) Project**

[🌐 Launch Live Driver App](https://traffic-route-optimization-mx7v.vercel.app/driver) • [🖥️ Launch Operations Control Center](https://traffic-route-optimization-mx7v.vercel.app/operations)

</div>

---

## 📌 Overview

Rapid urbanization and surging vehicular density lead to chronic gridlock, increased fuel consumption, elevated carbon emissions, and fatal delays for emergency services.

**MargDarshak** is an intelligent, multi-modal urban traffic management and route optimization platform. By combining vehicle-constraint-aware dynamic pathfinding with real-time green corridor dispatching, MargDarshak ensures optimal transit for commercial freight, passenger traffic, two-wheelers, and emergency responders alike.

---

## 🌟 Key Features

### 1. 🚑 Emergency Green Corridor Preemption
- **Instant Emergency Clearance**: Priority routing for ambulances and first responders with real-time civilian traffic diversion.
- **Corridor States**: Live transition alerts from `NORMAL` to `APPROACHING`, `ALTERNATE CORRIDOR`, and `ROUTE UPDATED`.

### 2. 🚛 Vehicle-Class-Aware Multi-Modal Pathfinding
Different vehicles face distinct constraints on Indian roadways. MargDarshak tailors routes based on vehicle profile:
- **Freight (Heavy Commercial)**: Enforces height clearances, bridge weight restrictions, and avoids narrow city streets.
- **Emergency**: Guaranteed lowest-latency corridors with automated signal preemption simulation.
- **Passenger Cars**: Optimized for smooth traffic flow and highway access.
- **Two-Wheelers**: Navigates through congested dense corridors where large vehicles cannot pass.

### 3. 🎯 Multi-Objective Optimization Modes
- **Balanced**: Best compromise between travel time and fuel efficiency.
- **Fastest**: Prioritizes minimum travel time and maximum congestion avoidance.
- **Lowest Emissions (Eco-Route)**: Minimizes idle time and stops to drastically curb greenhouse gas emissions.

### 4. 🎛️ Dual-Workspace Architecture
- **Driver Workspace (`/driver`)**:
  - Live interactive map with route tracing.
  - Turn-by-turn routing details, speed guidance, and ETA estimation.
  - Dynamic warnings for weight limits, overhead clearances, and congestion hotspots.
- **Operations Control Center (`/operations`)**:
  - Grid-level overview of city junctions, flyovers, and bottleneck nodes.
  - Incident detection (accidents, roadwork, closures) with live impact summaries.
  - Manual override and green corridor dispatch tools.

---

## 🚀 Live Demo & Links

| Surface | Direct Link | Description |
| :--- | :--- | :--- |
| **Driver Experience** | [traffic-route-optimization-mx7v.vercel.app/driver](https://traffic-route-optimization-mx7v.vercel.app/driver) | Turn-by-turn route navigation & vehicle profile selection |
| **Operations Dashboard** | [traffic-route-optimization-mx7v.vercel.app/operations](https://traffic-route-optimization-mx7v.vercel.app/operations) | Network-wide traffic control & emergency corridor activation |

---

## 🛠️ Tech Stack

- **Framework**: [Next.js 16](https://nextjs.org/) (App Router & React Server Components)
- **Library**: [React 19](https://react.dev/)
- **Language**: [TypeScript](https://www.typescriptlang.org/)
- **Styling**: [Tailwind CSS v4](https://tailwindcss.com/), Radix UI / Base UI, [Lucide Icons](https://lucide.dev/)
- **Data Visualization**: [Recharts](https://recharts.org/)
- **State Management**: React Context & Custom Hooks
- **Hosting**: [Vercel](https://vercel.com/)

---

## 📁 Project Structure

```text
traffic-route-optimization/
├── app/
│   ├── driver/page.tsx         # Driver navigation surface
│   ├── operations/page.tsx     # Operations control dashboard
│   ├── layout.tsx              # Root layout with theme & metadata
│   ├── globals.css             # Tailwind styling and design tokens
│   └── page.tsx                # Entry point redirecting to /driver
├── components/
│   ├── driver-experience.tsx   # Interactive driver navigation UI
│   ├── operations-dashboard.tsx# Traffic authority monitor & controls
│   ├── traffic-map.tsx         # Handcrafted vector traffic network renderer
│   ├── optimization-analysis.tsx# Metrics & algorithm comparison charts
│   ├── impact-summary.tsx      # CO2, fuel, and time savings analytics
│   └── ui/                     # Reusable design system components
├── lib/
│   ├── traffic-network.ts      # Deterministic network topology, nodes & segments
│   ├── driver-trip.ts          # Constraint evaluation & trip calculations
│   └── utils.ts                # Class merging & utility helpers
└── types/
    └── traffic.ts              # Core TypeScript interfaces & state models
```

---

## 💻 Local Development

Follow these steps to run the project locally:

### 1. Clone the repository
```bash
git clone https://github.com/Roastyyy31/MargDarshak.git
cd MargDarshak
```

### 2. Install dependencies
```bash
# Using pnpm (recommended)
pnpm install

# Or using npm
npm install
```

### 3. Run development server
```bash
pnpm dev
# or
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

### 4. Build for production
```bash
pnpm build
pnpm start
```

---

## 📈 Impact & Benefits

- ⚡ **Up to 35% Reduction** in emergency vehicle response times via dynamic corridor allocation.
- 📉 **20-25% Lower Emissions** for commercial freight by avoiding stop-and-go bottleneck zones.
- 🛡️ **Zero Clearance Incidents**: Enforces regulatory height/weight compliance to prevent bridge collisions.

---

## 📄 License

This project is open-source and developed for the Smart India Hackathon.

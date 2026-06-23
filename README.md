<![CDATA[<div align="center">

# 🥗 NutriTrack — AI-Powered Fitness & Nutrition Dashboard

**A premium, full-featured nutrition tracking web app with an AI Coach, B2B Coach Dashboard, and beautiful dark glassmorphism UI.**

[![License: MIT](https://img.shields.io/badge/License-MIT-10b981.svg)](LICENSE)
[![Made with JavaScript](https://img.shields.io/badge/Made%20with-JavaScript-f7df1e.svg)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Firebase](https://img.shields.io/badge/Backend-Firebase-ffca28.svg)](https://firebase.google.com/)
[![Gemini AI](https://img.shields.io/badge/AI-Google%20Gemini-4285F4.svg)](https://ai.google.dev/)

---

</div>

## ✨ Features

### 🍽️ Core Nutrition Tracking
- **Calorie & Macro Tracking** — Log meals with real-time calorie ring charts and macro breakdowns (Protein, Carbs, Fat, Fiber)
- **700+ Food Database** — Built-in searchable food database with detailed nutritional data
- **Smart Food Search** — Instant fuzzy search with portion size customization
- **Daily Budget System** — Set personalized calorie and macro goals with visual progress indicators

### 🤖 AI-Powered Features (Google Gemini)
- **AI Nutrition Coach** — Real-time conversational AI chat for diet advice, meal suggestions, and fitness guidance
- **Smart Meal Analysis** — AI analyzes your daily intake and provides actionable insights
- **AI Diet Plan Generator** — Get personalized weekly diet plans based on your goals and preferences
- **Healthier Alternatives** — AI suggests healthier substitutes for any food item

### 📊 Analytics & History
- **7-Day History** — Visual timeline of your nutrition data with interactive charts
- **Trend Analysis** — Track your calorie and macro adherence over time
- **Weekly Meal Planner** — Plan and organize meals for the entire week

### 👨‍💼 B2B Coach Dashboard (Phase 3)
- **Multi-Client Management** — Coaches can manage multiple client profiles
- **Client Nutrition Overview** — View any client's daily intake, macros, and adherence trends
- **Coach Notes System** — Add and track private notes for each client session
- **Adherence Trend Charts** — SVG-based visual charts showing 7-day calorie adherence patterns
- **AI Diet Plans for Clients** — Generate AI-powered diet plans on behalf of clients

### 🔐 Authentication & Data
- **Multi-User Auth** — Email/password login system with secure session management
- **Firebase Firestore** — Cloud database for real-time data sync across devices
- **Offline Mode** — Falls back to localStorage when Firebase is not configured
- **Data Privacy** — Each user's data is isolated and secure

---

## 🖥️ Tech Stack

| Layer | Technology |
|-------|-----------|
| **Frontend** | HTML5, CSS3, Vanilla JavaScript (ES6 Modules) |
| **UI Design** | Custom Glassmorphism Design System, SVG Charts |
| **Fonts** | Google Fonts — Inter (body), Outfit (headings) |
| **Backend** | Firebase Firestore (NoSQL Cloud Database) |
| **Auth** | Firebase Authentication |
| **AI Engine** | Google Gemini 2.0 Flash API |
| **Hosting** | Firebase Hosting |

---

## 📁 Project Structure

```
nutritrack/
├── index.html              # Single-page application (all views)
├── firebase.json           # Firebase Hosting configuration
├── css/
│   └── style.css           # Complete design system (~4000 lines)
└── js/
    ├── app.js              # Main application logic & UI controller
    ├── admin.js            # B2B Coach Dashboard module
    ├── ai.js               # Gemini AI integration & chat engine
    ├── auth.js             # Authentication system
    ├── charts.js           # SVG donut & macro bar chart renderer
    ├── db.js               # Database abstraction (Firebase/localStorage)
    ├── firebase-config.js  # Firebase project credentials
    ├── foodDatabase.js     # 700+ food items nutritional database
    ├── history.js          # 7-day history & analytics
    ├── planner.js          # Weekly meal planner
    ├── tracker.js          # Water & exercise tracker
    └── alternatives.js     # Healthier food alternatives engine
```

---

## 🚀 Getting Started

### Option 1: Run Locally (No Setup Required)

1. **Clone the repository:**
   ```bash
   git clone https://github.com/tyagipuru7/NutriTrack.git
   cd NutriTrack
   ```

2. **Open in browser:**
   Simply open `index.html` in your browser, or use a local server:
   ```bash
   # Using Python
   python -m http.server 8080

   # Using Node.js
   npx serve .
   ```

3. **Start tracking!** The app works immediately in offline/localStorage mode — no Firebase setup needed.

### Option 2: Enable Firebase (Cloud Sync)

1. Create a project at [Firebase Console](https://console.firebase.google.com/)
2. Enable **Authentication** (Email/Password) and **Firestore Database**
3. Copy your config values into `js/firebase-config.js`:
   ```javascript
   export const firebaseConfig = {
     apiKey: "your-api-key",
     authDomain: "your-project.firebaseapp.com",
     projectId: "your-project-id",
     storageBucket: "your-project.firebasestorage.app",
     messagingSenderId: "your-sender-id",
     appId: "your-app-id",
     measurementId: "your-measurement-id"
   };

   export const USE_FIREBASE = true;  // ← Set to true
   ```

### Option 3: Enable AI Features

1. Get a free Gemini API key at [aistudio.google.com/apikey](https://aistudio.google.com/apikey)
2. In the app, go to **Settings → AI Configuration** and paste your key
3. Start chatting with the AI Coach! 🤖

---

## 📸 Screenshots

> _Add your screenshots here after deploying!_
>
> Suggested screenshots:
> - Dashboard with calorie ring
> - AI Chat conversation
> - Coach Dashboard with client list
> - Weekly Meal Planner
> - 7-Day History view

---

## 🎨 Design Philosophy

NutriTrack uses a **custom dark glassmorphism design system** built from scratch with:

- 🌑 Deep dark backgrounds with frosted glass card effects
- 💚 Emerald → Cyan primary gradient accent
- ✨ Subtle glow effects and smooth hover transitions
- 📱 Fully responsive design (mobile-first)
- 🎯 Accessibility-focused contrast ratios
- 📊 Hand-crafted SVG charts (no external chart libraries)

---

## 🤝 Contributing

Contributions are welcome! Feel free to:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- [Google Gemini](https://ai.google.dev/) — AI-powered nutrition coaching
- [Firebase](https://firebase.google.com/) — Backend infrastructure
- [Google Fonts](https://fonts.google.com/) — Inter & Outfit typefaces
- [USDA FoodData Central](https://fdc.nal.usda.gov/) — Nutritional data reference

---

<div align="center">

**Built with ❤️ for fitness enthusiasts and nutrition coaches**

⭐ Star this repo if you found it helpful!

</div>
]]>

# FlavorMind

**FlavorMind** is an AI-powered mobile application designed to help users plan meals, log recipes, track pantry items, and discover personal flavor trends. The app uses Claude 3 or GPT-4 with memory (MCP) to deliver personalized meal recommendations and insightful analysis based on your cooking history and preferences.

---

## MVP Development Roadmap

### MVP 1: Local Mobile Prototype
- Set up the core React Native app using Expo
- Build the following UI screens:
  - Log Meal
  - Meal Plan
  - Pantry
  - Flavor Profile
  - Settings
- Use AsyncStorage for local state management
- Enable manual meal and pantry logging

### MVP 2: Backend Integration
- Create a backend service using FastAPI or Flask
- Design and expose the following API endpoints:
  - `POST /log-meal`
  - `GET /pantry`
  - `POST /update-pantry`
  - `GET /meal-plan`
- Use SQLite (initially) or Supabase (later) for persistent data storage
- Connect the mobile app to the backend using Axios

### MVP 3: AI-Powered Meal Planning
- Integrate Claude 3 or GPT-4 with memory (MCP)
- Structure and store user memory in a consistent format
- Design prompt templates to:
  - Plan weekly meals
  - Recommend dishes based on flavor preferences
  - Surface cooking insights from past logs
- Display AI-generated meal recommendations in the mobile interface

---

## Setup Instructions

### Mobile App (React Native / Expo)
1. Navigate to the mobile project directory:
   ```bash
   cd mobile
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   expo start
   ```

### Backend Server (FastAPI)
1. Navigate to the backend directory:
   ```bash
   cd backend
   ```
2. Install Python dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the API locally:
   ```bash
   uvicorn main:app --reload
   ```

---

## Technology Stack
- **Frontend:** React Native (Expo)
- **Backend:** FastAPI or Flask
- **State Management:** AsyncStorage, Zustand, or Context API
- **Database:** SQLite (local) or Supabase (cloud sync)
- **AI Agent:** Claude 3 or GPT-4 with long-term memory (MCP)

---

## Directory Overview

```
FlavorMind/
├── mobile/                      # React Native app (Expo)
│   ├── App.tsx                  # Root entry point
│   ├── navigation/              # Stack/tab navigation setup
│   ├── screens/                 # UI screens
│   ├── components/              # Reusable components
│   └── utils/                   # Helper functions and API logic
├── backend/                     # FastAPI backend
│   ├── main.py                  # API entry
│   ├── routes/                  # Endpoint logic
│   ├── db/                      # Database models
│   └── ai/                      # Prompt handling and AI logic
└── requirements.txt             # Backend Python dependencies
```

---

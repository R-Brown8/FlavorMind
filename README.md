  # FlavorMind
│
│   **FlavorMind** is an AI-powered mobile application designed to help users plan meals, log recipes, track pantry items, and discover personal flavor trends. The app leverages Claude 3 or GPT-4 with memory capabilities to deliver personalized meal recommendations and reflective culinary insights based on past behavior and preferences.
│
│   ## MVP Development Roadmap
│
│   ### MVP 1: Local Mobile Prototype
│   - Implement core React Native app using Expo
│   - Build basic UI screens: Log Meal, Meal Plan, Pantry, Flavor Profile, Settings
│   - Enable local state management using AsyncStorage
│   - Allow users to manually log meals, ingredients, and pantry status
│
│   ### MVP 2: Backend Integration
│   - Develop FastAPI or Flask-based backend service
│   - Design and expose API endpoints for:
│     - Logging meals
│     - Fetching and updating pantry data
│     - Generating weekly meal plans
│   - Use SQLite or Supabase for persistent storage
│   - Connect mobile app to backend with Axios
│
│   ### MVP 3: AI-Powered Meal Planning
│   - Integrate Claude or GPT-4 APIs with memory (MCP)
│   - Create structured memory format for meals and flavor logs
│   - Design prompt templates to generate personalized plans and flavor analysis
│   - Display AI-generated meal recommendations in the mobile UI
│
│   ## Setup Instructions
│
│   ### Mobile App (React Native / Expo)
│   1. Navigate to the mobile project directory:
│      ```bash
│      cd mobile
│      ```
│   2. Install dependencies:
│      ```bash
│      npm install
│      ```
│   3. Start the development server:
│      ```bash
│      expo start
│      ```
│
│   ### Backend Server (FastAPI)
│   1. Navigate to the backend directory:
│      ```bash
│      cd backend
│      ```
│   2. Install Python dependencies:
│      ```bash
│      pip install -r requirements.txt
│      ```
│   3. Run the API locally:
│      ```bash
│      uvicorn main:app --reload
│      ```
│
│   ## Technology Stack
│   - **Frontend**: React Native, Expo
│   - **Backend**: FastAPI or Flask
│   - **State Management**: AsyncStorage, Context API or Zustand
│   - **Database**: SQLite (local), Supabase (cloud sync)
│   - **AI Agent**: Claude 3 or GPT-4 with memory (MCP)
│
│   ## Directory Overview
│   Refer to the directory structure outlined above for file/module organization.

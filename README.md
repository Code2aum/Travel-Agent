# Travel Agent (Code will be updated shortly)

A modern travel planning assistant that helps users plan their trips using AI-powered agents. The application features a real-time chat interface for natural conversation and intelligent trip planning.
## Demo Video
Please view the demo here: https://sites.google.com/ds.study.iitm.ac.in/harshithravikopparam/home
## Features

- 🤖 AI-powered travel planning
- 💬 Real-time chat interface
- 🔍 Smart search capabilities
- 📱 Responsive web interface
- 🔄 WebSocket-based real-time communication
- 🎯 Trip planning with location, dates, and budget consideration

## Tech Stack

### Frontend
- React Native with Expo
- TypeScript
- NativeWind (Tailwind CSS for React Native)
- Redux Toolkit for state management
- WebSocket for real-time communication

### Backend
- FastAPI
- WebSocket support
- Redis for session management
- Autogen for AI agent orchestration
- Ollama for LLM integration

## Prerequisites

- Python 3.13+
- Node.js 18+
- npm or yarn
- Redis server
- Ollama (for LLM support)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/Travel-Agent-Omega.git
cd Travel-Agent-Omega
```

2. Set up the backend:
```bash
cd backend
python -m venv venv
source venv/bin/activate  # On Windows: .\venv\Scripts\activate
pip install -r requirements.txt
```

3. Set up the frontend:
```bash
cd frontend
npm install
```

## Configuration

1. Backend Configuration:
   - Ensure Redis server is running
   - Set up environment variables in `.env` file (if needed)
   - Configure Ollama model settings in `AutogenMagneticOne/main.py`

2. Frontend Configuration:
   - Update API endpoints in configuration files if needed
   - Configure environment variables if required

## Running the Application

1. Start the backend server:
```bash
cd backend
PYTHONPATH=$PYTHONPATH:. uvicorn FastAPI.main:app --reload
```

2. Start the frontend development server:
```bash
cd frontend
npm start
```

3. Access the application:
   - Web: http://localhost:8081
   - Mobile: Scan QR code with Expo Go app

## Development

### Project Structure
```
Travel-Agent-Omega/
├── backend/
│   ├── FastAPI/
│   │   ├── apis/
│   │   ├── models/
│   │   └── services/
│   ├── AutogenMagneticOne/
│   │   └── agents/
│   └── RedisSetup/
├── frontend/
│   ├── app/
│   │   ├── components/
│   │   └── store/
│   └── scripts/
└── docs/
```

### Available Scripts

- `npm start`: Start the frontend development server
- `npm run android`: Run on Android device/emulator
- `npm run ios`: Run on iOS simulator
- `npm run web`: Run in web browser
- `npm run test`: Run tests
- `npm run lint`: Run linter

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Autogen for AI agent framework
- Ollama for LLM support
- FastAPI for backend framework
- React Native and Expo for frontend framework

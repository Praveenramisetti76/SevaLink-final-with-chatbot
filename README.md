#  SevaLink - All-in-One Community Citizen Service Portal

##  Features :

### Service Request & Complaint Management
- Report civic issues (street lights, garbage, water problems)
- Real-time status tracking (Pending → In Progress → Resolved)
- Location-based categorization

###  Blood Donation Network
- Emergency blood requests with urgency levels
- Volunteer notification system
- Real-time matching and updates

###  Elderly People Support
- Transport, food, and medical assistance requests
- Community volunteer network
- Priority-based assignment

###  Intelligent Chatbot
- **Multi-language support**: Hindi, English, Telugu
- **Voice + Text input** with Web Speech API
- **AI-powered intent detection** using Gemini Pro
- **Automatic request logging** to database

##  Tech Stack

- **Frontend**: React 18 + Tailwind CSS + Framer Motion
- **Backend**: Node.js + Express.js
- **Database**: MongoDB Atlas
- **Authentication**: JWT tokens
- **AI/NLP**: Gemini Pro API + HuggingFace
- **Real-time**: Socket.io
- **Voice**: Web Speech API + Whisper

##  Project Structure

```
sevalink/
├── client/                 # React frontend
│   ├── src/
│   │   ├── components/     # Reusable components
│   │   ├── pages/         # Page components
│   │   ├── hooks/         # Custom hooks
│   │   ├── utils/         # Utility functions
│   │   └── styles/        # Global styles
├── server/                # Node.js backend
│   ├── models/           # MongoDB schemas
│   ├── routes/           # API routes
│   ├── middleware/       # Custom middleware
│   ├── controllers/      # Route controllers
│   └── utils/           # Server utilities
└── docs/                # Documentation
```

##  Quick Start

### Prerequisites
- Node.js 18+
- MongoDB Atlas account
- Gemini Pro API key

### Installation

1. **Clone and install dependencies**
```bash
git clone <repository-url>
cd sevalink
npm run install-all
```

2. **Environment Setup**
```bash
cd server
cp .env.example .env
# Edit .env with your configuration
```

3. **Start Development**
```bash
npm run dev
```

- Frontend: http://localhost:3000
- Backend: http://localhost:5000

##  User Roles

###  Citizen/User
- Raise service requests via chatbot or forms
- Track complaint status
- Receive updates and notifications

###  Volunteer
- Accept blood donation requests
- Provide elderly support services
- Manage availability status

##  API Endpoints

### Authentication
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `GET /api/auth/profile` - Get user profile

### Services
- `POST /api/complaints` - Create complaint
- `GET /api/complaints` - Get complaints
- `POST /api/blood-requests` - Create blood request
- `POST /api/elderly-support` - Create support request

### Chatbot
- `POST /api/chatbot/message` - Process chatbot message
- `POST /api/chatbot/voice` - Process voice input

## Configuration

### MongoDB Setup
1. Create MongoDB Atlas cluster
2. Get connection string
3. Add to `.env` file

### Gemini API Setup
1. Get API key from Google AI Studio
2. Add to `.env` file

## Mobile Responsive
Fully responsive design optimized for:
- Desktop (1920px+)
- Tablet (768px - 1024px)
- Mobile (320px - 767px)

##  Design System
- **Primary Colors**: Blue gradient theme
- **Typography**: Inter + Poppins fonts
- **Components**: Consistent design language
- **Animations**: Smooth transitions with Framer Motion

## Deployment

### Local Development
```bash
npm run dev
```

### Production Build
```bash
npm run build
npm start
```
## Built at CodeSpark'2025 KBN Collage Of Engineering




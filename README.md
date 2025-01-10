# Spamurai: AI-Powered Gmail Protection

Spamurai is a sophisticated email protection system that enhances Gmail's native spam filtering capabilities through AI-powered analysis, providing real-time threat assessment and detailed analytics via a sleek Chrome extension.

Visit our website: [spamurai.online](https://spamurai.online)

## Core Technologies

### AI Model ([Separate Repository](link-to-ai-repo))
- LSTM-based classification model trained on ~5,000 labeled emails
- Built with TensorFlow/Keras
- Achieves high accuracy in spam detection
- Trained on balanced dataset from Kaggle
- Handles text preprocessing and classification
- Integrated with main application via FastAPI endpoint

### Frontend (Chrome Extension)
- Built with React 18 + Vite
- Styled using Tailwind CSS
- Key Components:
  - Real-time analysis display
  - Interactive dashboard
  - Spam history visualization (Recharts)
  - Custom progress indicators
  - Tab-based interface (Radix UI)
  - Smooth animations (Framer Motion)

### Backend Infrastructure
- FastAPI application server
- PostgreSQL database (AWS RDS)
- Features:
  - Real-time email analysis
  - OAuth 2.0 authentication
  - Spam statistics tracking
  - Email authentication verification (SPF/DKIM)

### AWS Infrastructure
- Hosted on EC2 instances
- Route 53 DNS Management:
  - Manages domain routing
  - Handles health checks
  - Automated domain management
- RDS (Relational Database Service):
  - Managed PostgreSQL instance
  - Automated backups
  - High availability
  - Scalable performance
- SSL/TLS Encryption:
  - Secure data transmission
  - HTTPS enforcement
  - Server identity verification

### Security
- Google OAuth 2.0 authentication
- Token-based authorization
- SSL/TLS encryption for all communications
- No storage of email content
- Secure credential management

## API Endpoints

```plaintext
GET  /api/health          - Service health check
GET  /api/db_health      - Database connection check
POST /api/predict        - Email analysis
GET  /api/spam-stats     - User spam statistics
```

## Database Schema

The system uses PostgreSQL with three main tables:
- Users: Stores user identification and preferences
- Messages: Maintains analysis results and message metadata
- DailySpamStats: Tracks spam statistics over time

## Installation

### Extension Setup
1. Clone the repository
2. Install dependencies: `npm install`
3. Set up OAuth credentials:
   - Create Google Cloud project
   - Enable Gmail API
   - Configure OAuth consent
   - Create OAuth 2.0 Client ID
4. Configure manifest.json
5. Build: `npm run build`
6. Load in Chrome

### Backend Setup
1. Clone the repository
2. Install requirements: `pip install -r requirements.txt`
3. Configure environment variables
4. Set up PostgreSQL database
5. Run server: `uvicorn main:app --reload`

## Contributing

We welcome contributions! Please read our contributing guidelines and submit pull requests for any enhancements.

## License

[Add your license information here]

## Acknowledgments

- Gmail API
- Google OAuth 2.0
- FastAPI
- React
- Tailwind CSS
- AWS Services

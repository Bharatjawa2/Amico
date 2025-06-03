# Mini CRM Platform

A modern CRM platform that enables customer segmentation, personalized campaign delivery, and intelligent insights.

## Features

- 🔐 Secure REST APIs for data ingestion
- 🎯 Advanced customer segmentation with flexible rule logic
- 📊 Campaign management and delivery tracking
- 🤖 AI-powered features for enhanced insights
- 🔑 Google OAuth 2.0 authentication
- 📈 Real-time campaign analytics

## Tech Stack

### Backend
- FastAPI (Python)
- PostgreSQL
- Redis (Message Broker)
- Celery (Async Task Queue)
- OpenAI API (AI Features)

### Frontend
- React
- TypeScript
- Material-UI
- Redux Toolkit

## Setup Instructions

### Backend Setup

1. Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

2. Install dependencies:
```bash
cd Backend
pip install -r requirements.txt
```

3. Set up environment variables:
```bash
cp .env.example .env
# Edit .env with your configuration
```

4. Run database migrations:
```bash
alembic upgrade head
```

5. Start the backend server:
```bash
uvicorn app.main:app --reload
```

### Frontend Setup

1. Install dependencies:
```bash
cd Frontend
npm install
```

2. Start the development server:
```bash
npm start
```

## API Documentation

Once the backend is running, visit:
- Swagger UI: http://localhost:8000/docs
- ReDoc: http://localhost:8000/redoc

## Project Structure

```
├── Backend/
│   ├── app/
│   │   ├── api/
│   │   ├── core/
│   │   ├── models/
│   │   ├── schemas/
│   │   └── services/
│   ├── tests/
│   └── alembic/
├── Frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   └── store/
│   └── public/
└── README.md
```

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

MIT

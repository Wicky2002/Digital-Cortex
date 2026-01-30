# Development Guide

## Prerequisites

- Node.js 18+
- Python 3.10+
- PostgreSQL 14+
- Redis 6+
- Git

## Initial Setup

### 1. Clone Repository
```bash
git clone https://github.com/YourUsername/Digital-Cortex.git
cd Digital-Cortex
```

### 2. Environment Configuration
```bash
cp .env.example .env
# Edit .env with your configuration
```

### 3. Install Dependencies

**Frontend:**
```bash
cd frontend
npm install
```

**Backend:**
```bash
cd backend
npm install
```

**AI Service:**
```bash
cd ai-service
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
pip install -r requirements.txt
```

### 4. Database Setup
```bash
# Create database
createdb digital_cortex

# Run migrations
cd backend
npm run migrate
```

### 5. Start Services

**Option 1: Individual Services**
```bash
# Terminal 1 - Frontend
cd frontend
npm start

# Terminal 2 - Backend
cd backend
npm run dev

# Terminal 3 - AI Service
cd ai-service
python -m uvicorn app.main:app --reload

# Terminal 4 - Redis
redis-server
```

**Option 2: Docker Compose**
```bash
docker-compose up
```

## Development Workflow

### Branch Strategy
- `main` - Production-ready code
- `develop` - Development branch
- `feature/*` - Feature branches
- `bugfix/*` - Bug fix branches
- `hotfix/*` - Hotfix branches

### Creating a Feature
```bash
git checkout develop
git pull origin develop
git checkout -b feature/your-feature-name

# Make changes
git add .
git commit -m "feat: your feature description"
git push origin feature/your-feature-name

# Create pull request
```

### Code Style

**Frontend (TypeScript):**
```bash
npm run lint
npm run format
```

**Backend (JavaScript):**
```bash
npm run lint
npm run format
```

**AI Service (Python):**
```bash
black .
flake8 .
mypy .
```

### Testing

**Frontend:**
```bash
npm test                 # Run tests
npm run test:coverage   # With coverage
```

**Backend:**
```bash
npm test                 # Run tests
npm run test:integration # Integration tests
```

**AI Service:**
```bash
pytest                   # Run tests
pytest --cov            # With coverage
```

## Debugging

### Frontend
- Use React DevTools
- Chrome DevTools
- VSCode debugger config provided

### Backend
- Use VSCode debugger
- Node Inspector
- Console logging

### AI Service
- Python debugger (pdb)
- VSCode Python debugger
- Logging

## Common Tasks

### Adding a New API Endpoint
1. Create route in `backend/src/routes/`
2. Add controller in `backend/src/controllers/`
3. Update service in `backend/src/services/`
4. Add tests

### Adding a New React Component
1. Create component in `frontend/src/components/`
2. Add types in `frontend/src/types/`
3. Write tests
4. Update Storybook (if applicable)

### Adding AI Functionality
1. Create service in `ai-service/app/services/`
2. Add API endpoint in `ai-service/app/api/`
3. Update models if needed
4. Add tests

## Troubleshooting

### Port Already in Use
```bash
# Find process using port
lsof -i :3000  # Mac/Linux
netstat -ano | findstr :3000  # Windows

# Kill process
kill -9 <PID>
```

### Database Connection Issues
```bash
# Check PostgreSQL is running
pg_isready

# Check connection string in .env
# Verify database exists
psql -l
```

### Module Not Found
```bash
# Clear cache and reinstall
rm -rf node_modules package-lock.json
npm install
```

## Best Practices

1. **Code Review**: All changes require review
2. **Testing**: Maintain 80%+ coverage
3. **Documentation**: Update docs with code
4. **Commits**: Use conventional commits
5. **Security**: Never commit secrets
6. **Performance**: Profile before optimizing

## Resources

- [React Documentation](https://react.dev)
- [Node.js Documentation](https://nodejs.org)
- [Python Documentation](https://docs.python.org)
- [PostgreSQL Documentation](https://www.postgresql.org/docs/)

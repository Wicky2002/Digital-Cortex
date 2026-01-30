# Backend API

Node.js/Express backend API for Digital Cortex.

## Setup

```bash
npm install
npm run dev
```

## Structure

```
backend/
├── src/
│   ├── controllers/    # Request handlers
│   ├── models/         # Database models
│   ├── routes/         # API routes
│   ├── middleware/     # Custom middleware
│   ├── services/       # Business logic
│   ├── utils/          # Utility functions
│   └── config/         # Configuration
├── tests/              # Test files
└── package.json
```

## Technology Stack

- Node.js
- Express
- GraphQL
- PostgreSQL (with Sequelize ORM)
- Redis
- JWT Authentication

## API Endpoints

### Authentication
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - User login
- `POST /api/auth/refresh` - Refresh token

### Knowledge
- `GET /api/knowledge` - List knowledge items
- `POST /api/knowledge` - Create knowledge item
- `PUT /api/knowledge/:id` - Update knowledge item
- `DELETE /api/knowledge/:id` - Delete knowledge item
- `GET /api/knowledge/search` - Search knowledge

### Graph
- `GET /api/graph` - Get knowledge graph
- `POST /api/graph/connections` - Create connections

## Development

```bash
npm run dev      # Start development server
npm run build    # Build for production
npm run test     # Run tests
npm run migrate  # Run database migrations
```

# Test Suite

## Running Tests

### All Tests
```bash
npm run test:all
```

### Frontend Tests
```bash
cd frontend
npm test
```

### Backend Tests
```bash
cd backend
npm test
```

### AI Service Tests
```bash
cd ai-service
pytest
```

## Test Structure

```
tests/
├── unit/              # Unit tests
├── integration/       # Integration tests
├── e2e/              # End-to-end tests
└── fixtures/         # Test data
```

## Writing Tests

Follow the testing best practices outlined in the documentation.

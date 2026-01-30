# Documentation

Comprehensive documentation for Digital Cortex.

## Contents

- [Architecture](architecture.md) - System architecture overview
- [API Documentation](api.md) - API reference and examples
- [Development Guide](development.md) - Setup and development workflow
- [Deployment Guide](deployment.md) - Deployment instructions
- [User Guide](user-guide.md) - End-user documentation
- [Security](security.md) - Security best practices

## Quick Links

- [Getting Started](../README.md#getting-started)
- [Contributing](../CONTRIBUTING.md)
- [API Endpoints](api.md)
- [Troubleshooting](troubleshooting.md)

## Overview

Digital Cortex is an AI-powered knowledge management system that combines:
- Intelligent organization using NLP
- Semantic search capabilities
- Knowledge graph visualization
- AI-powered assistant

## Architecture Diagram

```
┌─────────────┐
│   Frontend  │ (React + TypeScript)
└──────┬──────┘
       │
       ▼
┌─────────────┐
│  API Layer  │ (Node.js + GraphQL)
└──────┬──────┘
       │
       ├──────────────┐
       │              │
       ▼              ▼
┌────────────┐  ┌──────────┐
│ AI Service │  │ Database │
│  (Python)  │  │(Postgres)│
└────────────┘  └──────────┘
```

## Support

For questions and support:
- GitHub Issues
- GitHub Discussions
- Documentation

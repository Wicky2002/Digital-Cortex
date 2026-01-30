# Build and Deployment Scripts

## Available Scripts

### Build
```bash
./scripts/build.sh          # Build all services
./scripts/build-frontend.sh # Build frontend only
./scripts/build-backend.sh  # Build backend only
```

### Deploy
```bash
./scripts/deploy.sh         # Deploy to production
./scripts/deploy-staging.sh # Deploy to staging
```

### Database
```bash
./scripts/db-migrate.sh     # Run migrations
./scripts/db-seed.sh        # Seed database
./scripts/db-backup.sh      # Backup database
```

### Docker
```bash
./scripts/docker-build.sh   # Build Docker images
./scripts/docker-push.sh    # Push to registry
```

## Usage

All scripts should be run from the project root directory.

```bash
cd Digital-Cortex
./scripts/build.sh
```

# Todo Application

Mock todo application for CloudBees Unify RO adoption journey demo.

## Overview
This application orchestrates the deployment of multiple components:
- Database component (component-db)
- Web component (component-web)

## Architecture
```
todo-app
├── component-db (database)
└── component-web (web application)
```

## Deployment Order
1. Database component must deploy first
2. Web component deploys after database is ready

## Deployment
```bash
./deploy.sh
```

## Environment Variables
- `VERSION`: Application version (default: 1.0.0)
- `ENVIRONMENT`: Target environment (default: dev)

## CloudBees Unify RO Integration
This application demonstrates release orchestration capabilities:
- Component dependency management
- Ordered deployment workflow
- Version coordination across components
- Environment promotion strategies

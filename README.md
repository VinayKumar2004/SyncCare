# SyncCare

SyncCare is a low-bandwidth collaborative reminder, communication, and synchronized media companion system.

## Repository Layout

- `backend/` - Spring Boot 3 + Java 17 backend baseline (security-first, REST/WebSocket ready)
- `frontend/` - React Native TypeScript architecture scaffold for local-first mobile features

## Current Bootstrap Status

### Backend (implemented)

- Spring Boot 3.5 baseline with layered package starter structure
- Security baseline (`SecurityFilterChain`, BCrypt encoder)
- Standardized API response wrapper (`ApiResponse`)
- Global exception handling scaffold (`GlobalExceptionHandler`)
- Health endpoint: `GET /api/v1/health`
- Actuator health exposed
- Smoke tests for endpoint and startup behavior

### Frontend (implemented)

- TypeScript-first module structure for clean architecture setup
- Feature and shared layer folders for scalable React Native development
- Path aliases for maintainable imports

## Run Backend Locally

```bash
cd backend
mvn spring-boot:run
```

## Run Backend Tests

```bash
cd backend
mvn test
```

## Next Iteration Targets

1. JWT auth + refresh token rotation
2. Pairing workflow APIs and DTOs
3. Reminder entity + local-first sync event schema
4. MQTT/WebSocket event transport and retry metadata APIs
5. React Native app bootstrap with navigation/state/store and local DB adapters

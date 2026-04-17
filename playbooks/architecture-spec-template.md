# Architecture Spec Template

Use this template as input to architecture diagram generation.

## 1. Project Identity

- Project name:
- Repository:
- Primary objective:
- Runtime environments (dev/stage/prod):

## 2. System Boundary

- What is inside this system:
- What is external:

## 3. Clients and Entry Points

- Web/mobile/CLI clients:
- API gateways/ingress:
- Auth entry points:

## 4. Core Services

- Service name:
- Responsibility:
- Language/runtime:
- Depends on:

## 5. Data Layer

- Databases:
- Caches:
- Object storage:
- Vector/graph stores:

## 6. Async and Eventing

- Queues/streams:
- Producers:
- Consumers:

## 7. External Integrations

- Third-party APIs:
- Blockchain/RPC providers:
- Identity/payment/notification services:

## 8. Security and Trust Boundaries

- AuthN/AuthZ model:
- Secret management:
- Network boundaries:

## 9. Observability and Operations

- Logging:
- Metrics:
- Alerting:
- CI/CD:

## 10. Critical Flows

- Flow A (user request path):
- Flow B (async/background path):
- Flow C (failure/retry path):

## 11. Diagram Prompt Block

Paste a concise architecture list for diagram generation:

- Component A -> Component B (protocol)
- Component B -> Database C (read/write)
- Worker D <- Queue E (consume)

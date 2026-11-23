# Production Setup

## Current status

The repository is a static front-end preview. It does not include production authentication, message delivery, user directory, database, media storage, push notifications, calling infrastructure, or compiled mobile-store applications. The visible call controls are not connected to a call service.

## Required services

Provision company-owned accounts and environments for:

- API and authenticated WebSocket service
- Relational database, migrations, backups, and disaster recovery
- Private object storage and malware scanning for uploads
- Push notification provider and secure token storage
- WebRTC signaling and TURN service for audio/video calls
- Monitoring, abuse prevention, support, and audit logging

## Secure configuration

Use `.env.example` as a list of configuration names only. Put real values in a deployment secret manager; never commit them to Git. Replace example domains before deployment.

## Release checklist

1. Select the backend, hosting region, identity provider, and data-retention policy.
2. Implement account creation, verification, recovery, contacts, conversations, durable message delivery, offline synchronization, and block/report controls.
3. Implement and independently review encryption and key management; do not claim security properties until verified.
4. Add authenticated media upload/download and push notifications.
5. Integrate and test WebRTC, signaling, TURN, device permissions, network changes, and call termination.
6. Complete privacy, accessibility, localization, and security reviews.
7. Build and test Android/iOS applications, create signing keys in company-controlled accounts, and follow each store's submission process.
8. Deploy gradually with monitoring and tested rollback procedures.

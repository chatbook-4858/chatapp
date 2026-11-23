# ChatApp — GMC Pvt LTD

A private, responsive messaging application created for **GMC Pvt LTD**.

## Included in this repository

- Responsive ChatApp web/PWA interface with original GMC branding and logo
- Chat list, search, message composer, sample conversation, and call interface
- Installable-app manifest and offline application shell
- Product, deployment, security, and ownership documentation
- Environment-variable template (contains no real credentials)

## Run the preview

From the repository root, run:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080`. Use HTTPS for installation and browser device APIs on a deployed site.

## Important production status

This repository provides a working **front-end preview**, not a production messaging service. Messages are not delivered to other users, and the call interface is a visual demo; it does not connect calls. There is no live authentication, server, database, push service, media storage, or deployed mobile-store package yet. Production deployment requires GMC Pvt LTD's backend, infrastructure, legal/privacy review, and organization-owned signing and service credentials. See [production setup](docs/SETUP.md).

## Ownership and credentials

This project is marked as proprietary software for GMC Pvt LTD. See [OWNERSHIP.md](OWNERSHIP.md) and [LICENSE](LICENSE). No production keys are included; do not commit secrets. The repository and deployment accounts should be controlled by GMC Pvt LTD.

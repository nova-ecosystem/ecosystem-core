# Welcome to the Nova Ecosystem Core

This is the "heart" of the Nova Ecosystem. It's a monorepo containing the four central services that power the entire platform.

* **`/api`**: The central **API Gateway** (REST/JSON) that acts as the single "front door" for all services.
* **`/app`**: The "Mission Control" **Dashboard** (`app.nova-ecosystem.org`) for user profiles and high-level ecosystem management.
* **`/auth`**: The central **Identity Service** (SSO, KYC, OAuth2) that all pillars consume.
* **`/website`**: The main Docusaurus site (`nova-ecosystem.org`) and high-level documentation.

## 🚀 Getting Started (Local Development)

This repository is configured to use **DevContainers** for a one-click setup.

1.  Make sure you have [Docker Desktop](https://www.docker.com/products/docker-desktop/) installed and running.
2.  Install the [Dev Containers extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) in VS Code.
3.  Clone this repository: `git clone https://github.com/nova-ecosystem/ecosystem-core.git`
4.  Open the cloned folder in VS Code.
5.  A pop-up will appear: "Folder contains a Dev Container... Reopen in Container?". Click **"Reopen in Container"**.

This will build the Docker-Compose environment defined in `.devcontainer/` and launch all four core services.

## 🏃 Running Tests

* **To run unit tests:** Go into the specific service directory (e.g., `cd api`) and run the local test command (e.g., `npm test` or `pytest`).
* **To run integration tests:** Go to the top-level `/tests` directory (e.g., `cd tests/integration`) and run the integration test suite.
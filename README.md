# Node Session Guardian & Uptime Monitor

An open-source, lightweight Node.js automation utility designed for community server administrators. It maintains active server sessions, prevents idle timeouts via intelligent leave/rejoin cycles, and records real-time connection health logs.

## Why Humans Need This
Managing community game servers requires constant uptime verification and session persistence. Instead of manually monitoring server availability or keeping heavy game clients open 24/7, administrators can run this low-memory CLI tool in the background to automate connection recovery and track server stability.

## Key Features
* **Automated Session Recovery (`leaveRejoin.js`):** Automatically handles connection drops, scheduled reconnect cycles, and timeout prevention.
* **Structured Event Logging (`logger.js`):** Captures connection states, timestamps, errors, and session activity for easy debugging.
* **Centralized Configuration (`settings.json`):** Customize host endpoints, reconnect intervals, and bot behavior without touching the core code.
* **Multi-Account Support (`launcher_accounts.json`):** Manage authentication profiles cleanly in a dedicated JSON structure.
* **Automated Dependency Security (`dependabot.yml`):** Pre-configured with GitHub Dependabot to keep Node.js packages secure and up to date.

## Project Structure
* `index.js` — Main application entry point and connection initializer
* `leaveRejoin.js` — Heartbeat and automated leave/rejoin cycle logic
* `logger.js` — Console and file logging utility
* `settings.json` — Server target and timing configuration
* `launcher_accounts.json` — Account credential storage template
* `package.json` — Node.js dependencies and startup scripts

## Quick Start

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/YOUR_USERNAME/node-session-guardian.git](https://github.com/YOUR_USERNAME/node-session-guardian.git)
   cd node-session-guardian

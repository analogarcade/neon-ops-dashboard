# NEON OPS

A compact, single-page cyberpunk operations dashboard with a futuristic terminal/HUD aesthetic. Built as a standalone browser experience with no frameworks, build step, or external dependencies.

![Status](https://img.shields.io/badge/status-operational-39ff88?style=flat-square)
![Stack](https://img.shields.io/badge/stack-HTML%20%2F%20CSS%20%2F%20JS-18f6c5?style=flat-square)

## Overview

NEON OPS combines a weather feed, signal-news panel, live simulated system statistics, alert timeline, and a terminal-style command interface into one responsive viewport.

The interface is intentionally self-contained: the current weather, headlines, statistics, and alert events are simulated in the browser. Clear labels mark the places where real API integrations could be connected.

## Features

- Dark terminal/HUD design with neon teal and green accents
- CSS scanlines, grid background, glow effects, and corner highlights
- Real-time clock and animated status indicators
- Simulated weather card with a CSS-only animated cloud/rain icon
- Refreshable signal-news feed with loading state
- Live-updating CPU, memory, and network values
- Canvas sparklines for system activity
- Auto-appending alerts every 10 seconds, with a clear action
- Ops-console terminal with command history, Tab completion, run-state feedback, and framed results
- Built-in HUD palettes: neon and ember
- Responsive single-viewport layout for desktop and small mobile screens

## Quick Start

Clone the repository:

```bash
git clone https://github.com/analogarcade/neon-ops-dashboard.git
cd neon-ops-dashboard
```

Open `index.html` directly in a browser:

```bash
start index.html
```

Or, in Git Bash on Windows:

```bash
explorer.exe index.html
```

No installation is required.

## Terminal Commands

| Command | Result |
| --- | --- |
| `help` | Shows formatted command usage and examples. |
| `weather` | Displays the simulated weather-feed response. |
| `news` | Describes the simulated headline feed. |
| `status` | Shows the current operational status. |
| `clear` | Clears the terminal log. |
| `history` | Prints commands entered during the current browser session. |
| `theme [neon\|ember]` | Switches the HUD palette; `theme` by itself toggles it. |

### Console Controls

- Press <kbd>↑</kbd> / <kbd>↓</kbd> to browse command history.
- Press <kbd>Tab</kbd> to complete a command. Repeated presses cycle matching commands.
- Each command starts with a RUN indicator and resolves to a consistently framed SUCCESS or ERROR entry.

## Connecting Real Data

The dashboard currently uses client-side simulation. To connect real sources, replace the relevant JavaScript data/update functions in `index.html`:

- Replace the `news` array and refresh handler with a news API request.
- Replace the weather values with a weather API request.
- Replace the simulated stat updates with telemetry from your own backend.

Avoid exposing private API keys in browser-side JavaScript. Use a backend or serverless endpoint to hold secrets and proxy external API requests.

## Project Structure

```text
neon-ops-dashboard/
├── index.html     # Complete dashboard: markup, styles, and interactions
└── README.md      # Project documentation
```

## License

This project is available for personal and educational use. Add a formal license file if you plan to distribute or accept contributions.

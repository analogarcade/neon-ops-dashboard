# ZION OPERATOR TERMINAL

A standalone Matrix-inspired operator console rendered entirely with HTML5, CSS3, and modern vanilla JavaScript. The experience uses a procedural digital-rain canvas, CRT HUD overlays, local archive storage, and a strict terminal command deck.

## Quick start

Open [`index.html`](./index.html) directly in a modern browser. No installation, build step, framework, CDN, font, image, or external asset is required.

## Interface modules

- **System Core:** real-time clock, construct connection addresses, signal tracing gauge, and EMP threat alert state.
- **Signal Intercept:** live decoded packet ticker with automatic four-second pulses.
- **Archive Node:** encrypted-notebook style title/body form backed by browser `localStorage` and an expandable data-tree log.
- **Terminal Deck:** interactive shell with command framing, history navigation, and page-scroll-safe keyboard capture.

## Terminal codes

| Code | Function |
| --- | --- |
| `help` | List available operational codes and parameters. |
| `probe` | Run a one-second visual glitch and simulated proxy-hop trace. |
| `decode` | Change the digital rain to binary streams for five seconds. |
| `manifest` | Print all notes stored in the active browser archive. |
| `purge` | Safely remove the local archive database. |
| `system` | Animate a system diagnostic and operational status report. |

Press `Enter` to execute a command. `ArrowUp` and `ArrowDown` browse commands entered during the current browser session.

## Data and privacy

Archive notes are stored only in the browser’s local storage under the `zion-archive` key. The app makes no network requests and does not transmit note content.

## Integration points

The weather-style telemetry, packet stream, proxy hops, and diagnostics are intentionally simulated. Replace the corresponding JavaScript generators with backend or API integrations if this becomes a real operations console.

## Project structure

```text
neon-ops-dashboard/
├── index.html   # Complete standalone experience
└── README.md    # Project documentation
```

## License

Available for personal and educational use. Add a formal license before distributing it as an open-source project.

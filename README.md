# Server Status

A simple, clean website that displays the real-time status of a Minecraft server.

## Features

- Real-time server status (Online/Offline)
- Server icon display
- Message of the Day (MOTD)
- Player count and max players
- List of online players with avatars
- Auto-refresh every 30 seconds
- Manual refresh button
- Dark theme with Minecraft-inspired styling
- Responsive design for mobile devices

## Server

**IP:** gnugg.servebeer.com:25565

## How to Use

### Option 1: Open Directly
Simply double-click `index.html` to open it in your default web browser.

### Option 2: Local Server
For the best experience, serve the file using a local HTTP server:

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (with http-server installed)
npx http-server

# Using PHP
php -S localhost:8000
```

Then open `http://localhost:8000` in your browser.

### Option 3: Web Hosting
Upload `index.html` to any static web hosting service:
- GitHub Pages
- Netlify
- Vercel
- Any web server with static file hosting

## API

This project uses the free [mcsrvstat.us](https://mcsrvstat.us/) API to fetch server status.

- Status API: `https://api.mcsrvstat.us/3/{server_address}`
- Icon API: `https://api.mcsrvstat.us/icon/{server_address}`

## Customization

To monitor a different server, edit the `SERVER_ADDRESS` variable in the JavaScript section of `index.html`:

```javascript
const SERVER_ADDRESS = 'your.server.address:port';
```

## Browser Support

Works in all modern browsers (Chrome, Firefox, Safari, Edge).

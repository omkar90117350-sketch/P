# PMPML Transit Assistant (Demo)
Voice + text transit assistant for blind/low-vision PMPML riders. Single file: `index.html` (no build step).

- Run locally: open `index.html` in Chrome or Edge (voice input needs internet).
- Deploy on Vercel: `npm i -g vercel && vercel --prod` in this folder (Framework: Other, no build command, output = root), or drag the folder into vercel.com/new. HTTPS is required for microphone access (Vercel provides it).
- Data is SIMULATED. To use real data, implement `TransitProvider` (getStops / getArrivals / getRouteStops) for PMPML/ITMS/GTFS-realtime and replace `new DemoTransitProvider()`.
- Browser screen-reader support is generally less reliable than native TalkBack.

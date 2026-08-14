DRAGONFLY EMBROIDERY CALCULATOR V2

Modes
-----
BASIC:
Time = stitches / machine speed
Stitch cost = stitches / 10,000 × rate
Final = stitch cost + setup fee

BUSINESS:
Base time = stitches / speed
Color-change time = color changes × seconds per color change
Trim/stop time = trims/jumps × seconds per trim/stop
Buffered production time = (base + color-change time + trim/stop time) × (1 + buffer%)
Stitch cost = stitches / 10,000 × rate
Cost = stitch cost + setup + garment/material + other cost
Selling price = cost / (1 - profit margin%)
Profit = selling price - cost

The business model intentionally separates machine production time from stitch-only time.
Tune the seconds per color change and trim/stop using your real machine observations.

ANDROID / LOCAL HOST
--------------------
Option A - easiest:
1. Extract this ZIP on a Windows PC/laptop.
2. Open Command Prompt in the extracted folder.
3. Run:
   python -m http.server 8000 --bind 0.0.0.0
4. Find the PC's local IPv4 address using:
   ipconfig
5. On the Android phone/tablet connected to the SAME Wi-Fi, open:
   http://YOUR-PC-IP:8000
6. For a simple shortcut, Chrome > ⋮ > Add to Home screen > Create shortcut.
7. For a true installable PWA, use HTTPS hosting (see README instructions in the previous version). localhost/file:// and plain LAN HTTP are useful for testing but are not the normal secure PWA installation environment.

Option B - publish it:
Upload the folder to an HTTPS static host. Open the HTTPS URL in Chrome Android and use:
⋮ > Add to Home screen > Install app
or the browser's Install option if shown.

No server/database is required. All calculations and saved settings are local in the browser.

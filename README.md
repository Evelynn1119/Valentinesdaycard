Be My Valentine? 💌
An interactive Valentine's Day card with a twist — the "No" button runs away from your cursor so it literally cannot be clicked. Built entirely in vanilla HTML, CSS, and JavaScript with no frameworks or dependencies.
Made with love by @evelynn.creates_

✨ Features
Envelope Opening Experience

Animated envelope with a 3D flap that opens on tap or click
Heart wax seal that fades as the envelope opens
Smooth transition from envelope scene to card scene

Interactive Card

Floating animated hearts in the background
Bouncing cupid illustration
"Yes" and "No" buttons — but the No button has a mind of its own

The Escaping No Button

Detects cursor or touch proximity and runs away before you can click it
Zigzag escape path with randomised waypoints
Leaves a trail of tiny hearts as it flees
Panics and shakes after being chased 3+ times
Shrinks slightly with each escape attempt
Changes text each time it runs (Nope!, Ahh!!, Too slow~, HELP!, etc.)
The Yes button grows bigger the more the No button escapes

Success Screen

Confetti and heart burst animation on clicking Yes
Confirmation card with a "reservation" for Valentine's Day
Celebration animation with floating hearts


🛠️ Technical Details
Technologies used:

Vanilla HTML5, CSS3, JavaScript — no frameworks, no build tools
HTML5 Canvas-compatible animations via CSS @keyframes
Touch and mouse event handling for mobile and desktop
SVG hearts generated dynamically in JavaScript
CSS clip-path for the envelope triangle flap
CSS 3D perspective and rotateX for the envelope opening animation

Browser support:

Modern browsers (Chrome, Firefox, Safari, Edge)
iOS Safari and Chrome Mobile
Fully touch-optimised — works on phones


🚀 Getting Started
This is a single-file application. No install or build process required.
Option A — Local server (recommended):
bash# Python 3
python -m http.server 8080

# Node.js
npx http-server -p 8080
Then open http://localhost:8080/index.html
Option B — Open directly in browser:
Double-click index.html — note that some animations may behave differently without a local server.

📁 Project Structure
valentinesdaycard/
├── index.html       # Entire application — self-contained single file
├── cupid.png        # Cupid illustration used in card and success screen
├── word.png         # "Be My Valentine?" lettering image
└── README.md        # This file

🎨 Design System
TokenValueUsageMain Pink#f7b4c4Card background, gradientLight Pink#fcc8d4Envelope body, gradient startEnvelope Pink#e8a0b2Envelope body fillFlap Pink#d6889cEnvelope flapRed#e01030Buttons, text, heartsDark Red#c00020Button borders, accents
Typography: Caveat (Google Fonts) — handwritten feel throughout

💡 How the No Button Escape Works

Mouse or touch position is tracked continuously
When the pointer gets within escapeRadius pixels of the No button, escape is triggered
The button calculates a direction away from the pointer
It generates 3–4 randomised waypoints in that direction, with zigzag variation
Each waypoint is clamped to the viewport so the button never leaves the screen
Overlap with the Yes button is detected and avoided
A heart trail is dropped at the button's previous position on each escape
escapeRadius grows with each escape, making it progressively harder to approach


📜 License
Made with ❤️ by Evelynn Chang — free for personal use.

🔗 Links

Instagram: @evelynn.creates_
GitHub: Evelynn1119

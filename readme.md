# 📝 Sticky Notes Wall

A dynamic, interactive digital "Wall of Inspiration" built with Vanilla JavaScript. This project spawns colorful, macOS-style sticky notes containing productivity tips, developer humor, success mantras, and calming reminders.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Vanilla JS](https://img.shields.io/badge/javascript-vanilla-yellow.svg)
![Responsive](https://img.shields.io/badge/responsive-mobile--friendly-brightgreen.svg)

## ✨ Features

- **Infinite Spawning:** Notes appear automatically at set intervals, filling your screen with wisdom and humor.
- **Interactive Windows:** Each note is a mini-window with:
  - 🔴 **Close:** Removes the note from the wall.
  - 🟡 **Minimize:** Smoothly shrinks and removes the note.
  - 🟢 **Maximize:** Expands the note to full-screen "Focus Mode" (Double-click the header also works!).
- **Drag & Drop:** Real-time movement of cards with smooth transitions.
- **Dynamic Environment:** 
  - The browser tab title and favicon update every 3 seconds to reflect the "mood" of the wall.
  - Responsive layout adapts card counts and sizes for Mobile vs. Desktop.
- **Categorized Content:** Messages are pulled from 5 categories: Productivity, Development, Funny, Calm, and Success.

## 🚀 Quick Start

Since this is a standalone project, no installation is required.

1.  Clone this repository or copy the code.
2.  Open `index.html` in any modern web browser.

```html
# If using a local server (optional)
npx serve .
```

## 🛠️ Customization

You can easily customize the experience by modifying the constants in the `<script>` section:

### Changing Content
Locate the arrays like `productivityNotes` or `funnyNotes` to add your own messages:
```javascript
const productivityNotes = ["Your new message here", "Stay focused!"];
```

### Adjusting Speed & Limits
Modify the following variables to change the wall behavior:
- `maxCards`: Maximum notes allowed on screen.
- `spawnInterval`: How fast new notes appear (in milliseconds).
- `colors`: Add or remove HEX codes to change the note color palette.

## 📱 Mobile Support
The app is fully touch-compatible. 
- **Tap & Drag:** Move notes around the screen.
- **Optimized UI:** Cards automatically resize and the spawn rate slows down on mobile devices to ensure smooth performance.

## 🧰 Technical Details
- **CSS-in-JS Animations:** Uses `transform: scale() rotate()` for high-performance rendering.
- **State Tracking:** Uses `WeakMap` for efficient memory management of card properties.
- **Adaptive Viewports:** Uses `dvh` (Dynamic Viewport Height) units for perfect scaling on mobile browsers.



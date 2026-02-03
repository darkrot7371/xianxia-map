# xianxia-map
A Procedural Generation Map Engine

# 🌌 Xianxia Infinite Realm: The Divine Sense Explorer

Welcome to the **Xianxia Infinite Realm**, a procedurally generated, infinite exploration engine built directly for the browser. This project is a fusion of modern web technology and the mystical themes of Chinese high fantasy (Xianxia). 

In this realm, you are not just a traveler; you are a cultivator using your **Divine Sense** to navigate a world that spans billions of coordinates, generated mathematically in real-time.

---

## 📜 Table of Contents
1. [The Vision](#the-vision)
2. [Core Gameplay Mechanics](#core-gameplay-mechanics)
3. [The World Engine (Technical Deep Dive)](#the-world-engine-technical-deep-dive)
4. [Biomes and Landmarks](#biomes-and-landmarks)
5. [How to Play: A Cultivator's Guide](#how-to-play-a-cultivators-guide)
6. [Controls & Commands](#controls--commands)
7. [Installation & Requirements](#installation--requirements)
8. [The "Dao" of the Code](#the-dao-of-the-code)
9. [Future Roadmap](#future-roadmap)
10. made by "Dark Rot"

---

## 🧐 The Vision
The **Xianxia Infinite Realm** was designed to capture the feeling of an "Infinite Plane." Unlike traditional games with boundaries, this project uses deterministic noise functions to ensure that every coordinate $(x, y)$ always corresponds to the same terrain, regardless of when or how you arrive there. 

It is a lightweight, single-file "Zen" experience where users can discover hidden sects, ancient ruins, and mystical forests while recording their journey in a "Divine Ledger."

---

## 🎮 Core Gameplay Mechanics

### 1. Divine Sense (The Map)
The main interface is an 11x11 grid representing your immediate surroundings. The center tile is your current location. As you move, the world "unfolds" around you.

### 2. The Ledger (Scribe Edict)
Every location in the infinite realm can be interacted with. By clicking on a tile or using the **Inspect (👁️)** tool, you can open a notebook. This allows you to "Scribe an Edict"—leaving a permanent note or lore entry for that specific coordinate. Tiles with saved notes will glow with a golden marker.

### 3. Movement & Void Drifting
Standard movement allows you to traverse the landscape tile-by-tile. However, for those seeking distant lands, the **Void Drift** feature allows you to leap thousands of miles in a random direction, instantly transporting your consciousness to a new corner of the world.

### 4. Reincarnation
If you wish to see a completely different universe, the **Reincarnate** function resets the world's "Seed." This reshapes the entire mathematical foundation of the realm, creating new continents, oceans, and mountain ranges.

---

## 🛠 The World Engine (Technical Deep Dive)

The world is built on a **Procedural Generation Stack** that requires no backend or database.

* **Seeding:** A 6-digit seed acts as the "DNA" of your universe.
* **Hashing:** A custom `hash(x, y)` function creates pseudorandom values based on coordinates.
* **Bilinear Interpolation:** This smooths out the raw random values to create natural-looking transitions between land and water.
* **Fractal Brownian Motion (fbm):** The engine uses multiple "octaves" of noise. This adds layers of detail—simulating the jaggedness of mountains and the gentle curves of coastlines.
* **Qi Density:** A hidden variable in the code determines the "Qi" of a region, affecting whether rare biomes like the **Jade Forest** or **Volcanoes** appear.

---

## 🏔 Biomes and Landmarks

As you travel, you will encounter distinct environments, each with its own visual identity and lore description:

| Biome | Color | Description |
| :--- | :--- | :--- |
| **Abyssal Sea** | Deep Black | Crushing depths where the light of the sun cannot reach. |
| **Spirit Ocean** | Dark Blue | Endless waters teeming with aquatic spirit beasts. |
| **Spirit Plains** | Deep Green | The heart of the mortal world; vast and peaceful. |
| **Deep Forest** | Dark Green | Ancient woods where the canopy hides the sky. |
| **Jade Forest** | Jade Green | A rare zone where Qi is so high that the bamboo glows. |
| **Dune Sea** | Golden Brown | Scorching sands that test a cultivator's endurance. |
| **Spirit Mountain** | Grey | Jagged peaks perfect for establishing a Sect. |
| **Heavenly Peak** | Snow White | The highest points of the world, frozen in eternal winter. |
| **Volcano** | Crimson | Unstable regions where the earth's fire leaks out. |

### 🏯 Special Landmarks
You may also find **Settlements** marked with unique icons:
* **🏯 Imperial Capital:** The massive heart of human civilization.
* **⛩️ Sect:** Where cultivators gather to seek immortality.
* **🏰 Fortress:** Military outposts guarding the borders.
* **🛕 Ruins:** Echoes of fallen civilizations containing ancient treasures.
* **⚓ Port City:** Coastal hubs found where the land meets the ocean.

---

## 📖 How to Play: A Cultivator's Guide

1.  **Open the Realm:** Launch the `xiaxia-map.html` file in any modern web browser (Chrome, Firefox, Safari, or Edge).
2.  **Observe your Surroundings:** Look at the **Divine Sense** display at the top left to see your current $(x, y)$ coordinates.
3.  **Traverse the Land:** Use the On-Screen D-Pad or your Keyboard (WASD/Arrows) to move.
4.  **Seek the Dao:** Wander until you find a location that interests you—perhaps a rare **Jade Forest** or a **Volcano**.
5.  **Record your Journey:** Click on your current tile. A modal will appear. Type your thoughts, lore, or "cultivation progress" into the box and click **Scribe Edict**.
6.  **Drift through the Void:** If you feel stuck in one region, click **Void Drift** to teleport to a far-off land.
7.  **Ascend or Reset:** Use **Reincarnate** when you are ready to explore a completely different reality.

---

## ⌨️ Controls & Commands

* **W / Up Arrow:** Move North
* **S / Down Arrow:** Move South
* **A / Left Arrow:** Move West
* **D / Right Arrow:** Move East
* **Enter / Space:** Inspect current location (Open Notebook)
* **Mouse Click:** Click any tile on the map to view its details and write notes.

---

## 💻 Installation & Requirements

No installation is required. This is a "Portable Realm."

1.  Download the `xiaxia-map.html` file.
2.  Double-click it to open it in your browser.
3.  **Mobile Friendly:** The game is fully responsive. You can open this on a smartphone and use the touch-based D-pad to play.

---

## 🧬 The "Dao" of the Code
The entire project is contained in a single file to demonstrate the power of **Vanilla JavaScript** and **CSS Grid**. 

* **No Frameworks:** No React, Vue, or external libraries.
* **Zero Assets:** All icons are Emojis, and all graphics are CSS-based, making the "game" weigh only a few kilobytes.
* **Performance:** The map renders instantly because it only calculates the 121 tiles currently visible to the player.

---

## 🗺 Future Roadmap
* **Inventory System:** Collect herbs and spirit stones from specific biomes.
* **Encounter System:** Randomly trigger "Tribulations" or meetings with other cultivators.
* **Fog of War:** A system to hide tiles until they have been "scanned" by Divine Sense.
* **Export Ledger:** The ability to download your saved notes as a JSON file.

---



**Made by Dark Rot**

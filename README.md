# Playable Ads & Creative Technology Portfolio

A collection of 3 production-ready HTML5 playable ads engineered within a strict 20-hour sprint. Designed for instant loading, mobile touch optimization, and high-conversion marketing funnels.

🎮 **[Live Hub Demo - Play the Ads Here](https://mihaellk.github.io/playable-ads-portfolio/)**

## 🏗️ Technical Architecture & Constraints Met
This repository demonstrates core competencies in ad-tech game development:
- **Single-File Output:** Configured via `vite-plugin-singlefile` to generate self-contained HTML payloads (inline CSS/JS, Base64 assets) ready for ad network injection (AppLovin, Meta, ironSource).
- **Config-Driven Systems:** Each game implements a `gameConfig.ts` to separate logic from parameters (speed, duration, total obstacles), allowing rapid A/B testing without recompiling core mechanics.
- **Responsive & Touch-First:** Handled `pointerdown/pointerup` events universally to ensure seamless parity across desktop testing and mobile WebViews, preventing hitbox offset issues on aspect ratio changes.
- **Web Audio Compliance:** Custom silent-buffer unlock system tied to the first user interaction to bypass modern browser autoplay restrictions.
- **MRAID / Tracking Hooks:** Standardized event logging (`game_start`, `first_interaction`, `cta_clicked`) built into the game loop lifecycle.

## 📦 The Micro-Experiences

### 1. [Insert Name] (Phaser 3)
- **Focus:** 2D Physics-lite, Game Juice (tweens, particles), and clear onboarding (3-second rule).
- **Core Tech:** Phaser 3, TypeScript.

### 2. [Insert Name] (PixiJS)
- **Focus:** UI architecture, modular mini-game state machines, and responsive layouts.
- **Core Tech:** PixiJS, GSAP.

### 3. Tiny Wheels - 3D Fake Runner (Three.js)
- **Focus:** Performance-first 3D, Custom DeltaTime loop replacing deprecated APIs, AABB collision.
- **Core Tech:** Vanilla TypeScript, Three.js (Zero third-party loaders).

## 🚀 Local Deployment
To run the hub and compile the games locally:
```bash
git clone [https://github.com/mihaellk/playable-ads-portfolio.git](https://github.com/mihaellk/playable-ads-portfolio.git)
cd playable-ads-portfolio
npm install
npm run dev
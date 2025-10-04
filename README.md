# BrowserRift 🌌

> An open-source arcade of experimental web games that break the fourth wall of your browser. Play across multiple windows where actions in one tab magically affect the other.

This repository is a growing arcade of unique, browser-based games and interactive experiences built on a simple yet powerful premise: **real-time synchronization across browser windows.**

## 🎯 The Vision

Our mission is to build an open-source playground that explores the creative frontier of the web browser. We are achieving this by:

- **🎮 Redefining Local Multiplayer:** Creating novel co-op and PvP games that two people can play on the same machine.
- **🎨 Building Interactive Art:** Designing digital toys where separate windows act as portals to a single, cohesive world.
- **🧑‍💻 Making Advanced APIs Accessible:** Demonstrating the power of `LocalStorage` and `BroadcastChannel` in a fun, hands-on way.

## 🚀 How to Play

Getting started with BrowserRift is simple! Follow these steps to experience the magic:

1. **Clone or Download the Repository:**

   ```bash
   git clone https://github.com/rohan-27p/BrowserRift.git
   cd BrowserRift
   ```

2. **Open the Main Page:**

   - Open `index.html` in your web browser (Chrome, Firefox, Edge, or Safari recommended)
   - You'll see a gallery of all available games and visualizers

3. **Launch a Game or Visualizer:**

   - Click on any thumbnail in the gallery to open that experience
   - Each game/visualizer will open in a new window or tab

4. **Experience the Multi-Window Magic:**
   - **For single-window experiences:** Simply interact and enjoy!
   - **For multi-window games:** Open multiple instances by clicking the launch button multiple times or duplicating the tab
   - Watch as actions in one window affect the others in real-time!

### Tips:

- For the best experience, arrange your browser windows side-by-side
- Some games require 2 players - perfect for sharing with a friend on the same computer
- Make sure your browser allows pop-ups from the local file

## 🎪 Game Showcase

Explore our growing collection of browser-bending experiences:

### 🎮 Games

- **Rift Pong:** The classic game of Pong, but with a twist. Each player controls their paddle from a separate browser tab!

### 🎨 Visualizers & Interactive Art

- **3D Cube Sync Motion:** A synchronized 3D sphere across two windows demonstrating real-time cross-window coordination using Three.js.

_Have an idea? [Contribute your own game or visualizer!](#how-to-add-a-new-gamevisualizer)_

## 🛠️ How to Add a New Game/Visualizer

Want to contribute your own creation? Here's a step-by-step guide:

### Step 1: Create Your Project Folder

Create a new folder in the `gamesNdesigns/` directory with a descriptive name:

```bash
cd gamesNdesigns
mkdir my-awesome-game
```

### Step 2: Build Your Experience

Create an `index.html` file in your new folder. This is the entry point for your game/visualizer:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>My Awesome Game</title>
  </head>
  <body>
    <!-- Your game code here -->
    <script src="main.js"></script>
  </body>
</html>
```

**Key Requirements:**

- Keep all assets (JS, CSS, images) within your game folder
- Use `localStorage` or `BroadcastChannel` API for cross-window communication
- Ensure your game works in modern browsers
- Test with multiple windows/tabs to verify synchronization

### Step 3: Create a Thumbnail

Create a `thumbnail.png` file (recommended size: 400x300px or 4:3 aspect ratio) that represents your game. This will be displayed in the main gallery.

### Step 4: Update the Manifest

Add your game entry to the `manifest.json` file in the root directory:

```json
{
  "title": "My Awesome Game",
  "description": "A brief description of what makes your game unique",
  "folder": "my-awesome-game",
  "thumbnail": "thumbnail.png",
  "author": "your-github-username",
  "tags": ["Game", "2-Player", "Your-Tag"]
}
```

### Step 5: Test and Submit

1. Test your game thoroughly by opening `index.html` in the root directory
2. Verify your game appears in the gallery with the correct thumbnail
3. Submit a Pull Request following our [contribution guidelines](CONTRIBUTING.md)

## 🙌 How to Contribute

We welcome contributions of all kinds! Whether you're fixing a bug, improving documentation, or creating a new game, we'd love to have you involved. This is a perfect project for **Hacktoberfest**.

1.  Find an issue to work on in the [Issues tab](https://github.com/rohan-27p/BrowserRift/issues). Look for ones tagged `hacktoberfest` or `good first issue`.
2.  If you have a new game idea, please [create a new issue](https://github.com/rohan-27p/BrowserRift/issues/new) to discuss it first.
3.  Follow the detailed instructions in our [CONTRIBUTING.md](CONTRIBUTING.md) file to get started.

---

Made with ❤️ for Open Source.

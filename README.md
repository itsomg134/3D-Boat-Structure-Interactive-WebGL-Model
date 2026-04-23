#  3D Boat Structure - Interactive WebGL Model

An interactive, real-time 3D visualization of a classic sailboat built with **Three.js**. Explore the boat’s hull, mast, sail, and rigging in a dynamic ocean environment with realistic lighting, shadows, and gentle water animation.

![3D Boat Structure Preview](https://via.placeholder.com/800x400?text=3D+Boat+Visualization)

##  Features

- **Fully Detailed 3D Model** – Hull, keel, bow, stern, deck, mast, yard, canvas sail, rigging ropes, and a small flag.
- **Realistic Materials** – Wood textures for the hull and mast, semi-transparent canvas sail, metallic water surface.
- **Dynamic Environment** – Animated water waves, floating particles, subtle boat rocking, drifting clouds, and a starfield background.
- **Interactive Controls** – Orbit, pan, and zoom with mouse or touch.
- **Informative Labels** – CSS2D labels identify key parts of the boat.
- **Optimized Lighting** – Directional sunlight, ambient fill, rim light, and hemisphere light create depth and realism.

## 🎮 Controls

| Action               | Input                              |
| -------------------- | ---------------------------------- |
| Rotate view          | Left-click + drag                  |
| Pan                  | Right-click + drag                 |
| Zoom                 | Scroll wheel / pinch               |

## 🚀 Live Demo

> *(If hosted on GitHub Pages or another platform, replace the link below)*

🔗 [View Live Demo](https://your-username.github.io/3d-boat-structure)

## 🛠️ Technologies Used

- [Three.js](https://threejs.org/) – WebGL 3D library
- JavaScript (ES6 Modules)
- CSS2DRenderer for text labels
- HTML5/CSS3

## 📂 Project Structure

```
3d-boat-structure/
├── index.html          # Main entry point (contains all code)
└── README.md           # Project documentation
```

> The entire application is contained in a single HTML file for easy deployment and sharing.

## 🧩 How It Works

1. **Scene Setup** – A Three.js scene with perspective camera, WebGL and CSS2D renderers, and orbit controls.
2. **Lighting** – Combination of directional, point, ambient, and hemisphere lights to simulate natural outdoor lighting.
3. **Boat Construction** – Individual `BoxGeometry`, `CylinderGeometry`, `ConeGeometry`, and `TubeGeometry` meshes grouped together to form the boat.
4. **Water Animation** – Vertex shader-less dynamic wave modification of a plane mesh using sine/cosine functions.
5. **Labels** – CSS2DRenderer places HTML divs that always face the camera.
6. **Animation Loop** – Updates water vertices, boat rocking, flag waving, cloud positions, and light intensity.

## 📦 Local Installation

To run this project locally:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/3d-boat-structure.git
   cd 3d-boat-structure
   ```

2. Start a local server (e.g., using VS Code Live Server, Python HTTP server, or `npx serve`):
   ```bash
   # Python 3
   python -m http.server 8000

   # Node.js (npx)
   npx serve
   ```

3. Open your browser and navigate to `http://localhost:8000`

> No build steps or dependencies are required – the script imports Three.js from CDN.

## 🎨 Customization Ideas

- **Change Boat Colors** – Modify the `color` values in `MeshStandardMaterial` parameters (hull, sail, mast).
- **Adjust Water Movement** – Edit the `animateWater()` function to change wave frequency/amplitude.
- **Add More Details** – Include an anchor, lifebuoy, or additional sails.
- **Replace Water Texture** – Use a custom shader or load an environment map for reflections.

## 📸 Screenshots

| Perspective | Close-up on Hull |
|-------------|------------------|
| *(Add screenshot 1)* | *(Add screenshot 2)* |

## 📄 License

MIT License – free for personal and commercial use.

## 🙏 Acknowledgements

- Built with [Three.js](https://threejs.org/)
- Inspired by classic sailing vessels and maritime aesthetics

---

**Enjoy sailing the digital seas!** 🌊⛵
```

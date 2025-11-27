# 🖐️ Telekinetic Particles (Web-Kinesis)

> **A real-time, interactive 3D particle morphing system controlled by hand gestures.**

**Telekinetic Particles** is a web-based experiment that combines **Three.js** for high-performance particle rendering with **Google MediaPipe** for computer vision. It allows users to manipulate a cloud of 15,000+ glowing particles using nothing but their webcam and hand movements—no mouse or keyboard required.


## ✨ Features

  * **Hand Gesture Control**: Uses computer vision to track your thumb and index finger distance.
      * 🤏 **Pinch**: Condenses the particle cloud.
      * 🖐️ **Open Hand**: Expands and diffuses the particles.
  * **Real-time Morphing**: Seamlessly transition between different mathematical 3D structures:
      * ❤️ **Heart**: A parametric 3D heart shape.
      * 🪐 **Saturn**: A planet with a tilted ring system.
      * 🌸 **Lotus**: A procedural flower shape based on rose curves.
      * 🎆 **Fireworks**: Dynamic, exploding particle effects.
      * 🌀 **Abstract Knot**: Complex torus knot geometry.
  * **Customization**: Real-time color picking and glassmorphism UI.
  * **Zero Backend**: Runs entirely in the browser using client-side JavaScript.

## 🛠️ Tech Stack

  * **[Three.js](https://threejs.org/)**: 3D Rendering Engine & Particle System.
  * **[MediaPipe Hands](https://developers.google.com/mediapipe)**: Real-time hand tracking and landmark detection.
  * **HTML5 / CSS3**: Layout and Glassmorphism UI styling.

## 🚀 Quick Start

Due to browser security policies regarding webcam access (CORS), **you cannot simply double-click the `.html` file**. You must run it through a local server.

### Option 1: VS Code (Recommended)

1.  Install the **"Live Server"** extension in VS Code.
2.  Right-click `index.html` and select **"Open with Live Server"**.

### Option 2: Python

If you have Python installed (macOS/Linux/Windows), run this in your terminal:

```bash
# Go to the project directory
cd path/to/project

# Start a simple server
python3 -m http.server
```

Then open your browser and visit: `http://localhost:8000`

### Option 3: Node.js

```bash
npx serve .
```

## 🎮 Controls

1.  **Allow Camera Access** when prompted by the browser.
2.  **Raise your hand** in front of the camera.
3.  **Interact**:
      * Move your hand closer/further to test tracking.
      * **Pinch** your fingers to make the shape smaller.
      * **Release** your fingers to make the shape breathe and expand.
4.  **UI Panel**: Use the top-right panel to switch shapes or change the particle color.

## 🔧 Troubleshooting

  * **Camera Light Not Turning On?**
      * Ensure you are running on `localhost` or `https`. Most browsers block camera access on insecure `http` (except localhost).
      * Check your OS privacy settings (System Settings -\> Privacy -\> Camera).
  * **Particles Not Appearing?**
      * Wait a few seconds for the MediaPipe AI model to download (dependent on internet speed).
      * Check the browser console (F12) for any network errors.


# Fog Mirror

An interactive, in-browser canvas that transforms your webcam into a virtual, steamy mirror. Exhale to create realistic condensation over your reflection, then draw or wipe it away in real time using hand gestures powered entirely by on-device computer vision.

## ✨ Features

- **Gesture Interaction:** Draw fine lines using a pinch gesture or wipe away large areas with a closed fist.
- **Audio-Reactive Condensation:** Detects breath sounds through your microphone to dynamically generate realistic fog effects.
- **Privacy by Design:** No data streaming. Audio and computer vision processing run entirely within your browser.
- **Real-Time Rendering:** Interactive fog, drawing, and wiping effects rendered using HTML5 Canvas and WebGL.
- **Keyboard Shortcuts:** Control the experience with simple keyboard commands.
- **Zero Build Step:** Built with vanilla JavaScript, HTML5 Canvas, and CSS, with no build process required.

## 🎮 Controls

| Action | Control |
| :--- | :--- |
| Generate Fog | Exhale into the microphone or hold `Space` |
| Draw | Pinch your thumb and index finger together |
| Wipe | Make a closed fist |
| Clear Screen | `C` |
| Save Photo | `S` or click the shutter icon |
| Toggle Debug HUD | `D` |
| Exit | `Esc` |

## 🚀 Getting Started

Camera and microphone access require a secure context, such as `localhost` or HTTPS. Run the project through a local development server instead of opening the HTML file directly.

### Prerequisites

- A modern web browser with camera and microphone support
- Python 3 or Node.js
- A webcam and microphone
- An internet connection if the project loads computer vision libraries or models from a CDN

### Run Locally

**1. Clone the repository**

```bash
git clone https://github.com/nagamanikanta5455/fog-mirror.git
cd fog-mirror
```

**2. Start a local server**

Using Python:

```bash
python -m http.server 8000
```

Alternatively, using Node.js:

```bash
npx serve .
```

**3. Open the application**

Navigate to:

```text
http://localhost:8000
```

**4. Grant permissions**

Allow camera and microphone access when your browser prompts you. Once the application initializes, interact with the virtual mirror using the supported gestures and keyboard shortcuts.

## 🛠️ Built With

- **Languages:** HTML5, CSS3, JavaScript
- **Computer Vision:** MediaPipe Hands and Face Detection
- **Rendering:** HTML5 Canvas and WebGL
- **Audio Processing:** Web Audio API (`AnalyserNode`)
- **Typography:** Inter

## 🔒 Privacy

Fog Mirror is designed to process camera, hand-tracking, and audio input locally in the browser. It does not require uploading your webcam footage or microphone recordings to a remote server.

External libraries or models may be loaded from a CDN, depending on the implementation. Review the source code and network requests to verify the application's actual data flows.

## 📸 Controls at a Glance

| Key | Function |
| :---: | :--- |
| `Space` | Generate fog |
| `C` | Clear the mirror |
| `S` | Save a photo |
| `D` | Toggle debug information |
| `Esc` | Exit |

## 📄 License

This project is licensed under the MIT License. See the [`LICENSE`](LICENSE) file for details.

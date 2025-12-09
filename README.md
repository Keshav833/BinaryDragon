<div align="center">

# 🐉✨ **Smoothed Hand-Tracking Dragon**
### _A futuristic interactive ASCII dragon controlled by your hands_

![Made with JS](https://img.shields.io/badge/Made%20with-JavaScript-F7DF1E?style=for-the-badge)
![MediaPipe](https://img.shields.io/badge/MediaPipe-Hands-blue?style=for-the-badge)
![Canvas](https://img.shields.io/badge/HTML5-Canvas-orange?style=for-the-badge)

</div>

---

## 🌌 **Overview**

This project animates a **cyber-style ASCII dragon** that **follows your fingertip in real-time** using **MediaPipe Hands**.  
Every movement is **smooth, organic, and fluid**, thanks to easing, wave functions, and procedural wing animation.

Control the dragon with:
- 🖐 **Your real hand** (via webcam), or  
- 🖱 **Your mouse cursor**

The result?  
A **living, breathing digital creature** made entirely from `"1"` and `"0"`.

---

## 🔥 **Key Features**

### 🖐 Real-Time Hand Tracking  
Uses **MediaPipe Hands** to track your index fingertip and map its movement to the dragon's head.

### 🐉 Procedural Dragon Animation  
- Segmented body with wave-like motion  
- Dynamic wings with gravity & flap logic  
- ASCII-based glowing cyber aesthetics  

### 🌈 Smooth Motion System  
- Custom easing  
- Trailing effects  
- Organic, snake-like following animation  

### 💻 Canvas-Powered Graphics  
No libraries. No frameworks. Just pure JavaScript + HTML5 Canvas magic.

---

## 🧠 **How It Works**

### 1. Hand landmark detection  
MediaPipe tracks the hand → extracts **landmark[8]** (index fingertip).

### 2. Smooth filtering  
```js
mouse.x += (rawFingertip.x - mouse.x) * smoothingFactor;
mouse.y += (rawFingertip.y - mouse.y) * smoothingFactor;

. Dragon physics

Each segment follows the previous through:

easing

directional correction

sine-wave body offset

4. Procedural wings

Wing shapes are built dynamically and flap using:

Math.sin(frame * wingFlapSpeed) * wingFlapAmplitude

🖼 Preview (Add Screenshot/GIF Here)
![Dragon Demo](assets/dragon-demo.gif)

📦 Installation & Usage
1️⃣ Clone the repository
git clone https://github.com/your-username/hand-tracking-dragon.git
cd hand-tracking-dragon

2️⃣ Run the project

Just open the HTML file in any browser:

index.html

3️⃣ Allow camera access

Webcam permission is required for hand tracking.

4️⃣ Move your hand

The dragon will follow your index finger smoothly.

🛠 Configuration (Customize the Dragon)

Inside config:

smoothingFactor: 0.2,
numBodySegments: 50,
numWingSegments: 25,
segmentLength: 20,
wingFlapSpeed: 0.060,
waveFrequency: 0.003,
headSize: 50,


You can modify:

speed

body length

wing style

wave motion

visual aesthetics

🚀 Future Upgrades

🔥 Fire-breathing effect

🌈 Neon gradient particle trails

👾 Multi-dragon mode

🎮 Game version (collect orbs, avoid enemies)

🎨 Skins/theme selector

❤️ Credits

MediaPipe Hands — for real-time tracking

HTML5 Canvas — for rendering

Custom animation logic & ASCII dragon art

<div align="center">
⭐ If you like this project, give it a star!

Made with ❤️ by creative coding.

</div> ```
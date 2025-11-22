# Dodge Game – Python Kivy

A simple dodge-style game built using **Python** and **Kivy**, created as a beginner-friendly project for mobile game development.  
Move the player left and right to avoid falling enemies. Each successful dodge increases your score. A collision resets the game.

---

## 🎮 Features
- Player movement using **touch** or **mouse**
- Random enemy spawns with increasing difficulty
- Fullscreen background image
- Realtime scoring system
- **Sound effects:**
  - `point.wav` → score increase  
  - `hit.wav` → collision  
- Player & enemy sprites using **transparent PNG** assets
- Game starts immediately on launch (no start screen)
- Ready to build for Android APK using **Buildozer**
- Supports future features (gyroscope, animations, etc.)

---

## 🖥️ Run on PC (Windows / Linux / Mac)

### 1. Install dependencies
```bash
pip install kivy
pip install kivy[base]
```

### 2. Run the game
```bash
python main.py
```

---

## 📱 Build for Android (APK)

Requires **Linux** or **WSL** (Windows Subsystem for Linux).

### 1. Install Buildozer & system requirements
```bash
pip install buildozer
sudo apt install -y python3-pip python3-setuptools python3-dev
sudo apt install -y build-essential git unzip
sudo apt install -y openjdk-17-jdk
sudo apt install -y libandroid-tools
```

### 2. Initialize Buildozer
```bash
buildozer init
```

### 3. Build APK (Debug mode)
```bash
buildozer -v android debug
```

Your APK will be generated in:
```
bin/*.apk
```

---

## 📂 Project Structure
```
dodge-game/
│── main.py
│── dodge.kv
│── assets/
│    ├── bg.png
│    ├── player.png
│    ├── enemy_red.png
│    ├── enemy_green.png
│── sounds/
│    ├── point.wav
│    └── hit.wav
│── buildozer.spec
└── README.md
```

---

## 📜 License
Free to use, modify, and learn from.  
This project is intended for educational and personal development purposes.

---

## ⭐ Notes
Feel free to improve or extend this project with:
- Gyroscope movement support  
- Animated sprites  
- Game Over screen  
- Highscore save system  
- Background music  

Pull requests are welcome!

# 🕹️ Fly and Spy

Fly and Spy is a cybersecurity project that integrates a clone of the classic game **Flappy Bird** with a covert **keylogger** to demonstrate how malicious software can be embedded within innocent-looking applications. This project was developed as part of an **Introduction to Cybersecurity Lab** and emphasizes technical integration along with ethical considerations.

---

## 🚀 Project Objectives

- ✅ Develop a functional Flappy Bird clone.
- 🕵️ Integrate a stealthy keylogger that:
  - Logs **keystrokes**.
  - Captures **active window titles**.
  - Saves logs locally and **uploads to Dropbox**.
  - **Auto-starts** with the system on boot.

---

## 🎮 Game: Flappy Bird Clone

### 📋 Overview
The game replicates the Flappy Bird mechanics—players control a bird using the space bar to fly through gaps in pipes.

### 🔧 Key Features
- **Dynamic Gameplay:** Gravity-based bird movement.
- **Customizable Settings:** Game speed, gravity, pipe gaps.
- **Resizable Screen:** Adjusts to various window sizes.

### 🧱 Code Structure
- **Classes:**
  - `Bird`: Manages movement, collision.
  - `Pipe`: Creates and moves pipes.
- **Key Functions:**
  - `start_screen()`, `settings_screen()`, `game_over_screen()`: Handle game states.
  - `main()`: Core game loop and rendering.
- **Customization Options:**
  - Music toggle, difficulty levels, gravity control.

---

## 🛡️ Keylogger Component

### 🔍 Overview
Runs stealthily in the background while the game is active, collecting and transmitting user data.

### 📌 Features
- **Keystroke Logging:** Captures all keys (including special keys).
- **Active App Logging:** Tracks current window titles.
- **Dropbox Sync:** Periodically uploads log files to Dropbox.
- **Startup Integration:** Ensures persistence across reboots.

### 🧱 Code Structure
- **Functions:**
  - `add_to_startup()`: Adds keylogger to system startup.
  - `log_key()`: Records each key press.
  - `log_active_application()`: Captures app titles.
  - `upload_file_to_dropbox()`: Handles file uploads.
- **Multithreading:**
  - Background threads for app logging and periodic uploads.
- **Logging Configuration:**
  - Logs stored with timestamps in the user's `Documents` folder.

---

## 🔄 Integration

- The **game and keylogger run simultaneously**.
- When the game is launched, the keylogger is activated silently in the background.
- Ensures **minimal performance impact** and maintains stealth.

---

## ⚠️ Ethical Considerations

> This project is strictly for **educational** and **ethical demonstration** purposes only.

- 🚫 **Unauthorized use of keyloggers is illegal.**
- ✅ Intended for use in **controlled environments** to raise awareness.
- 📣 Highlights the importance of **cyber hygiene** and software trustworthiness.

---

## 🧩 Challenges Faced

- 🔄 Game-keylogger integration without performance lag.
- 🖥️ Platform-specific startup configuration.
- ⚙️ Thread synchronization and log handling.
- 🛠️ Robust error handling for Dropbox and I/O operations.

---

## 📚 Conclusion

Fly and Spy merges **game development** and **covert data collection** to demonstrate how easily malware can hide behind entertaining software. It showcases:

- 🎯 Game mechanics and UI development.
- ⚙️ Background process handling with multithreading.
- ☁️ Secure cloud sync (Dropbox API).
- 🔐 Real-world cybersecurity implications.

---

## 📎 Disclaimer

This software is for educational purposes only. **Do not** deploy this project outside authorized lab environments. Misuse of surveillance tools is a **criminal offense**.

---

## 👨‍💻 Author

**Muhammad Adeel Haider**  
[GitHub Profile](https://github.com/4deeel)  
BS Cybersecurity – Air University

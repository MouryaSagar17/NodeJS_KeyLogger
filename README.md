# NodeJS_KeyLogger
A low-level Linux-based keyboard input event listener built using Node.js. This tool reads raw keystroke data from /dev/input/event* devices using the Linux Input Subsystem, parses keyboard scan codes, and emits high-level key events in real-time.
# ⚠️ Disclaimer:
This project is strictly for educational and ethical security research purposes. Unauthorized use of this code to monitor or record input from others without explicit consent is illegal and unethical. Always ensure you have proper authorization when using this tool.

# 🔍 Features
Monitors keyboard input from /dev/input/event*

Emits keydown, keypress, and keyup events

Uses event codes and maps them to readable key labels

Emits structured key events with timestamps

Modular and easy to integrate into other Node.js projects

# 🧑‍💻 Use Case (Ethical Only)
Educational demonstration of low-level input handling

Building Linux automation or accessibility tools

Cybersecurity labs for ethical penetration testing with consent

# 📦 Installation
bash
git clone https://github.com/MouryaSagar17/NodeJS_KeyLogger

cd NodeJS_KeyLogger

npm install

# 🚀 Quick Start
js
const Keyboard = require('./Keyboard');

const kb = new Keyboard('event3'); // Replace with your input device

kb.on('keydown', (event) => {
  console.log(`[KEYDOWN] ${event.keyId}`);
});
🛑 Requirements
Linux-based OS

Root or sudo privileges to access /dev/input/*

Node.js 12+

# 📁 File Structure
Keyboard.js – Core logic for parsing input event streams

keycodes.js – Mapping of key codes to human-readable strings

# ✅ Legal/Ethical Use Only
By using this project, you agree to:

Not use it to spy on or steal private information

Use it only in systems or environments you own or are authorized to test

Comply with all local and international data privacy laws

# 📄 License
This project is licensed under the MIT License.
See LICENSE for details.


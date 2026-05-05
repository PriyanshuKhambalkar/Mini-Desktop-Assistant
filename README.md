<div align="center">

```
 █████╗ ███████╗███████╗██╗███████╗████████╗ █████╗ ███╗   ██╗████████╗
██╔══██╗██╔════╝██╔════╝██║██╔════╝╚══██╔══╝██╔══██╗████╗  ██║╚══██╔══╝
███████║███████╗███████╗██║███████╗   ██║   ███████║██╔██╗ ██║   ██║   
██╔══██║╚════██║╚════██║██║╚════██║   ██║   ██╔══██║██║╚██╗██║   ██║   
██║  ██║███████║███████║██║███████║   ██║   ██║  ██║██║ ╚████║   ██║   
╚═╝  ╚═╝╚══════╝╚══════╝╚═╝╚══════╝   ╚═╝   ╚═╝  ╚═╝╚═╝  ╚═══╝   ╚═╝   
```

### Voice-Powered Python Desktop Assistant

*Automate your desktop with your voice — open apps, search the web, check the time and more.*

<br/>

<img src="https://img.shields.io/badge/Python-3.x-3776ab?style=for-the-badge&logo=python&logoColor=white&labelColor=1a1a2e"/>
<img src="https://img.shields.io/badge/SpeechRecognition-Voice%20Input-ef4444?style=for-the-badge&logoColor=white&labelColor=1a1a2e"/>
<img src="https://img.shields.io/badge/pyttsx3-Text%20to%20Speech-10b981?style=for-the-badge&logoColor=white&labelColor=1a1a2e"/>
<img src="https://img.shields.io/badge/Platform-Windows%20%7C%20Linux%20%7C%20macOS-f59e0b?style=for-the-badge&logoColor=white&labelColor=1a1a2e"/>
<img src="https://img.shields.io/badge/License-MIT-6366f1?style=for-the-badge&logoColor=white&labelColor=1a1a2e"/>

<br/><br/>

</div>

---

## 📖 What is Mini Desktop Assistant?

**Mini Desktop Assistant** is a lightweight Python-based voice assistant that listens to your spoken commands and automates common desktop tasks — all without touching your keyboard. Built using Python's speech recognition and text-to-speech libraries, it demonstrates how natural language interaction can be integrated into everyday computing.

Speak a command, and the assistant responds — opening applications, searching the web, telling you the time, or answering basic queries. It is designed to be simple, readable, and easily extensible — a perfect foundation for building more advanced voice-controlled automation.

---

## ✨ Features

- 🎙️ **Voice Command Recognition** — Listens and understands spoken instructions in real time
- 🔊 **Text-to-Speech Response** — Responds audibly using natural-sounding speech via pyttsx3
- 🌐 **Web Search** — Searches Google, Wikipedia, or YouTube on voice command
- 🖥️ **Open Applications** — Launches installed desktop applications by name
- 🕐 **Time and Date** — Tells you the current time and date on request
- 📂 **File and Browser Control** — Opens websites and local files via voice
- ⚡ **Lightweight** — No heavy frameworks, no cloud dependency for TTS
- 🔧 **Easily Extensible** — Add new commands with minimal code changes

---

## 🛠️ Tech Stack

| Library / Tool | Purpose |
|----------------|---------|
| Python 3.x | Core language |
| `SpeechRecognition` | Captures and transcribes voice input via microphone |
| `pyttsx3` | Offline text-to-speech engine — converts responses to audio |
| `webbrowser` | Opens URLs and performs web searches |
| `datetime` | Provides current time and date information |
| `os` | Launches applications and interacts with the operating system |

---

## 📁 Project Structure

```
Mini-Desktop-Assistant/
│
├── assistant.py        # Main program — voice loop, command parsing, responses
├── requirements.txt    # Python dependencies
└── README.md           # Project documentation
```

---

## 🧠 How It Works

```
Program starts
      │
      ▼
Microphone activated — assistant listening
      │
      ▼
Voice captured via SpeechRecognition
      │
      ▼
Audio converted to text (Google Speech API)
      │
      ▼
Text matched against command keywords
      │
      ├── "open youtube"      →  webbrowser.open(youtube)
      ├── "search <query>"    →  Google search in browser
      ├── "what time is it"   →  datetime.now() → pyttsx3 speaks
      ├── "open notepad"      →  os.system(notepad)
      └── unknown command     →  "Sorry, I didn't understand that"
      │
      ▼
pyttsx3 speaks the response aloud
      │
      ▼
Loop back — assistant keeps listening
```

---

## ⚙️ Installation

**1. Clone the repository:**
```bash
git clone https://github.com/18PriyanshuK/Mini-Desktop-Assistant.git
cd Mini-Desktop-Assistant
```

**2. Install dependencies:**
```bash
pip install -r requirements.txt
```

**Or install manually:**
```bash
pip install SpeechRecognition pyttsx3 pyaudio
```

> **Windows users:** If `pyaudio` fails to install, use the prebuilt wheel:
> ```bash
> pip install pipwin
> pipwin install pyaudio
> ```

---

## ▶️ Usage

**1. Ensure your microphone is connected and enabled.**

**2. Run the assistant:**
```bash
python assistant.py
```

**3. Wait for the prompt, then speak a command clearly.**

---

## 🗣️ Example Commands

| Voice Command | Action |
|---------------|--------|
| `"What time is it?"` | Speaks the current time |
| `"What is today's date?"` | Speaks today's date |
| `"Search Python tutorials"` | Opens Google search |
| `"Open YouTube"` | Opens YouTube in browser |
| `"Open Notepad"` | Launches Notepad (Windows) |
| `"Search Wikipedia for AI"` | Opens Wikipedia article |
| `"Open Google"` | Opens Google homepage |

---

## ⚠️ Notes

- An active internet connection is required for the Google Speech Recognition API to transcribe voice input.
- `pyttsx3` works fully offline — no internet needed for speech output.
- Ensure microphone access is enabled in your system settings before running.
- Speak clearly and at a normal pace for best recognition accuracy.

---

## 🔮 Future Enhancements

- [ ] Wake word detection ("Hey Assistant")
- [ ] Weather information via API
- [ ] Send emails by voice
- [ ] Play music from local library or Spotify
- [ ] Set reminders and alarms
- [ ] GUI interface with voice visualiser
- [ ] Offline speech recognition using Vosk

---

## 🤝 Contributing

Contributions and new command ideas are welcome.

```bash
# Fork the repository
git fork https://github.com/18PriyanshuK/Mini-Desktop-Assistant.git

# Create a feature branch
git checkout -b feature/new-command

# Commit and push
git commit -m "Add: new voice command"
git push origin feature/new-command
```

---

## 📜 License

This project is licensed under the [MIT License](https://github.com/PriyanshuKhambalkar/Mini-Desktop-Assistant/blob/22e97ffc3a18fde89dbcd57e222b1a4d37f015d4/LICENSE) - see the LICENSE file for details.
For commercial use or redistribution, please get in touch with the author.

---

## 👤 Author

**Priyanshu Khambalkar**

---

<div align="center">

*Built with Python · SpeechRecognition · pyttsx3*

⭐ **Star this repo if it sparked your interest in voice automation**

</div>

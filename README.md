<div align="center">

<!-- HERO BANNER -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:051a10,50:0d3b2e,100:0a1628&height=200&section=header&text=Binary%20X&fontSize=62&fontColor=ffffff&fontAlignY=38&desc=Text%20%E2%86%94%20Binary%20Converter%20%E2%80%A2%20Powered%20by%20Python%20%2B%20PyQt5&descAlignY=58&descSize=16" width="100%"/>

<br/>

<!-- BADGES ROW 1 -->
[![Python](https://img.shields.io/badge/Built%20with-Python%203.x-10b981?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![PyQt5](https://img.shields.io/badge/GUI-PyQt5-0ea5e9?style=for-the-badge&logo=qt&logoColor=white)](https://pypi.org/project/PyQt5/)
[![Status](https://img.shields.io/badge/Status-Active-10b981?style=for-the-badge&logo=statuspage&logoColor=white)]()
[![License](https://img.shields.io/badge/License-MIT-f59e0b?style=for-the-badge)](LICENSE)

<!-- BADGES ROW 2 -->
[![GitHub](https://img.shields.io/badge/GitHub-mebdulrafay-181717?style=flat-square&logo=github)](https://github.com/mebdulrafay)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Hafiz%20Abdul%20Rafay-0A66C2?style=flat-square&logo=linkedin)](https://www.linkedin.com/in/hafiz-abdul-rafay-4577a5395/)
[![Email](https://img.shields.io/badge/Email-mebdulrafay@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:mebdulrafay@gmail.com)
[![HP LIFE](https://img.shields.io/badge/Certified-HP%20LIFE%20AI-0096D6?style=flat-square&logo=hp&logoColor=white)]()

<br/>

> **Binary X** is a sleek, dark-themed desktop application by **Hafiz Abdul Rafay** — converting text to binary and binary back to text with a clean PyQt5 GUI, zero dependencies, and instant clipboard support.

</div>

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Architecture](#-architecture)
- [Tech Stack](#-tech-stack)
- [Features](#-features)
- [How It Works](#-how-it-works)
- [Screenshots](#-screenshots)
- [Getting Started](#-getting-started)
- [Configuration](#-configuration)
- [About the Author](#-about-the-author)

---

## 🌐 Overview

**Binary X** is a production-ready, desktop GUI application built with Python and PyQt5. It converts any text into its 8-bit binary (ASCII) representation — and converts binary strings right back to readable text. Designed with a premium dark aesthetic and a buttery-smooth workflow.

```
User types text  ──►  Binary X App  ──►  Binary Output
                            │
          ┌─────────────────┼──────────────────┐
          ▼                 ▼                  ▼
   Text → Binary     Binary → Text      Copy / Reset
   (8-bit ASCII)    (Parse & Decode)   (Clipboard API)
```

### ✨ What Binary X Can Do

- 🔢 Convert any **text string → 8-bit binary** representation
- 🔁 Decode **binary → readable text** in reverse
- ⚡ **SWAP** content between fields with one click
- 📋 **COPY** the output directly to your clipboard
- 🔄 **RESET** both fields instantly for a fresh session
- 🎨 Fully **dark-themed** UI with a modern, minimal aesthetic

---

## 🏗 Architecture

```
┌─────────────────────────────────────────────────────────────────────┐
│                      BINARY X — APP ARCHITECTURE                     │
├─────────────────────────────────────────────────────────────────────┤
│                                                                       │
│   ┌──────────────────┐        ┌───────────────────────────────────┐  │
│   │   Text Input      │──────►│        BinaryXConverter (Core)     │  │
│   │   (QTextEdit)     │  swap │   PyQt5 QMainWindow • Dark Theme   │  │
│   └──────────────────┘        └───────────┬───────────────────────┘  │
│                                           │                           │
│                    ┌──────────────────────┼──────────────────────┐   │
│                    │                      │                       │   │
│             text_to_binary         binary_to_text           UI Layer  │
│                    │                      │                       │   │
│         ┌──────────▼──────┐   ┌──────────▼──────┐    ┌──────────┴─┐  │
│         │  ord(char)       │   │  chr(int(b, 2)) │    │  Buttons   │  │
│         │  format → 08b    │   │  Split & Parse  │    │ SWAP COPY  │  │
│         └─────────────────┘   └─────────────────┘    │   RESET    │  │
│                                                        └────────────┘  │
└─────────────────────────────────────────────────────────────────────┘
```

---

## 🛠 Tech Stack

### 🐍 Language & GUI

| Technology | Role | Version |
|:---:|:---|:---:|
| ![Python](https://img.shields.io/badge/Python-Core_Language-10b981?style=flat-square&logo=python&logoColor=white) | Application logic & conversion engine | 3.x |
| ![PyQt5](https://img.shields.io/badge/PyQt5-Desktop_GUI_Framework-0ea5e9?style=flat-square&logo=qt) | Window, widgets, layout, and styling | Latest |
| ![Qt Fusion](https://img.shields.io/badge/Qt_Fusion-Cross--Platform_Style-6366f1?style=flat-square) | Consistent UI rendering across OS | Built-in |

### 🔧 Built-In Modules Used

| Module | Purpose | Type |
|:---:|:---|:---:|
| ![sys](https://img.shields.io/badge/sys-App_Entry_%26_Exit-10b981?style=flat-square&logo=python&logoColor=white) | Launch & lifecycle management | `stdlib` |
| ![PyQt5.QtWidgets](https://img.shields.io/badge/QtWidgets-UI_Components-0ea5e9?style=flat-square) | QMainWindow, QTextEdit, QPushButton | `PyQt5` |
| ![PyQt5.QtGui](https://img.shields.io/badge/QtGui-Fonts_%26_Clipboard-6366f1?style=flat-square) | QFont, QClipboard | `PyQt5` |
| ![PyQt5.QtCore](https://img.shields.io/badge/QtCore-Alignment_%26_Events-f59e0b?style=flat-square) | Qt alignment constants | `PyQt5` |

### 🌐 Abdul Rafay's Core Tech (Portfolio)

| Category | Technologies |
|:---|:---|
| **Frontend** | ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3) ![JavaScript](https://img.shields.io/badge/JavaScript_ES6+-F7DF1E?style=flat-square&logo=javascript&logoColor=black) |
| **Python** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![PyQt5](https://img.shields.io/badge/PyQt5-41CD52?style=flat-square&logo=qt) ![CustomTkinter](https://img.shields.io/badge/CustomTkinter-blue?style=flat-square) |
| **Hardware / IoT** | ![Arduino](https://img.shields.io/badge/Arduino-00979D?style=flat-square&logo=arduino&logoColor=white) Servo • Ultrasonic Sensors • Serial Comm |
| **Design** | Glassmorphism • Branding • Social Media Creatives |
| **AI/Automation** | ![n8n](https://img.shields.io/badge/n8n-EA4B71?style=flat-square&logo=n8n) Google Gemini • LangChain Agents |

---

## ⚡ Features

| # | Feature | Description |
|:---:|:---|:---|
| 1 | **Text → Binary** | Converts each character to its 8-bit ASCII binary code, space-separated |
| 2 | **Binary → Text** | Parses space-separated 8-bit groups and decodes them back to characters |
| 3 | **SWAP Button** | Detects which field has content and performs the appropriate conversion |
| 4 | **RESET Button** | Clears both text and binary fields in one click |
| 5 | **COPY Button** | Sends the binary output directly to the system clipboard |
| 6 | **Dark Theme UI** | Full dark aesthetic with `#1a1a1a` background and `#0d7dff` accent blue |
| 7 | **Error Handling** | Gracefully handles invalid binary input with a friendly error message |

---

## 🔩 How It Works

### Text → Binary
```python
# Each character is converted to 8-bit binary using Python's format() built-in
def text_to_binary(self, text):
    binary_list = []
    for char in text:
        binary = format(ord(char), '08b')   # e.g. 'A' → '01000001'
        binary_list.append(binary)
    return ' '.join(binary_list)            # e.g. 'Hi' → '01001000 01101001'
```

### Binary → Text
```python
# Space-separated 8-bit groups are parsed and decoded back to characters
def binary_to_text(self, binary_string):
    binary_list = binary_string.split()
    text_list = []
    for binary in binary_list:
        binary = ''.join(c for c in binary if c in '01')
        if len(binary) == 8:
            char = chr(int(binary, 2))      # e.g. '01000001' → 'A'
            text_list.append(char)
    return ''.join(text_list)
```

### Example Conversion

```
Input Text:    Hello
               ─────────────────────────────────────────────────────────
Binary Output: 01001000 01100101 01101100 01101100 01101111
               H        e        l        l        o
```

---

## 📸 UI Layout

```
┌─────────────────────────────┐
│          BINARY X            │   ← Title Label
├─────────────────────────────┤
│                              │
│   Enter Text...              │   ← QTextEdit (Text Input)
│                              │
├─────────────────────────────┤
│           [ SWAP ]           │   ← Converts & swaps content
├─────────────────────────────┤
│                              │
│   Enter Binary...            │   ← QTextEdit (Binary Output)
│                              │
├──────────────┬──────────────┤
│   [ RESET ]  │   [ COPY ]   │   ← Action buttons
└──────────────┴──────────────┘
```

---

## 🚀 Getting Started

### Prerequisites

- Python 3.x installed on your system
- `pip` available in your environment

### Installation

**1. Clone this repository**
```bash
git clone https://github.com/mebdulrafay/BINARY-APP.git
cd BINARY-APP
```

**2. Install PyQt5**
```bash
pip install PyQt5
```

**3. Run the application**
```bash
python "BINARY APP CODE"
```

> ✅ No other dependencies — just Python and PyQt5!

### Quick Usage

```
1. Type any text into the top field
2. Press  [ SWAP ]  to convert it to binary
3. Press  [ COPY ]  to copy the binary to your clipboard
4. Press  [ RESET ] to clear both fields and start fresh

OR

1. Paste binary code into the bottom field
2. Press  [ SWAP ]  to decode it back into readable text
```

---

## ⚙️ Configuration

### Theme Customization

Colors are defined as constants at the top of the source file — easy to tweak:

```python
BACKGROUND_COLOR   = "#1a1a1a"   # Main window background
WIDGET_BG_COLOR    = "#2a2a2a"   # Text area background
TEXT_COLOR         = "#ffffff"   # All text
BUTTON_COLOR       = "#0d7dff"   # Button fill (accent)
BUTTON_HOVER_COLOR = "#1e8fff"   # Button hover state
BORDER_COLOR       = "#3a3a3a"   # Widget borders
```

### Window Sizing

The app launches at **400 × 650 px** with a minimum of **400 × 600 px**. Adjust in `init_ui()`:

```python
self.setMinimumSize(400, 600)
self.resize(400, 650)
```

---

## 👨‍💻 About the Author

<div align="center">

| Field | Detail |
|:---:|:---|
| **Name** | Hafiz Abdul Rafay |
| **Role** | Student • AI-Assisted Web Developer • Freelancer |
| **Location** | 📍 Mianwali, Pakistan |
| **Achievement** | 🏆 2nd Place — Science Expo 2025, PAEC Education Center (Level VI–VIII) |
| **Certification** | 🎓 HP LIFE Certified — AI's Business Impact & Ethics |

</div>

### 🤝 Connect with Abdul Rafay

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-mebdulrafay-181717?style=for-the-badge&logo=github)](https://github.com/mebdulrafay)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/hafiz-abdul-rafay-4577a5395/)
[![Email](https://img.shields.io/badge/Email-Say%20Hello!-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:mebdulrafay@gmail.com)

</div>

---

### 📌 Full Project Portfolio

| Project | Stack | Description |
|:---|:---|:---|
| 🎯 **Radar System** | Arduino • Ultrasonic Sensor | Object detection with AI voice alerts & real-time distance feedback |
| 🌦 **Weather Forecast App** | HTML/CSS/JS • OpenWeather API | Responsive live weather app with dynamic UI |
| 🔢 **Binary X** | Python • PyQt5 | *This project* — Desktop app for text-to-binary conversion |
| 🔔 **PC-Controlled Buzzer** | Arduino • Serial Comm | Hardware alert system controlled via PC |
| 🌐 **Personal Portfolio** | HTML/CSS/JS • Glassmorphism | Premium interactive site showcasing all digital & hardware projects |
| 🤖 **ROEX AI Assistant** | n8n • Gemini • LangChain | AI-powered portfolio representative with memory & GitHub integration |

---

### 💼 Freelancing Services

| Service | Description |
|:---|:---|
| 🌐 Modern Web Development | Responsive & premium UI/UX with glassmorphism aesthetics |
| 🤖 AI-Assisted Development | Faster turnaround using AI-powered n8n workflows |
| ⚡ Arduino & IoT Prototyping | Sensor integration, serial comms, and hardware projects |
| 🎨 Graphic Design & Branding | Social media creatives, logos, and visual identity |

> 📬 Interested in working together? Reach out at **mebdulrafay@gmail.com**

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0a1628,50:0d3b2e,100:051a10&height=100&section=footer" width="100%"/>

**Made with 💚 by [Hafiz Abdul Rafay](https://github.com/mebdulrafay) — Mianwali, Pakistan**

*"Specializing in elegant solutions that combine beautiful design with powerful functionality."*

⭐ **Star this repo if Binary X made your day a little more digital!**

</div>

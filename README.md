<div align="center">

  <!-- Dynamic Waving Header Banner -->
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,40:161b22,100:238636&height=250&section=header&text=CHHUN%20LONG&fontSize=48&fontColor=ffffff&animation=twinkling&desc=R%26D%20Engineer%20%7C%20Electronics%20%26%20Embedded%20Systems&descSize=20&descAlignY=62" width="100%" alt="Header Banner" />

  <!-- Animated Typing SVG -->
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&pause=1000&color=238636&center=true&vCenter=true&width=700&lines=From+schematic+to+shipped+product+%F0%9F%9A%80;Multi-Layer+PCB+Layout+%26+JLCPCB+Stackups;Embedded+Firmware+(ESP32-S3%2C+STM32%2C+PIC);IoT+Device+Design+%26+KHQR+Payment+Soundboxes;SolidWorks+3D+CAD+%26+Bambu+Lab+A1+3D+Printing;Solar+Pump+Controllers+%26+Industrial+Automation" alt="Typing SVG" />
  </a>

  <p align="center">
    📍 <b>Phnom Penh, Cambodia 🇰🇭</b> | 🎓 <b>B.S. Telecommunication & Electronic Engineering (RUPP)</b>
  </p>

  <p align="center">
    <a href="https://github.com/CHHUNLONGKH?tab=followers">
      <img src="https://img.shields.io/github/followers/CHHUNLONGKH?label=Followers&style=for-the-badge&color=238636&logo=github" alt="Followers" />
    </a>
    <img src="https://img.shields.io/badge/Focus-Embedded%20%26%20IoT-blue?style=for-the-badge&logo=microchip" alt="Focus" />
    <img src="https://img.shields.io/badge/Status-Building%20Hardware-orange?style=for-the-badge&logo=powershell" alt="Status" />
    <img src="https://img.shields.io/badge/Open%20to-Collaboration-success?style=for-the-badge" alt="Open to collaboration" />
  </p>

  <!-- Language switcher -->
  <p align="center">
    🌐 <b>English</b> | <a href="https://github.com/CHHUNLONGKH/CHHUNLONGKH/blob/main/README.km.md">ភាសាខ្មែរ</a>
  </p>

  <!-- Quick navigation -->
  <p align="center">
    <a href="#-workflow">Workflow</a> •
    <a href="#-featured-projects">Projects</a> •
    <a href="#-engineering-notebook">Notebook</a> •
    <a href="#-skill-map">Skills</a> •
    <a href="#-github-activity">Activity</a> •
    <a href="#-lets-build-something">Contact</a>
  </p>

</div>

---

# Hi there, I'm Chhun Long 👋

> **"I don't just design circuits, I take an idea all the way from schematic to a box on a shop counter."**

I'm an **R&D Engineer** building real hardware for real businesses in Cambodia: PCB, firmware, enclosure, and cloud connection, all in one loop. 🔁

<table>
<tr>
<td width="50%" valign="top">

### 🧭 Right now
- 🔭 **Building:** KHQR payment notification hardware, smart displays, custom ESP32-S3 IoT modules
- 🌱 **Learning:** tighter impedance control, RTOS patterns, faster prototype → production cycles
- 💬 **Ask me about:** KiCad 6-layer stackups, C/C++ firmware, SolidWorks, MQTT & HTTP APIs
- 📫 **Reach me:** [Telegram @CHHUNLONGKH](https://t.me/CHHUNLONGKH)

</td>
<td width="50%" valign="top">

### 🪪 Quick facts
- 🎓 B.S. Telecom & Electronic Eng. (RUPP)
- 📍 Phnom Penh, Cambodia 🇰🇭
- 🧰 Runs **EC STORE**, a tools & electronics shop
- 🎥 Shares builds on YouTube & TikTok
- 🖨️ Every enclosure is printed in-house on a Bambu Lab A1
- ☕ Fueled by coffee and solder fumes

</td>
</tr>
</table>

---

## 🔄 Workflow

```mermaid
flowchart LR
    A[💡 Idea / Client Need] --> B[📐 Schematic<br/>KiCad]
    B --> C[🔌 PCB Layout<br/>4 / 6-layer]
    C --> D[🏭 JLCPCB + LCSC<br/>Fab & Parts]
    B --> E[📦 Enclosure<br/>SolidWorks]
    E --> F[🖨️ Bambu Lab A1<br/>Print]
    D --> G[⚙️ Firmware<br/>ESP32-S3 / STM32 / PIC]
    F --> H[🚀 Assemble & Test]
    G --> H
    H --> I[🏪 Deployed in the field]
    I -. feedback .-> A
```

---

## 🚀 Featured Projects

### 🔊 KHQR Smart Soundbox & Display
Instant audio + LCD feedback the moment a KHQR payment lands. Deployed with **Mr. Laundry** and **Easy Laundry**.

```mermaid
sequenceDiagram
    participant C as 👤 Customer
    participant B as 🏦 Bank / KHQR
    participant S as ☁️ Server
    participant D as 🔊 Soundbox (ESP32-S3)
    C->>B: Scan & pay
    B->>S: Payment confirmed
    S->>D: MQTT / HTTP notification
    D-->>C: 🔔 Voice announcement + LCD amount
```

<details>
<summary><b>🧩 Device architecture (click to expand)</b></summary>

```mermaid
graph TD
    PWR[🔋 Power In<br/>USB-C / DC] --> REG[Regulators]
    REG --> MCU[ESP32-S3]
    MCU -- Wi-Fi --> CLOUD[☁️ MQTT / HTTP]
    MCU -- I2S / DAC --> AMP[🔊 Audio Amp] --> SPK[Speaker]
    MCU -- SPI / I2C --> LCD[🖥️ Display]
    MCU -- GPIO --> UI[Buttons / LEDs]
```

| | |
|---|---|
| **Hardware** | ESP32-S3, audio amp, LCD, custom PCB |
| **Connectivity** | MQTT · HTTP API · Wi-Fi |
| **Mechanical** | SolidWorks enclosure, 3D printed |

</details>

### 🔌 High-Density PCB Layouts
- 4-layer and 6-layer boards in **KiCad** with defined net classes
- Trace impedance tuning against **JLCPCB stackups**
- Component sourcing through **LCSC** for fast, low-cost production runs

### ⚙️ Firmware Across the MCU Spectrum

| MCU | Style | Typical use |
|---|---|---|
| **ESP32-S3** | RTOS + networking | IoT, displays, soundboxes |
| **STM32** | Low-level C/C++ | Control & peripherals |
| **PIC12F1822** | Tiny & efficient | Simple, cost-sensitive logic |

### ☀️ Solar Power Automation
Industrial **solar motor pump controllers** and inverter configuration for **380V, 10HP** systems, where hardware really has to be reliable.

---

## 📓 Engineering Notebook

Small, practical things I've learned building hardware. Click to expand.

<details>
<summary><b>✅ My pre-fab PCB checklist</b></summary>

- [ ] DRC and ERC clean, with no ignored warnings
- [ ] Net classes set (power, signal, high-speed) with correct widths and clearances
- [ ] Stackup matches the fab's real capabilities (JLCPCB layer stack and impedance table)
- [ ] Decoupling caps placed right at the MCU power pins
- [ ] Continuous ground reference under fast signals
- [ ] Antenna keep-out respected on ESP32 modules
- [ ] Every part checked against LCSC stock and footprint
- [ ] Silkscreen: polarity, pin 1, test points, and version number
- [ ] 3D view checked against the SolidWorks enclosure

</details>

<details>
<summary><b>💻 Firmware pattern I like for IoT (ESP32 + MQTT)</b></summary>

A minimal sketch of the idea: keep the callback tiny, and push work to a queue so audio and display tasks never block the network stack.

```cpp
#include <WiFi.h>
#include <PubSubClient.h>

QueueHandle_t paymentQueue;

void onMessage(char* topic, byte* payload, unsigned int len) {
  // Keep it short: copy and hand off, don't process here.
  char msg[64] = {0};
  memcpy(msg, payload, min(len, sizeof(msg) - 1));
  xQueueSend(paymentQueue, msg, 0);
}

void audioTask(void*) {
  char msg[64];
  for (;;) {
    if (xQueueReceive(paymentQueue, msg, portMAX_DELAY)) {
      // parse amount -> update LCD -> play voice clips
    }
  }
}
```

</details>

<details>
<summary><b>🖨️ Print-to-fit enclosure tips</b></summary>

- Print a fast test fit before finalizing the design
- Add 0.2 to 0.3 mm clearance for snap-fits and PCB slots
- Model screw bosses from the actual PCB hole positions (export from KiCad)
- Keep speaker grilles and antenna areas free of thick walls

</details>

---

## 🎯 Skill Map

| Area | Level |
|---|---|
| PCB Design (KiCad) | ![](https://geps.dev/progress/90?dangerColor=238636&warningColor=238636&successColor=238636) |
| Embedded C/C++ | ![](https://geps.dev/progress/88?dangerColor=238636&warningColor=238636&successColor=238636) |
| IoT Protocols (MQTT/HTTP) | ![](https://geps.dev/progress/80?dangerColor=238636&warningColor=238636&successColor=238636) |
| 3D CAD (SolidWorks) | ![](https://geps.dev/progress/82?dangerColor=238636&warningColor=238636&successColor=238636) |
| Additive Manufacturing | ![](https://geps.dev/progress/85?dangerColor=238636&warningColor=238636&successColor=238636) |
| Power / Solar Automation | ![](https://geps.dev/progress/75?dangerColor=238636&warningColor=238636&successColor=238636) |

### 🛠️ Hardware & Technical Stack

**PCB & CAD / 3D Modeling**

![KiCad](https://img.shields.io/badge/KiCad-314159?style=for-the-badge&logo=kicad&logoColor=white)
![SolidWorks](https://img.shields.io/badge/SolidWorks-DC3545?style=for-the-badge&logo=dassaultsystemes&logoColor=white)
![Bambu Lab](https://img.shields.io/badge/Bambu_Lab_A1-00A859?style=for-the-badge&logo=3d&logoColor=white)
![JLCPCB](https://img.shields.io/badge/JLCPCB-00599C?style=for-the-badge&logo=pcb&logoColor=white)

**Firmware & Languages**

![C](https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![PlatformIO](https://img.shields.io/badge/PlatformIO-F6821F?style=for-the-badge&logo=platformio&logoColor=white)

**Microcontrollers & Hardware**

![ESP32](https://img.shields.io/badge/ESP32--S3-E7352C?style=for-the-badge&logo=espressif&logoColor=white)
![STM32](https://img.shields.io/badge/STM32-03234C?style=for-the-badge&logo=stmicroelectronics&logoColor=white)
![Microchip PIC](https://img.shields.io/badge/PIC_MCU-003366?style=for-the-badge&logo=microchip&logoColor=white)

**Communication Protocols & Tools**

![MQTT](https://img.shields.io/badge/MQTT-660099?style=for-the-badge&logo=hivemq&logoColor=white)
![HTTP API](https://img.shields.io/badge/HTTP_API-008080?style=for-the-badge&logo=postman&logoColor=white)
![UART / SPI / I2C](https://img.shields.io/badge/Serial-UART%20%7C%20SPI%20%7C%20I2C-black?style=for-the-badge)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

---

## 🧭 Roadmap

- [x] KHQR soundbox deployed to real shops
- [x] 6-layer KiCad boards in production via JLCPCB
- [ ] Open-source a reference KHQR soundbox design
- [ ] OTA firmware updates across all devices
- [ ] Battery + low-power soundbox variant
- [ ] More build videos on YouTube & TikTok

<sub>Edit this list to match your real plans.</sub>

---

## 📊 GitHub Activity

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=CHHUNLONGKH&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="GitHub Stats" width="48%" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=CHHUNLONGKH&layout=compact&theme=tokyonight&hide_border=true" alt="Top Languages" width="48%" />
</div>

<br />

<div align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=CHHUNLONGKH&theme=tokyonight&hide_border=true" width="97%" alt="Streak Stats" />
</div>

<br />

<div align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=CHHUNLONGKH&theme=tokyo-night&hide_border=true&area=true" width="97%" alt="Activity Graph" />
</div>

<br />

<div align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=CHHUNLONGKH&theme=onedark&no-frame=true&no-bg=true&margin-w=8&row=1&column=7" alt="Trophies" />
</div>

<br />

<!-- Contribution snake: needs the workflow in .github/workflows/snake.yml (repo must be CHHUNLONGKH/CHHUNLONGKH) -->
<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/CHHUNLONGKH/CHHUNLONGKH/output/github-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/CHHUNLONGKH/CHHUNLONGKH/output/github-snake.svg" />
    <img alt="Contribution snake" src="https://raw.githubusercontent.com/CHHUNLONGKH/CHHUNLONGKH/output/github-snake.svg" />
  </picture>
</div>

<!-- Pinned repo cards: uncomment and put in your real repo names
<div align="center">
  <a href="https://github.com/CHHUNLONGKH/REPO_NAME"><img src="https://github-readme-stats.vercel.app/api/pin/?username=CHHUNLONGKH&repo=REPO_NAME&theme=tokyonight&hide_border=true" /></a>
</div>
-->

---

## 🤝 Let's Build Something

Got an IoT idea, a payment device, a custom PCB, or a controller that needs to survive real-world conditions? Message me on Telegram. Let's turn it into hardware. ⚡

<div align="center">

[<img src="https://img.shields.io/badge/Message_me_on_Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white" />](https://t.me/CHHUNLONGKH)

</div>

## 🌐 Connect & Follow

<div align="center">

[<img src="https://img.shields.io/badge/Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white" />](https://t.me/CHHUNLONGKH)
[<img src="https://img.shields.io/badge/GrabCAD-000000?style=for-the-badge&logo=grabcad&logoColor=white" />](https://grabcad.com/chhun.long.chay-1)
[<img src="https://img.shields.io/badge/Facebook_Profile-1877F2?style=for-the-badge&logo=facebook&logoColor=white" />](https://www.facebook.com/Chhunlongkh44)
[<img src="https://img.shields.io/badge/EC_STORE-1877F2?style=for-the-badge&logo=facebook&logoColor=white" />](https://www.facebook.com/ECSTORE.TOOLS/)
[<img src="https://img.shields.io/badge/TikTok-000000?style=for-the-badge&logo=tiktok&logoColor=white" />](https://www.tiktok.com/@chhunlongkh?lang=en)
[<img src="https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white" />](https://www.youtube.com/channel/UCtKbRAz7CkX35r7EZQbLT5w)
[<img src="https://img.shields.io/badge/Blog-FF5722?style=for-the-badge&logo=blogger&logoColor=white" />](https://chhunlonchay44.blogspot.com/)

</div>

---

<div align="center">
  <img src="https://quotes-github-readme.vercel.app/api?type=horizontal&theme=tokyonight" alt="Random quote" />
  <br /><br />
  <img src="https://komarev.com/ghpvc/?username=CHHUNLONGKH&color=238636&style=flat-square&label=PROFILE+VIEWS" alt="Profile Views" />
  <br />
  <sub>⚡ Made with solder fumes, coffee, and a lot of prototypes ⚡</sub>
</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,40:161b22,100:238636&height=120&section=footer" width="100%" alt="Footer" />

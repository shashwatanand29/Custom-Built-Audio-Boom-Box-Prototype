# 🔊 Custom Built 2.1 Bluetooth Boom Box

> 📅 **Started: November 2024 | Current Version: V2**

A custom-built portable **2.1-channel Bluetooth boom box** developed through multiple hardware iterations. The project combines audio electronics, lithium-ion battery technology, power management, soldering, speaker integration, and hands-on enclosure fabrication.

The project began as a **cardboard prototype (V1)** and was later upgraded to **Version 2**, using a reclaimed Philips shelf-speaker enclosure for a more rigid and acoustically capable build.

---

## 🎯 Project Highlights

- 🔊 Fully functional **2.1-channel portable audio system**
- 📱 **Bluetooth audio** connectivity
- 🎧 **AUX input** for wired audio sources
- 🔋 Custom **6S 18650 Li-ion battery pack**
- 🛡️ **6S 15A BMS** for battery protection
- ⚡ **25.5V DC charging** through an external **XT60 connector**
- 📟 Real-time battery **voltage and current monitoring**
- 🔋 Integrated battery-level indicator
- 🎚️ Dedicated audio controls
- 🪵 V2 built using a **reclaimed Philips shelf-speaker enclosure**
- 🔇 Internal acoustic damping
- 🧰 Hand-built and soldered internal wiring

---

# 🚀 Version History

## V1 — Original Cardboard Prototype

The project was initially built in **November 2024** using a cardboard enclosure.

The purpose of V1 was to validate the complete electrical and audio system before investing time into a more permanent enclosure.

### V1 included:

- TPA3116D2 2.1-channel amplifier
- Bluetooth audio
- 2 × Sony stereo drivers
- Dedicated subwoofer
- 6S 18650 battery pack
- 6S 15A BMS
- 25.5V DC charging
- Digital voltage/current monitoring
- Hand-soldered internal wiring
- Cardboard enclosure

Although the cardboard enclosure was useful for rapid prototyping, it was not ideal for structural rigidity or acoustic performance.

---

# 🆕 V2 — Enclosure & Connectivity Upgrade

Version 2 focuses primarily on improving the **physical construction, acoustics, and connectivity** of the original prototype.

The electronics architecture and core audio system were retained, while the cardboard enclosure was replaced with a **reclaimed Philips shelf-speaker enclosure**.

### Major V2 Changes

| Feature | V1 | V2 |
|---|---|---|
| 🪵 Enclosure | Cardboard | Reclaimed Philips shelf-speaker enclosure |
| 🔊 Speaker mounting | Prototype mounting | Improved rigid enclosure mounting |
| 🔇 Acoustic treatment | Basic | Internal damping material |
| 🔌 Charging connector | Basic DC input | **XT60 connector** |
| 🎧 AUX input | Available | **Retained / integrated** |
| 🔋 Battery | 6S 18650 | 6S 18650 |
| 🛡️ BMS | 6S 15A | 6S 15A |
| ⚡ Charging | 25.5V DC | 25.5V DC |
| 📟 Voltage monitoring | Yes | Yes |
| 📟 Current monitoring | Yes | Yes |
| 🔋 Battery indicator | Yes | Yes |
| 🔊 Amplifier | TPA3116D2 2.1 | TPA3116D2 2.1 |
| 📱 Bluetooth | Yes | Yes |
| 🧰 Construction | Rapid prototype | Rebuilt enclosure |
| 🎵 Sound quality | Prototype-level | **Improved due to enclosure upgrade** |

### What V2 Improved

The biggest improvement in V2 is the **enclosure**.

The original cardboard cabinet was replaced with a rigid wooden Philips speaker enclosure, providing a substantially better platform for the drivers and reducing the limitations of the original temporary construction.

The enclosure was also fitted with internal acoustic damping material to help control internal reflections and resonance.

An **XT60 connector** was added as the dedicated external charging connection, providing a more robust and practical charging interface.

The **AUX input** was retained so the speaker can be used with both wireless Bluetooth sources and wired audio sources.

---

# 🔧 Hardware Specifications

| Component | Details |
|---|---|
| 🔉 **Amplifier** | TPA3116D2 2.1-channel amplifier |
| 🔊 **Stereo Speakers** | 2 × Sony XS-FB102E |
| 🔊 **Subwoofer** | Dedicated subwoofer driver |
| 📱 **Wireless Input** | Bluetooth |
| 🎧 **Wired Input** | AUX |
| 🔋 **Battery** | 6 × 18650 Li-ion cells |
| 🔋 **Battery Configuration** | 6S |
| 🛡️ **Battery Protection** | 6S 15A BMS |
| ⚡ **Charging Voltage** | 25.5V DC |
| 🔌 **Charging Connector** | XT60 |
| 📟 **Monitoring** | Digital voltage & current meter |
| 🔋 **Battery Status** | LED battery-level indicator |
| 🪵 **V1 Enclosure** | Cardboard |
| 🪵 **V2 Enclosure** | Reclaimed Philips shelf-speaker cabinet |
| 🔇 **Acoustic Treatment** | Internal damping material |

---

# ⚙️ System Architecture

```text
                     ┌─────────────────────┐
                     │   Bluetooth / AUX    │
                     │     Audio Input      │
                     └──────────┬──────────┘
                                │
                                ▼
                     ┌─────────────────────┐
                     │     TPA3116D2       │
                     │   2.1 Ch Amplifier  │
                     └──────┬────────┬─────┘
                            │        │
                       L + R │        │ Sub
                            ▼        ▼
                       ┌────────┐ ┌──────────┐
                       │ Stereo │ │Subwoofer │
                       │Drivers │ │  Driver  │
                       └────────┘ └──────────┘


                 ┌──────────────────────┐
                 │ 6S 18650 Battery     │
                 │      Pack            │
                 └──────────┬───────────┘
                            │
                            ▼
                     ┌─────────────┐
                     │  6S 15A BMS │
                     └──────┬──────┘
                            │
             ┌──────────────┼──────────────┐
             │              │              │
             ▼              ▼              ▼
        Amplifier      V/A Meter     Battery Indicator


        25.5V DC Charger
               │
               ▼
          ┌─────────┐
          │  XT60   │
          │ Charging│
          │  Input  │
          └─────────┘

## 🛠️ Assembly Overview

1. **Battery Pack**: 6x 18650 cells configured in 6S, protected by a 15A BMS.
2. **Wiring**: Manual soldering and cable routing for speakers, meters, amplifier, and power.
3. **Audio Section**: Subwoofer and stereo channels connected to TPA3116D2 amp board.
4. **Monitoring**: Digital voltmeter/ammeter mounted on face panel.
5. **Power Input**: External 25.5V SMPS connected through dedicated charging port.
6. **Enclosure**: Temporary build in cardboard; MDF version in future revision.

---

## 📸 Project Media

<table>
  <tr>
    <td><img src="Custom_Built_Audio_Boom_Box.jpg" width="300"/></td>
    <td><img src="Custom_Built_Audio_Boom_Box_Charging_Monitor.jpg" width="300"/></td>
  </tr>
  <tr>
    <td><img src="Custom_Built_Audio_Boom_Box_Battery_Pack.jpg" width="300"/></td>
    <td><img src="Custom_Built_Audio_Boom_Box_BMS.jpg" width="300"/></td>
  </tr>
  <tr>
    <td><img src="Custom_Built_Audio_Boom_Box_Inside.jpg" width="300"/></td>
    <td><img src="Custom_Built_Audio_Boom_Box_Back.jpg" width="300"/></td>
  </tr>
</table>



---

## 🚀 Future Improvements

- CNC-cut MDF or wooden enclosure with acoustic tuning

---

## 👨‍💻 Author

**Shashwat**  
[GitHub](https://github.com/shashwatanand29) | [LinkedIn](https://www.linkedin.com/in/shashwat-anand-b85509209/)

---


## 🎥 Demo Video 

📽️ [Watch Video on Google Drive](https://drive.google.com/file/d/1lwp948RQFKhyJF6PXhbXN4GmUYBBxtbc/view?usp=sharing)
---
🖼️ [More Photos on Google Drive](https://drive.google.com/drive/folders/1TNvkKNu4axBeoHTYECP6J2ObiK9xANx6?usp=drive_link)


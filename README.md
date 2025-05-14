# AM Receiver – Final Project Report  
**Course:** ELE402 – Electronics Lab  
**Instructor:** Mr. Chadi T. Chamoun  
**University:** Lebanese American University  
**Date:** 11 May 2025  

## 👥 Team Members
- Ali Awada – 202300797  
- Malak Darwich – 202304438  
- Dana Hachem – 202300964  
- Mahdi Zein Al Dine – 202300041  

---

## 📡 Project Overview
This project involved the design, simulation, and hardware implementation of a complete **Amplitude Modulation (AM) Receiver**, structured into three functional stages:

1. **Passive Demodulator** – Extracts the baseband audio signal using envelope detection with a germanium diode and an RC low-pass filter.
2. **Baseband Amplifier** – A non-inverting op-amp amplifier with adjustable gain to boost the demodulated signal.
3. **Class A Output Stage** – A high-current BJT amplifier designed to drive an 8Ω speaker with sufficient power.

Each stage was simulated using **LTspice**, then physically implemented and tested on a **breadboard** and later **soldered onto a perforated board**.

---

## 🔧 Components Used
| Component           | Model/Value   | Quantity |
|--------------------|---------------|----------|
| Resistors          | 1kΩ, 510Ω, 130Ω, etc. | Multiple |
| Capacitors         | 1μF, 22μF, 1.8nF       | Multiple |
| Diode              | OA71 (germanium)      | 1        |
| Transistors        | BC337                 | 12       |
| Op-Amp             | TL084                 | 1        |
| Speaker            | 8Ω                    | 1        |
| Breadboard, wires, IC sockets, etc. | — | — |

*Full bill of materials with prices is included in the report.*

---

## 🔬 Simulation and Testing
Simulations were carried out using **LTspice** for:
- Signal demodulation
- Frequency response & gain analysis
- Output waveform behavior at various frequencies

Hardware tests included:
- Oscilloscope visualization of input/output signals
- Audio playback via speaker for various tone frequencies
- Gain calibration using voltage divider and potentiometer
- Thermal analysis and heat dissipation management

---

## ⚙️ Key Features
- Envelope detection using a germanium diode (low forward voltage drop)
- Adjustable gain via potentiometer for volume control
- Parallel BJTs in output stage to handle high current
- Smoothing filters and voltage dividers for optimal stage integration
- Oscilloscope-verified signal integrity across all stages

---

## 🧪 Challenges Faced
- High diode forward voltage caused signal clipping → solved by switching to OA71
- Excessive gain in baseband amp → solved with input voltage divider
- Overheating resistors in Class A stage → solved with resistor power rating adjustments
- Transistor overheating → solved by using multiple BJTs in parallel
- Soldering errors → resolved with continuity testing and careful debugging

---

## 📉 Limitations
- Low speaker volume at times
- Limited frequency response above 10kHz
- Significant power consumption in output stage
- Heat buildup during extended operation

---

## ✅ Conclusion
This project successfully demonstrated the design and implementation of a working analog AM receiver. Each stage was theoretically analyzed, simulated, constructed, and tested. The final system was able to clearly demodulate and play AM-modulated audio signals. The project provided deep hands-on experience in analog circuit design, troubleshooting, and communication systems.

---

## 📁 Files Included
- `AM_Demodulator.asc` – LTspice simulation
- `Baseband_Amplifier.asc`
- `ClassA_Output_Stage.asc`
- `AM_Receiver.asc`
- `FinalReport.pdf` – Full technical report (if exported as PDF)
- `README.md`

---

## 📚 References
- GeeksForGeeks: Amplitude Modulation Explained  
- Vedantu: Why AM is used for long-distance communication  
- ELE402 Course Materials and SPICE models

---

> 🔧 Built with analog components, teamwork, and lots of oscilloscope debugging!

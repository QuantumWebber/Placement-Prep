<p>Very useful video https://youtu.be/SCrt9sdULhw?si=EZLnPP-uTKRLq1Er</p>


# Texas Instruments — Analog Role Interview Prep

Curated resources + practice questions for **Analog Design / Analog Applications / Field Applications Engineer** roles at TI (and similar: ADI, NXP, Infineon, Qualcomm Analog, Cadence, Synopsys AMS).

> Format: every topic has **(a) what to read**, **(b) what to practice**. Tick the boxes as you go.

---

## 0. Round Structure (what to expect)

| Round | Focus |
|---|---|
| Online Test | Aptitude + Analog/Digital MCQs + basic C |
| Tech Round 1 | Device physics, MOSFET/BJT, small-signal, op-amp |
| Tech Round 2 | Feedback & stability, bandgap, LDO/DC-DC, ADC, noise |
| Tech Round 3 | Circuit puzzles on paper, layout awareness, projects deep-dive |
| HR / Managerial | Projects, why analog, why TI |

Analog interviews are **derivation-heavy**. Expect: "draw the circuit, write the small-signal model, derive the transfer function, tell me the pole locations."

---

## 1. Core Resources

### Books (the standard set)
- **Behzad Razavi — *Fundamentals of Microelectronics*** → start here if you're rusty.
- **Behzad Razavi — *Design of Analog CMOS Integrated Circuits*** → the single most interview-relevant book. Ch. 2–6, 8, 9, 10, 11.
- **Sedra & Smith — *Microelectronic Circuits*** → best for BJT and op-amp fundamentals.
- **Gray, Hurst, Lewis, Meyer — *Analysis and Design of Analog ICs*** → noise & bandgap chapters.
- **Baker — *CMOS: Circuit Design, Layout, and Simulation*** → layout, matching, mixed-signal.
- **Johns & Martin — *Analog Integrated Circuit Design*** → data converters.
- **Sergio Franco — *Design with Op Amps and Analog ICs*** → best for **applications** roles (board-level).

### Video Lectures
- Razavi's own lecture series (UCLA, on YouTube) — Fundamentals of Microelectronics + Advanced Analog IC Design.
- NPTEL: *Analog IC Design* (Prof. Nagendra Krishnapura, IITM) — closest to Indian interview style.
- NPTEL: *Analog Circuits* (Prof. Jayanta Mukherjee, IITB).
- NPTEL: *Switched Mode Power Conversion* (Prof. V. Ramanarayanan, IISc) — for power roles.

### TI's Own Material (huge advantage — interviewers wrote these)
- **TI Precision Labs** — op-amps, ADCs, amplifiers, magnetic sensing. Free, short videos + exercises. Mention it in the interview.
- **TI Analog Engineer's Pocket Reference** (free PDF) — formulas, conversions, PCB rules.
- **TI Analog Engineer's Circuit Cookbook: Op Amps / ADCs** (free PDF) — 60+ solved sub-circuits with design steps. Excellent practice source.
- **TI Application Notes**: AN-31 (op-amp circuit collection), "Op Amps for Everyone" (Ron Mancini), "Noise Analysis in Operational Amplifier Circuits".
- **TINA-TI / PSpice for TI / WEBENCH** — free simulators. Simulate every practice circuit below.

### Practice Question Banks
- Razavi end-of-chapter problems (Ch. 3–11 of *Analog CMOS*).
- GATE EC/IN — Analog Circuits + Electronic Devices previous year papers (2000–present). Very close to TI's written test.
- ISRO/BARC electronics papers for extra MCQ volume.
- *Analog Circuit Design Interview Questions* compilations on GitHub — good for rapid-fire revision.

### Tools to know
LTspice / TINA-TI / Cadence Virtuoso · MATLAB / Python for control-loop plots · basic lab: oscilloscope, function generator, bode plotting.

---


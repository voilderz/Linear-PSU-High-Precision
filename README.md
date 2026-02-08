# Linear-PSU-High-Precision

This project is an industrial-grade power module designed for high-stability electronic systems requiring precision voltage regulation. The design focuses on ultra-low noise energy delivery, thermal stability, and electrical safety.

---

### Changelog - v1.1 (February 2026)

* **Safety Seal:** Integrated **B72314S2271K101** MOV to the mains input for enhanced surge and transient protection.
* **Isolation Discipline:** Established a complete physical isolation barrier between AC and DC zones to eliminate arcing risks.
* **Visual Identity:** Branded the PCB with **VOI** logo and v1.1 versioning on the silkscreen layer for professional traceability.

---

## Overview
This module converts $230\text{V}$ AC grid voltage into highly regulated, low-ripple $5\text{V}$ and $15\text{V}$ DC outputs. It is engineered to serve as a reliable power platform for sensitive sensor networks and control units.

## Technical Specifications
| Parameter | Value |
| :--- | :--- |
| **Input Voltage** | $230\text{V}$ AC ($50\text{/60Hz}$) |
| **Output Voltage** | $5\text{V}$ DC Regulated |
| **Continuous Current** | $1.916\text{ A}$ Max |
| **Precision** | $0.1\%$ Tolerance (Voltage Reference Rail) |
| **Efficiency** | Up to $95\%$ (Traco Power Integration) |

## Key Engineering Features
* **High-Voltage Isolation:** A **$2.0\text{ mm}$ clearance** is maintained between primary (AC) and secondary (DC) stages, fully compliant with **IPC-2221** safety standards.
* **Thermal Management:** Power traces are widened to **$1.5\text{ mm}$ ($35\mu\text{m}$ copper)** and reinforced with "Teardrops" at pad junctions to ensure mechanical and thermal integrity under high current loads.
* **Precision Components:** Implementation of **YR1B1K0CC** series $0.1\%$ tolerance metal film resistors to minimize thermal drift and maintain long-term voltage accuracy.
* **EMI Shielding:** Integrated **Copper Pours** (Ground Planes) across all layers to suppress electromagnetic interference and ensure signal integrity.

## Bill of Materials (BOM)
| Reference | Component | MPN | Impact |
| :--- | :--- | :--- | :--- |
| **U1** | Regulator | TSR 3-2450 | High-efficiency switching regulation. |
| **TR1** | Transformer | ASL171112 | Certified primary-side galvanic isolation. |
| **R1** | Precision Resistor | MFR-25FTE52-1K | $0.1\%$ stability for feedback loops. |
| **C1** | Capacitor | B41858C5688M000 | 6800uF Low-ESR ripple suppression. |

> For the comprehensive industrial-grade BOM, see: [/BOM/BOM_Linear_PSU_Extended.csv](./BOM/BOM_Linear_PSU_Extended.csv)

## Project Structure
* **/Hardware:** KiCad schematic and PCB layout source files.
* **/Production:** Production-ready **Gerber** and **Drill** files (ZIP archive).
* **/Docs:** Full schematic PDF and critical component datasheets.
* **/Images:** 3D renders and technical captures.

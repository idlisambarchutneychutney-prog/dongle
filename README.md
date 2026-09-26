# Dongle

<img width="783" height="591" alt="Screenshot 2026-09-05 211441" src="https://github.com/user-attachments/assets/f1eb03cd-d2d2-4927-ba47-1fa76fcd274f" />

A custom-designed, programmable USB dongle featuring a 9-LED grid, powered by the CH552G microcontroller. The board includes a user push-button and a USB connector.

## Features
* **Microcontroller:** CH552G 
* **Display:** 9x LEDs (D1-D9) with dedicated 330Ω resistors
* **Input:** 1x tactile push-button for user interaction
* **Custom Enclosure:** Includes a 3D-printable shell designed in Onshape

## Previews

### Schematic
<img width="272" height="617" alt="Screenshot 2026-09-05 210914" src="https://github.com/user-attachments/assets/abac358c-d36b-4c12-8ea8-f0845d32b604" />

### PCB Layout & Artwork
<img width="281" height="668" alt="Screenshot 2026-09-05 211006" src="https://github.com/user-attachments/assets/1f84a2ba-04f6-45d6-a5d3-1b8ea1b686b7" />
<img width="293" height="671" alt="Screenshot 2026-09-05 211028" src="https://github.com/user-attachments/assets/1da804c0-ca2a-4a6d-8dfe-0d03b5fb7e6c" />

### case
<img width="192" height="131" alt="Screenshot 2026-09-05 211410" src="https://github.com/user-attachments/assets/0571dcf7-e421-4e0c-88c9-8f074ddf8dc7" />

## Bill of Materials (BOM)

| Designator | Component Name | Value/Specs | Footprint | LCSC Part # | Notes / Sourcing |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **U1** | CH552G | 8-bit MCU, 16KB Flash | SOP-16 | `C111292` | Microcontroller |
| **C1, C2** | Ceramic Capacitor | 100nF (0.1uF) | 0603 | `C14663` | Decoupling Caps |
| **R1** | Resistor | 10kΩ | 0603 | `C25804` | Pull-up Resistor |
| **R2, R3, R4, R5, R6, R7, R8, R9, R10** | Resistor | 330Ω | 0603 | `C23138` | Current limiting for LEDs |
| **D1, D2, D3, D4, D5, D6, D7, D8, D9** | LED | Standard LED | 0805 | `C84256` | Indicator/Matrix LEDs |
| **J1** | USB Type-A Port | Male, 4-Pin, SMD | *See Footprint*| — | *Inventory Shortage* (Solder manually or substitute) |
| **SW1** | Tactile Switch | Push Button | *See Footprint*| — | *Inventory Shortage* (Solder manually or substitute) |

##  Manufacturing & Assembly
1. **PCB Fabrication:** Download the `.zip` file from the `/PCB` folder and upload it to your preferred PCB manufacturer. 
2. **Components:** All components are surface-mount (SMD) and located on the top layer to preserve the artwork on the back.
3. **3D Printing:** The enclosure can be printed in PLA, PETG, or ABS without supports. Use the `.step` file provided to slice the model in your preferred slicer.

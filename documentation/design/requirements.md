# Dual-Rail Embedded Power Supply

## 1. Overview

A compact two-layer DC power supply providing regulated 5 V and 3.3 V outputs from a 9–12 V DC input.

The design is intended for powering low-power embedded and digital electronics.

---

## 2. Electrical Specifications

| Parameter | Specification |
|---|---|
| Input voltage | 9–12 V DC |
| Nominal input | 12 V DC |
| 5 V output | 5.0 V ±5% |
| 5 V output current | ≥300 mA |
| 3.3 V output | 3.3 V ±5% |
| 3.3 V output current | ≥300 mA |
| PCB | 2-layer |
| PCB material | FR-4 |
| Mounting | Minimum 4 mounting holes |

Both output rails shall provide accessible VCC and GND connections.

---

## 3. Input

The input shall provide:

- A 2-pin screw terminal or DC barrel jack
- Clearly marked polarity
- Reverse-polarity protection
- Input overcurrent protection
- Appropriate input filtering and decoupling

---

## 4. Outputs

The board shall provide:

### +5 V Rail

- Nominal output: 5.0 V
- Regulation: ±5%
- Continuous output current: ≥300 mA

### +3.3 V Rail

- Nominal output: 3.3 V
- Regulation: ±5%
- Continuous output current: ≥300 mA

Output connectors shall be clearly labelled.

---

## 5. Power Conversion

The power-conversion architecture shall support generation of both regulated output rails from the 9–12 V input.

The selected topology shall satisfy the required:

- Output voltage
- Output current
- Efficiency
- Thermal performance
- Regulation
- Stability

Component selection and topology shall be supported by manufacturer datasheets and relevant application documentation.

---

## 6. Protection

The design shall include:

- Reverse-polarity protection
- Input overcurrent protection

The requirement for additional protection features such as transient, short-circuit, thermal, or overvoltage protection shall be evaluated based on the selected power architecture.

---

## 7. Decoupling and Filtering

Appropriate input and output capacitors shall be provided according to the requirements of the selected regulator(s).

Capacitor values, voltage ratings, package types, and placement shall comply with applicable manufacturer recommendations.

---

## 8. Indicators

The PCB shall include independent LED indicators for:

- Input power
- +5 V rail
- +3.3 V rail

LED current shall be appropriately limited.

---

## 9. Test Points

Dedicated test points shall be provided for:

- VIN
- GND
- +5 V
- +3.3 V

Test points shall be accessible for standard voltage and current measurements.

---

## 10. PCB Layout

The PCB shall use a two-layer copper stackup with an appropriate ground-plane strategy.

The layout shall consider:

- Power-current paths
- Ground-return paths
- Voltage drop
- Thermal dissipation
- Regulator-specific layout requirements
- Switching-current loops, where applicable
- Component clearances
- Connector accessibility

Critical power components shall be placed in accordance with the relevant manufacturer layout recommendations.

---

## 11. Design Rules

PCB design rules shall be selected according to the capabilities of the intended PCB fabrication process.

The design shall define appropriate:

- Minimum trace width
- Minimum clearance
- Via dimensions
- Drill sizes
- Copper-to-edge clearance

Power traces shall be sized according to expected current and acceptable electrical and thermal limits.

---

## 12. Component Selection

All components shall have appropriate:

- Voltage ratings
- Current ratings
- Power ratings
- Operating temperature ranges
- Package specifications

Critical component footprints shall be verified against the corresponding manufacturer datasheet.

The final BOM shall include:

- Reference designator
- Manufacturer
- Manufacturer part number
- Description
- Value
- Package
- Quantity

---

## 13. Verification

### Electrical Rules Check

The schematic shall undergo ERC.

All ERC violations shall be resolved or documented.

### Design Rules Check

The PCB shall undergo DRC.

All DRC violations shall be resolved or documented.

### Design Verification

The following shall be verified before finalizing the design:

- Regulator pin configuration
- Component values
- Component ratings
- Footprint dimensions and pin numbering
- Connector pinout
- Power connectivity
- Ground connectivity
- Decoupling implementation
- PCB clearances
- Mounting-hole clearances
- Silkscreen readability
- Manufacturing constraints

---

## 14. Documentation

The repository shall contain:

- KiCad schematic
- KiCad PCB layout
- Bill of Materials
- Schematic PDF
- PCB layout PDF
- 3D renders
- Design documentation

# OmniScroll

**OmniScroll** is an open-source, ultra-smooth desktop scroll wheel designed for precise CAD navigation, timeline scrub control, and high-speed document scrolling. 

By utilizing a large-diameter thin-section bearing and an off-axis magnetic rotary encoder, FluxDial achieves an effortless flywheel spin with zero axis wobble.

![FluxDial Banner](https://via.placeholder.com/1200x400?text=FluxDial+Desktop+Scroll+Wheel)

---

## Key Features

* **Flywheel Momentum:** Utilizes an `S6808` hybrid ceramic bearing ($40 \times 52 \times 7\text{ mm}$) stripped of grease for near-zero rotational resistance.
* **Magnetic Angle Sensing:** High-resolution rotary encoder (AS5600 / MA730) for smooth, non-contact position tracking.
* **Zero Axis Play:** Large-bore thin-section design houses internal electronics inside the hollow core, lowering the center of gravity and eliminating side-to-side wobble.
* **Custom Control Curves:** Configurable firmware supporting variable-speed scroll acceleration, granular scrub modes, and custom macro actions.

---

## Hardware Assembly

### Bill of Materials (BOM)

| Component | Specification / Part | Qty | Notes |
| :--- | :--- | :--- | :--- |
| **Main Bearing** | `S6808-2RS` Hybrid Ceramic ($40 \times 52 \times 7\text{ mm}$) | 1 | Degreased with IPA for maximum free-spin |
| **Magnetic Encoder** | AS5600 or MA730 PCB Module | 1 | Mounts coaxially inside the inner ring |
| **Diametral Magnet** | $6\text{ mm} \times 2.5\text{ mm}$ N35 (Diametrically Magnetized) | 1 | Fixed to the rotating outer knob shaft |
| **Microcontroller** | Raspberry Pi Pico / Seeed XIAO (RP2040) | 1 | Compact form factor fits inside housing base |
| **Enclosure** | 3D Printed (PLA/PETG) or Machined Aluminum | 1 | Files provided in `/cad` |

---

## Getting Started

### 1. Bearing Preparation
1. Carefully pop off the rubber seals (`2RS`) on the `S6808` bearing.
2. Submerge in isopropyl alcohol (IPA) and spin thoroughly to strip factory grease.
3. Blow dry with compressed air. (Optional: Apply 1 drop of high-speed instrument oil for quieter operation).

### 2. Firmware Setup
1. Clone this repository:
   ```bash
   git clone [https://github.com/your-username/FluxDial.git](https://github.com/your-username/FluxDial.git)

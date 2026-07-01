# Handheld-3D-Bioprinter
A modular, handheld 3D bioprinter featuring a mechanical stepper drivetrain and custom hydrogel extrusion system designed in OnShape.
# Modular Handheld 3D Bioprinter & Extrusion System

An open-source, modular handheld 3D bioprinting device engineered to precisely extrude multi-component bioinks while minimizing material waste. This repository contains the CAD models, drive train documentation, and system architecture for a handheld bioprinter that utilizes a mechanical stepper-driven extrusion mechanism to deposit specialized hydrogel matrices.

---

## 🔬 System Overview

This project bridges the gap between macro-scale tissue engineering and manual surgical application. By utilizing a compact, lightweight handheld form factor, this bioprinter allows for the direct, on-demand deposition of biocompatible scaffolds. 

### Key Technical Specifications:
* **Extrusion Mechanism:** Stepper motor-driven linear actuator drivetrain.
* **Control Electronics:** Breadboard-prototyped microcontroller interface with dedicated stepper drivers.
* **Chassis & Structure:** Custom modular components designed in OnShape and fabricated via precision FDM 3D printing.
* **Target Material Compatibility:** Multi-component shear-thinning and chemically crosslinkable hydrogels.

---

## 🧪 Bioink Formulation & Crosslinking Chemistry

The system is optimized for a custom, multi-component bioink formulation designed for mechanical stability, shear-thinning printability, and biocompatibility:

1. **Sodium Alginate:** The primary structural polysaccharide network, providing the base matrix for hydrogel formation.
2. **Calcium Chloride ($$\text{CaCl}_2$$):** Ionic crosslinking agent that reacts rapidly with sodium alginate to form a stable, insoluble hydrogel network.
3. **Xanthan Gum:** Actively modulates rheological properties, acting as a viscosity modifier to induce shear-thinning behavior (essential for smooth extrusion through fine-gauge nozzles).
4. **Tannic Acid:** Integrates natural polyphenolic crosslinking, enhancing antioxidant properties and tailoring mechanical stiffness.
5. **Genipin:** A naturally derived bi-functional crosslinker that covalently binds to amino groups, providing secondary long-term structural stabilization and reducing enzymatic degradation.

---

## 🛠️ Hardware & Structural Architecture

### 1. Mechanical Drivetrain
The extrusion system replaces traditional pneumatic pressure with a high-torque mechanical drive train to prevent material compression lag and ensure uniform volumetric flow rates:
* **Actuator:** High-precision NEMA stepper motor.
* **Drive Mechanism:** Leadscrew-coupled carriage that converts rotational torque into linear force against a standard syringe plunger.
* **Modular Mounts:** Designed for rapid toolless removal to easily swap or sterilize syringe barrels, dramatically reducing bioink waste during transitions.

### 2. Electronics & Control Prototyping
The electrical control architecture is currently prototyped on a breadboard for rapid iteration:
* **Microcontroller Interface:** Logic signals control speed, direction, and extrusion distance.
* **Motor Driver:** Dedicated current-limiting driver (e.g., A4988 or TMC2209) configured for microstepping to guarantee ultra-fine volumetric deposition without pulsing artifacts.
* **User Input:** Integrated tactile buttons or foot pedal signals to toggle extrusion on/off seamlessly during manual handling.

### 3. CAD & Digital Fabrication
* **Design Platform:** Modelled natively in **OnShape** using top-down parametric design principles to ensure perfect alignment between the motor housing, guide rails, and syringe sleeves.
* **Fabrication:** Components are optimized for 3D printing (FDM) without excessive support structures, utilizing high-infill PLA/PETG for structural rigidity under extrusion loads.

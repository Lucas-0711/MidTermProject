# Hardware & Safety: Generating the $B_0$ Field

To manipulate billions of microscopic protons, we need macroscopic, extremely powerful hardware. A modern MRI scanner is essentially a giant, multi-layered electromagnet. 

## The Solenoid Design
According to Maxwell's equations of electromagnetism, an electrical current running through a wire induces a magnetic field {cite}`Schild1990`. By linking many loops of wire together into a cylinder—a design known as a **solenoid**—we can create a large, highly homogeneous magnetic field inside the bore {cite}`Larson2026`. 

The strength of this magnetic field depends on the amount of current flowing through the wires.

*https://encrypted-tbn2.gstatic.com/licensed-image?q=tbn:ANd9GcQKMtSCHm3cP5X4izP6AJuxoChqPjcprWzCCoOe3Wv-m4CQaDDIh35zdYJm_LYEohvD9z77hWeS2zBnRQk*

## Achieving High Fields: Superconductivity
While early MRI systems used permanent magnets (which are incredibly heavy and limited in field strength) or resistive electromagnets (which generate massive amounts of heat), modern 1.5T, 3T, and 7T scanners rely on **superconducting magnets** {cite}`Schild1990`.

To achieve the massive currents required for clinical and Ultra-High-Field imaging without melting the wires, the solenoid coils are made of superconducting alloys {cite}`Larson2026`. These coils are bathed in liquid helium (a cryogen), cooling them to approximately 4 Kelvin (-269° C) {cite}`Schild1990`. At this temperature, the material loses all electrical resistance {cite}`Schild1990`. Once the current is introduced during installation, it flows permanently without requiring additional electrical energy to maintain the field {cite}`Schild1990`.

**Structural Differences (1.5T vs 7T):**
Moving from a 1.5T to a 7T system requires exponentially more wire, larger helium reservoirs, and massive iron shielding to contain the fringe magnetic field. This makes 7T scanners significantly heavier, bulkier, and more expensive to install and maintain.

*https://encrypted-tbn1.gstatic.com/licensed-image?q=tbn:ANd9GcRnlute3rRUzVdqVwSA4VvZ4SCaPQqHv68oNdakUF5RjVxqot1f72aYyKbpRdS714_z0e-uRVzMqlwAFrU*

## Critical Safety Aspects

The most important rule of MRI safety stems directly from the hardware design:

**The Magnet is ALWAYS ON.**
Because the coils are superconducting, the $B_0$ field is permanently active, 24/7, even when no patient is being scanned and no power is being drawn from the hospital grid {cite}`Larson2026`.

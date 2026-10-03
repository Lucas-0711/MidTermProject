# Hardware & Safety: Generating the $B_0$ Field

To manipulate billions of microscopic protons, we need macroscopic, extremely powerful hardware. A modern MRI scanner is essentially a giant, multi-layered electromagnet. 

## The Solenoid Design
According to Maxwell's equations of electromagnetism, an electrical current running through a wire induces a magnetic field {cite}`Schild1990`. By linking many loops of wire together into a cylinder—a design known as a **solenoid**—we can create a large, highly homogeneous magnetic field inside the bore {cite}`Larson2026`. 

The strength of this magnetic field depends directly on the amount of current flowing through the wires.

## Achieving High Fields: Superconductivity
While early MRI systems used permanent magnets (which are incredibly heavy and limited in field strength) or resistive electromagnets (which generate massive amounts of heat), modern 1.5T, 3T, and 7T scanners rely on **superconducting magnets** {cite}`Schild1990`.

To achieve the massive currents required for clinical and Ultra-High-Field imaging without melting the wires, the solenoid coils are made of superconducting alloys {cite}`Larson2026`. These coils are bathed in liquid helium (a cryogen), cooling them to approximately 4 Kelvin (-269° C). At this temperature, the material loses all electrical resistance. Once the current is introduced during installation, it flows permanently without requiring additional electrical energy to maintain the field. {cite}`Schild1990`

**Structural Differences (1.5T vs 7T):**
Moving from a 1.5T to a 7T system requires exponentially more wire, larger helium reservoirs, and massive iron shielding to contain the fringe magnetic field. This makes 7T scanners significantly heavier, bulkier, and more expensive to install and maintain.

### Sustainable Innovations: The Low-Helium MRI
While traditional superconducting magnets require massive amounts of liquid helium (often over 1,000 liters), recent breakthroughs have dramatically reduced this dependency. In 2023, the team of Dr. Stephan Biber and Dr. David M. Grodzki from Siemens Healthineers, along with Prof. Dr. Michael Uder from Uniklinikum Erlangen, was awarded the prestigious "Deutscher Zukunftspreis" (German Future Prize) {cite}`Zukunftspreis2023`. 

They developed a novel MRI system equipped with "DryCool" technology that operates with a sealed-for-life magnet requiring only 0.7 liters of liquid helium {cite}`SiemensFreeMax`. This innovation makes MRI technology more accessible globally, easier to install without massive quench pipes, and significantly more sustainable.

## Critical Safety Aspects

The most important rule of MRI safety stems directly from the hardware design:

**The Magnet is ALWAYS ON.**
Because the coils are superconducting, the $B_0$ field is permanently active, 24/7, even when no patient is being scanned and no power is being drawn from the hospital grid {cite}`Larson2026`.

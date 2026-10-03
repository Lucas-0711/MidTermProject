# The Main Magnetic Field ($B_0$)

To understand how an MRI generates images, we first have to look at the patient's own hydrogen atoms. 

## Protons as Tiny Magnets
Hydrogen protons possess a positive electrical charge and are constantly spinning around their own axis {cite}`Schild1990`. Because a moving electrical charge creates an electrical current, it naturally induces a tiny magnetic field {cite}`Schild1990`. Consequently, every single hydrogen proton in your body acts like a microscopic bar magnet {cite}`Schild1990`.

Under normal circumstances, these millions of tiny magnets point in completely random directions. Their individual magnetic fields cancel each other out, leaving the body with no net magnetic force. 

## Polarization: Walking on Feet vs. Hands
This chaos changes the moment a patient enters the main magnetic field of the scanner (denoted as $B_0$). Just like a compass needle aligns with the earth's magnetic field, the protons align themselves with the scanner's powerful $B_0$ field {cite}`Schild1990`. 

However, they can only align in two specific ways {cite}`Schild1990`:
*   **Parallel (Low Energy):** Pointing in the same direction as the external field. This is the preferred, comfortable state—analogous to a person walking naturally on their feet {cite}`Schild1990`.
*   **Anti-parallel (High Energy):** Pointing in the exact opposite direction. This state requires more energy—analogous to the exhausting effort of walking on one's hands {cite}`Schild1990`.

Because the parallel state requires less energy, a slightly larger number of protons choose to "walk on their feet" {cite}`Schild1990`. For every 10 million protons pointing against the field, there are roughly 10,000,007 pointing with it {cite}`Schild1990`. This tiny, unopposed majority adds up to create a new, measurable magnetic force within the patient: the **Net Magnetization**.

## The Impact of Ultra-High Fields (1.5 T to 7 T)
The primary purpose of the $B_0$ magnet is to create this polarization {cite}`Larson2026`. The stronger the external magnetic field, the more protons are forced into the parallel alignment. A shift from a clinical 1.5 T scanner to an Ultra-High-Field 7 T scanner dramatically increases the net magnetization, providing a stronger signal and significantly sharper images.

Use the interactive 3D visualization below to increase the $B_0$ field strength. Watch how the initially random protons (small cones) align, causing the net magnetization vector (the large central arrow) to grow.

```{embed} B0_Polarization.ipynb#polarization-3d```

**Safety Hazard: The Missile Effect**
Creating a 3T or 7T field requires massive electromagnets made of superconducting coils bathed in liquid helium. Because they are superconducting, **the magnet is ALWAYS ON.** The invisible magnetic field extends far beyond the scanner bore. Any ferromagnetic objects (like scissors, oxygen tanks, or certain implants) brought into the room can be violently sucked into the scanner, creating a lethal projectile hazard.

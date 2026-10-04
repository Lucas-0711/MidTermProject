# Physiological Effects of MRI Fields on the Human Body

An MRI scanner exposes the human body to three distinct types of magnetic fields: the static main field ($B_0$), the radiofrequency field ($B_1$), and the rapidly switching gradient fields. Each interacts with human physiology in unique ways.

## The Static Magnetic Field ($B_0$): Sensory Effects
The main magnetic field is permanently active and creates a powerful, uniform magnetic environment. While human tissue is primarily diamagnetic and structurally unaffected by static fields, movement through the field's spatial gradients (e.g., when the patient table slides into the bore) can induce distinct sensory effects.

Particularly noticeable in 3T and Ultra-High-Field (7T) scanners, patients may experience a fleeting sense of dizziness, vertigo, or a metallic taste in their mouth. This is caused by magnetohydrodynamic forces: moving through the strong magnetic field gradient induces tiny electrical currents in the endolymph fluid of the inner ear's vestibular system, temporarily tricking the brain into sensing motion. <br>
These sensory effects are transient, entirely harmless, and resolve once the patient rests stationary inside the isocenter.

## The Radiofrequency Field ($B_1$): Tissue Heating and SAR
To excite the spins, the scanner transmits Radiofrequency (RF) pulses. The human body acts as a conductive medium, and as it absorbs this electromagnetic RF energy, the energy is converted into heat. 

The Specific Absorption Rate (SAR) measures the amount of energy absorbed by the body from an RF pulse. It is proportional to the integrated total RF pulse power:

$$
SAR \propto \int_{0}^{T_{rf}} |b_1(\tau)|^2 d\tau
$$

Since this absorption can cause tissue heating, there are strict safety limits on SAR to minimize this heating. The scanner's software continuously calculates the accumulated SAR based on the patient's weight and the specific pulse sequence being run. It will automatically pause or prevent a scan if regulatory thresholds (typically limiting core body temperature rise to no more than 1°C) are approached.

## The Gradient Fields: PNS and Acoustic Noise
Magnetic field gradients are rapidly switched on and off to encode spatial information. According to Faraday's Law of Induction, changing magnetic fields ($\frac{dB}{dt}$) induce electrical currents in nearby conductive materials, including the human nervous system.

*   **Peripheral Nerve Stimulation (PNS):** If the gradients switch too rapidly or at too high an amplitude, the induced electrical currents can exceed the depolarization threshold of peripheral nerves. This results in Peripheral Nerve Stimulation (PNS), felt by the patient as a mild tingling, tapping sensation, or involuntary muscle twitching. Modern scanners actively monitor and limit gradient slew rates to ensure these induced currents remain comfortably below the threshold for pain or cardiac stimulation.
*   **Acoustic Noise:** The rapid switching of currents within the strong $B_0$ field subjects the gradient coils to immense Lorentz forces, causing them to vibrate violently against their mountings. This physical vibration generates the loud, characteristic knocking noises of an MRI scan, requiring patients to wear active or passive ear protection.

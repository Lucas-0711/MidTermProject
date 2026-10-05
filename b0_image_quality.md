# Image Quality

Moving from a standard 1.5T scanner to 3T, 7T, or beyond fundamentally alters the physics of the scan. A stronger magnetic field is not simply a "better camera", it introduces complex trade-offs between signal, contrast, and physiological safety.

## Signal-to-Noise Ratio
Signal-to-Noise Ratio (SNR) is the fundamental metric of image quality in MRI. It represents the ratio of true, usable image data (signal) emitted by the tissue to the random electronic interference (noise) inherent in the system. A high SNR produces a clear, sharp, and detailed image, whereas a low SNR results in a grainy, "noisy" appearance.

In MRI, SNR is primarily governed by four factors:
1. **Field Strength ($B_0$):** Higher magnetic fields polarize more protons, creating a larger net magnetization.
2. **Voxel Size:** Larger 3D-pixels capture more protons and yield more signal, but at the cost of spatial resolution (sharpness).
3. **Scan Time (Averages):** Measuring the same slice multiple times increases the true signal while averaging out random noise ($SNR \propto \sqrt{t}$).
4. **RF Coils:** Placing receiver coils closer to the body captures more pure signal and less environmental noise.

## Balancing Spatial Resolution and Scan Speed
Because SNR increases approximately linearly with the static magnetic field strength ($SNR \propto B_0$), a 3T scanner inherently provides roughly double the baseline SNR of a 1.5T scanner. This surplus acts as a "currency" that technologists can spend in two ways:
*   **Higher Spatial Resolution:** The extra signal can be divided into smaller voxels, providing sharper images capable of resolving finer anatomical details (e.g., minute ligaments or cranial nerves).
*   **Faster Scan Times:** If the baseline 1.5T resolution is sufficient, the extra signal can be used to accelerate the scan. Since $SNR \propto \sqrt{t}}$, doubling the baseline SNR allows the scan time to be cut significantly while maintaining diagnostic quality.

## Tissue Contrast: $T_1$ Prolongation
As the $B_0$ field gets stronger, protons precess faster ($\omega_0 = \gamma B_0$). This makes it harder for them to release absorbed energy into their surrounding molecular lattice, which prolongs **$T_1$ relaxation times**. 
*   **The Clinical Impact:** $T_1$-weighted contrast between different tissues (like gray and white matter in the brain) diminishes at higher field strengths. To compensate and restore this contrast, the Repetition Time (TR) of the pulse sequence must be increased, which can lengthen the overall scan time. {cite}`Schild`

## Susceptibility and Chemical Shift
Both magnetic susceptibility and chemical shift effects scale linearly with $B_0$. This creates distinct advantages and disadvantages:
*   **Magnetic Susceptibility:** Differences in how tissues become magnetized cause local distortions in the field. 
    *   *Pros:* Greatly enhances functional MRI (fMRI) by amplifying the BOLD effect, and improves the detection of micro-hemorrhages (SWI sequences).
    *   *Cons:* Worsens image distortion and signal voids near air-tissue interfaces (e.g., sinuses) or metallic implants.
*   **Chemical Shift:** The resonance frequency difference between fat and water protons grows at higher fields.
    *   *Pros:* Makes it much easier to isolate and selectively suppress the fat signal (Fat Saturation).
    *   *Cons:* Increases the "chemical shift artifact" (black and white borders) at interfaces where fat and water coexist, requiring higher receiver bandwidths to correct.
 
<img width="552" height="373" alt="chemical shift artifact" src="https://github.com/user-attachments/assets/513a2d0a-f065-4712-9405-3d6f3c2c4a3e" />

[MRIquestions/chemical-shift-artifact](https://mriquestions.com/chemical-shift-2nd-kind.html)

## The Limiting Factor: SAR (Tissue Heating)
While signal increases linearly with $B_0$, the radiofrequency (RF) energy required to tilt the protons increases quadratically ($\text{SAR} \propto B_0^2$). 
*   **The Bottleneck:** A 90° RF pulse at 3T deposits four times more heat into the patient's tissue than the exact same pulse at 1.5T. This makes SAR limits a major bottleneck in high-field MRI, often forcing the scanner to enforce mandatory cooling pauses or restricting the use of certain high-energy sequences (like Fast Spin Echo) altogether.

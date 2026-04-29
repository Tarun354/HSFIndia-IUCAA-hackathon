# Gravitational Wave Signal Identification from Strain Data

## 📌 Overview

This repository contains my solution to a problem from the **HSF India – IUCAA Hackathon**.

The original repository (forked) provides:
- Three strain datasets (`strain-1.gwf`, `strain-2.gwf`, `strain-3.gwf`)
- A problem statement to identify the presence of a gravitational wave signal

👉 The folder:HSFIndia-IUCAA-hackathon-Question/

contains the **original data**.

👉 The solution notebook:
contains my full analysis.

---

## 🎯 Objective

To determine whether a **gravitational wave signal** is present in the given strain data and identify which strain contains a physically consistent signal.

---

## ⚙️ Approach

The analysis follows a standard gravitational-wave data analysis pipeline:

### 1. Data Conditioning
- High-pass filtering
- Resampling
- Cropping edges

### 2. Matched Filtering
- Templates generated using **IMRPhenom waveform models**
- Signal-to-noise ratio (SNR) computed for each strain

### 3. Peak Detection
- Identified top peaks in SNR time series
- Compared multiple candidate peaks

### 4. χ² (Chi-square) Test
- Used to check signal consistency with template
- Helps distinguish real signals from noise glitches

### 5. Reweighted SNR
- Combined SNR and χ² using `newsnr`
- Suppresses false peaks (glitches)
- Highlights physically consistent signals

---

## 📊 Key Observations

- A **very strong peak** appears in all three strains at the same time  
  → This is identified as a **noise glitch**

- Secondary peaks exist in the data:
  - Lower raw SNR
  - Much lower χ² values

- After applying **reweighted SNR**:
  - Glitch peak is suppressed
  - A **physically meaningful signal emerges**

---

## ✅ Results

- The most consistent signal is found in:
  👉 **Strain 3**

- This peak:
  - Has moderate SNR
  - Has **low χ² (good consistency)**
  - Has **higher reweighted SNR compared to others**

- This indicates a **potential binary black hole (BBH) merger signal**

---

## 🧠 Conclusion

- Raw SNR alone is not sufficient to identify real signals
- χ² and reweighted SNR are essential to remove glitches
- The analysis shows that:

👉 **Strain 3 contains a BBH MERGER gravitational wave signal**

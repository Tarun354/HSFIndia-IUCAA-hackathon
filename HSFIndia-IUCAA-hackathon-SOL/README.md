# HSFIndia-IUCAA Hackathon: Gravitational Wave Data Analysis Challenge

Welcome to the HSFIndia-IUCAA Workshop Hackathon. In this challenge, you will step into the shoes of a LIGO data analyst to search for hidden gravitational-wave (GW) signals within real strain data from the O3b observing run.

## 📁 Dataset Overview

The repository contains three frame files (.gwf) of strain data recorded by the **Livingston (L1)** detector. Each file represents a continuous segment of **1024 seconds**.

### The Challenge

Buried within these frames are simulated signals merged with real detector noise. Your task is to identify and characterize them.

*   **The "Golden" Signal:** One of the three frames contains a clear, high-signal-to-noise ratio (SNR) gravitational wave signal.
*   **The Bonus (Precessing) Signals:** Two of the frames contain a weaker, more complex signal originating from a **precessing** binary system.

## 🎯 Objectives

### Phase 1: Detection

*   Analyze all three frames to identify which one contains the loud GW signal.
*   Provide a calculated estimate of the system parameters (e.g., Chirp Mass, Mass 1, Mass 2).

### Phase 2: Bonus Challenge

*   Identify which two frames contain the weak precessing signal.
*   Attempt to estimate the parameters of the precessing system.

## 🛠 Technical Specifications & Constraints

To ensure consistency in your analysis, please adhere to the following parameters:

*   **Detector:** L1 (Livingston)
*   **Data Origin:** O3b Run
*   **Channel Name:** L1:DCS-CALIB\_STRAIN\_C01
*   **Lower Frequency Cutoff (f\_low):** 30.0 Hz
*   **Duration:** 1024 seconds per frame.

**Good luck, and happy hunting for ripples in spacetime\!**


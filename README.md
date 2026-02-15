# 🛰️ Doppler Shift Estimation using RAD-DAR Dataset with FFT and Machine Learning


##  Project Overview

This project presents a web-based Doppler shift estimation tool for analyzing radar signals from the RAD-DAR dataset.

The system:

- Applies windowing functions
- Performs FFT transformation
- Extracts Doppler frequency shifts
- Estimates target velocities
- Classifies targets into:
  - Cars
  - Drones
  - People

Classification accuracy exceeds 85%.


## Doppler Radar Theory

The Doppler shift in radar systems is given by:

fd = (2 × fc × v) / c  

Velocity estimation:

v = (fd × c) / (2 × fc)

Where:
- fd = Doppler shift (Hz)
- fc = Carrier frequency (Hz)
- v = Velocity (m/s)
- c = Speed of light (299,792,458 m/s)

---

##  Methodology

1. Load RAD-DAR dataset
2. Apply window function (Hanning default)
3. Perform FFT (256–4096)
4. Extract frequency peaks
5. Compute Doppler shift
6. Estimate velocity
7. Classify targets
8. Visualize results

---

## Features

- Carrier frequency support: 1–10,000 MHz
- 15 Window functions
- Configurable FFT sizes
- Doppler shift plot
- Velocity histogram
- Automatic target classification
- Accuracy metric display

---

## Project Structure


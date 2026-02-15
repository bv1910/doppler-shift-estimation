#  Doppler Shift Estimation using RAD-DAR Dataset with FFT and Machine Learning

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)


##  Project Overview
This project estimates the Doppler shift from radar signals using FFT.  
It can detect the relative velocity of objects from radar datasets (RAD‑DAR).

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

## Installation
No installation needed! Open `web_app/index.html` in a browser to run.

## How to run the web app
1. Download or clone the project.
2. Navigate into the folder.
3. Open **web_app/index.html** in any web browser (Chrome, Firefox, Edge).


## Project Structure
doppler-shift-estimation/
 - Dataset/
 - web_app/
 - docs/
 - report/
 - README.md
 




#  Doppler Shift Estimation using RAD-DAR Dataset with FFT and Machine Learning

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

#  Doppler Shift Estimation Tool

Analyze radio frequency shifts from moving targets using RTL-SDR data.  
This web-based tool allows you to upload radar datasets, process them, and visualize Doppler shifts and target velocities interactively.

---

##  Tech Stack
- HTML, CSS, JavaScript
- [Chart.js](https://www.chartjs.org/) for visualizations
- [JSZip](https://stuk.github.io/jszip/) for ZIP file handling

---

## Features
- Upload ZIP datasets containing SDR/radar data
- Apply various window functions (Hanning, Hamming, Blackman, etc.)
- Perform FFT-based Doppler shift analysis
- Estimate velocities of targets
- Interactive charts for Doppler vs Frequency and Velocity distributions
- Target classification (Cars, Drones, People)
- Real-time progress display

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

## Installation
No installation needed! Open `web_app/index.html` in a browser to run.

##  How to Run
1. Clone or download the repo
2. Open `web_app/index.html` in any modern browser (Chrome, Firefox, Edge)
3. Upload your ZIP dataset
4. Adjust parameters and click **Process Data & Estimate Doppler Shifts**


## Project Structure
doppler-shift-estimation/
 - Dataset/
 - web_app/
 - docs/
 - report/
 - README.md

## 📊 Screenshots

<img src="docs/images/uploading dataset.jpg" width="500" alt="uploading dataset">













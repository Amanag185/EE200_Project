# 📡 EE200: Digital Signal Processing 

**Zapptain America Team Project | Signals, Systems & Networks**

This repository contains the foundational Digital Signal Processing (DSP) algorithms and analyses developed for Questions 1 and 2 of our EE200 coursework project. These scripts demonstrate core principles of signal manipulation, frequency-domain analysis, and robust acoustic feature extraction.
**Files:** `EE200_course_project_summer_2026.pdf`

---

## 📂 Part 1 (Q1): Spectral Analysis & Time-Frequency Domains
**Files:** `ee200Q1_Final_draft.ipynb` | `ee200Q1_report.pdf`

### Objective
To analyze the frequency spectrum of audio signals and understand the fundamental time-frequency trade-offs inherent in Digital Signal Processing using the Fourier Transform.

### Methodology
* **Signal Windowing:** Applied various windowing functions (e.g., Hamming, Hann) to raw audio arrays to mitigate spectral leakage during transformation.
* **Discrete Fourier Transform (DFT):** Transitioned raw audio from the time domain to the frequency domain to identify dominant harmonic frequencies.
* **Short-Time Fourier Transform (STFT):** Segmented the audio into overlapping frames to generate our first basic spectrograms, mapping how frequencies change over time.
* **Results:** Successfully visualized the spectral density of different audio clips, establishing the mathematical foundation needed for advanced audio profiling.

---

## 📂 Part 2 (Q2): Feature Extraction & Constellation Mapping
**Files:** `EE200_Q2_final.ipynb` | `EE200_Q2_Report.pdf`

### Objective
To isolate mathematically robust anchor points within a dense audio spectrogram, ensuring the features remain identifiable even in the presence of heavy acoustic noise or distortion.

### Methodology
* **Logarithmic Scaling:** Converted the linear power spectrograms from Q1 into the Decibel (dB) scale to accurately reflect human auditory perception.
* **2D Maximum Filtering:** Passed a sliding neighborhood filter (`scipy.ndimage.maximum_filter`) over the spectrogram array to identify local energy maxima.
* **Thresholding:** Applied an amplitude threshold to strip away the background noise floor, leaving only the most prominent acoustic peaks.
* **Results:** Successfully distilled millions of audio data points into a sparse, highly robust "constellation map" of time-frequency coordinates.

---

## 💻 Tech Stack
* **Language:** Python 3
* **Environment:** Jupyter Notebook (`.ipynb`)
* **Libraries:** NumPy, SciPy (`scipy.signal`, `scipy.ndimage`), Matplotlib

---

## 🚀 How to Run

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/Amanag185/EE200_Project.git](https://github.com/Amanag185/EE200_Project.git)
2. **Open the uploaded code for two parts**
3. **Run them in jupyter notebook/ google collab**

---

## 👥 Contributors

* **Aman Agrawal** - [@Amanag185](https://github.com/Amanag185)
* **Shorya Singh Rathore** - [@shorya-IITK](https://github.com/Shorya-IITK)

# Neonatal Sepsis Early Prediction Using AI

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-red)
![Model](https://img.shields.io/badge/Model-GRU%20%7C%20LSTM-orange)
![Project](https://img.shields.io/badge/Type-Research%20Project-yellow)
![License](https://img.shields.io/badge/License-MIT-green)

This repository presents a **patient-aware deep learning framework** for the **early prediction of neonatal sepsis**, focusing on **preterm infants** admitted to the Neonatal Intensive Care Unit (NICU).  
The system leverages **non-invasive vital signs**, specifically **Heart Rate (HR)** and **Oxygen Saturation (SpO₂)**, to identify early physiological deterioration *before clinical onset*.

---

## Framework Overview

<p align="center">
  <img src="figures/Overall framework pipeline (1).png" width="95%">
</p>

The figure above illustrates the end-to-end pipeline of the proposed framework, starting from raw NICU physiological monitoring, through preprocessing and temporal sequence construction, toMachine Learning and LSTM and ensemble Learning-based modeling and post-processing for clinically actionable alert generation.


## Project Overview

Neonatal sepsis is a time-critical condition in which early physiological changes often precede observable clinical symptoms. Conventional detection approaches typically rely on late-stage indicators, limiting the opportunity for timely intervention.  

This project proposes an **end-to-end, patient-aware deep learning framework** that integrates:

- Robust physiological data preprocessing  
- Time-series feature extraction and temporal sequence construction  
- **Machine Learning and LSTM and ensemble Learning**  
- Post-processing mechanisms for clinically meaningful alert generation  

The framework is designed to support **early warning prediction**, minimize false alarms, and reflect realistic NICU deployment conditions.


Evaluating both architectures enables a balanced assessment between **model expressiveness, computational efficiency, and generalization performance**, which is critical in safety-sensitive healthcare applications.

---

## Methodology Highlights

- Continuous HR and SpO₂ signals sampled at 0.5 Hz  
- Non-overlapping 10-minute windows for feature extraction  
- Statistical and cross-correlation features  
- Forecast-based labeling with a 24-hour prediction horizon  
- Patient-aware train/validation/test splitting  
- Temporal modeling using **Machine Learning and LSTM and ensemble Learning**  
- Post-processing for alarm stabilization  

---


---

## Technologies Used

- **Python**
- **NumPy, Pandas**
- **PyTorch**
- **Machine Learning and LSTM and ensemble Learning**
- **Time-Series Analysis**

---

## Key Contributions

- Patient-aware preprocessing pipeline to prevent data leakage  
- Forecast-based labeling strategy for early neonatal sepsis prediction  
- Comparative evaluation of Machine Learning and LSTM and ensemble Learning architectures  
- Clinically motivated post-processing for alert generation  

---

## Disclaimer

This project is intended **strictly for academic and research purposes**.  
It is **not** a certified medical device and should not be used for clinical decision-making without appropriate validation and regulatory approval.

---
## Note
This project is for academic and research purposes only.

## License

This project is released under the **MIT License**.



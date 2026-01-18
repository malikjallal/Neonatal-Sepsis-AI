# Neonatal Sepsis Early Prediction Using AI

This repository presents a patient-aware deep learning framework for the **early prediction of neonatal sepsis**, with a focus on **preterm infants** admitted to the Neonatal Intensive Care Unit (NICU).  
The system leverages **non-invasive vital signs**, specifically **Heart Rate (HR)** and **Oxygen Saturation (SpO₂)**, to identify early physiological patterns associated with sepsis *before clinical onset*.

---

## Project Overview

Neonatal sepsis is a time-critical condition in which early physiological changes often precede observable clinical symptoms. Conventional detection approaches typically rely on late-stage indicators, limiting the opportunity for timely intervention.  

This project proposes an **end-to-end, patient-aware deep learning framework** that integrates:

- Robust physiological data preprocessing  
- Time-series feature extraction and temporal sequence construction  
- **Recurrent neural network modeling using GRU and LSTM architectures**  
- Post-processing mechanisms for clinically meaningful alert generation  

The framework is designed to support **early warning prediction**, minimize false alarms, and reflect realistic NICU deployment conditions.

---

## Why GRU and LSTM?

Recurrent neural networks are well-suited for modeling physiological time-series due to their ability to capture temporal dependencies. In this work, **both Long Short-Term Memory (LSTM) and Gated Recurrent Unit (GRU)** architectures were investigated to leverage their complementary strengths.

- **LSTM** models long-term temporal dependencies using explicit memory and gating mechanisms, making it effective for capturing gradual physiological deterioration patterns.
- **GRU**, with its simplified gating structure, offers comparable representational capacity while requiring fewer parameters, leading to faster convergence and improved stability on large-scale, imbalanced clinical datasets.

Evaluating both architectures enables a balanced assessment between **model expressiveness, computational efficiency, and generalization performance**, which is critical in safety-sensitive healthcare applications.

---

## Methodology Highlights

- Continuous HR and SpO₂ signals sampled at 0.5 Hz  
- Non-overlapping 10-minute windows for feature extraction  
- Statistical and cross-correlation features  
- Forecast-based labeling with a 24-hour prediction horizon  
- Patient-aware train/validation/test splitting  
- Temporal modeling using **GRU and LSTM networks**  
- Post-processing for alarm stabilization  

---


---

## Technologies Used

- **Python**
- **NumPy, Pandas**
- **PyTorch**
- **GRU and LSTM-based Deep Learning**
- **Time-Series Analysis**

---

## Key Contributions

- Patient-aware preprocessing pipeline to prevent data leakage  
- Forecast-based labeling strategy for early neonatal sepsis prediction  
- Comparative evaluation of GRU and LSTM architectures  
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



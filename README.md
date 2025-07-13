# ECG Classification Using Phase-Folded Feature Extraction

This repository contains code, data, and results from my Master's thesis project on ECG classification using phase-folded waveform parameterisation. The project explores the extraction of interpretable ECG features from the PTB-XL dataset and evaluates model performance in both multiclass and binary classification tasks.

## Project Overview
- Developed a custom **phase-folding approach** to extract temporal and amplitude features from 12-lead ECG signals.
- Performed ML by using the extracted ECG parameters as features and disease superclasses as outcomes. 
- Evaluated model performance using **LightGBM** for both binary (NORM vs ABNORMAL) and multiclass classification across diagnostic superclasses (e.g., NORM, STTC, MI, CD, HYP).
- Compared extracted features with existing benchmark datasets, including **EcgDeli** and **UniG**, using **Pearson cross-correlation**.

## Key Findings
- Binary Classification achieved the highest accuracy of 83%, and Multiclass Classification had 68%.
- Best performance on **Normal** and **STTC** classes (F1-scores of 82% and 69%)
- Lower performance on **MI**, **HYP**, and **CD**, influenced by **class imbalance**
- Strong correlation between phase-folded features and EcgDeli/UniG (e.g., R amplitude: 95%)

## 📄 File Descriptions

| File Name                   | Description                                                                 |
|----------------------------|-----------------------------------------------------------------------------|
| `ECG Project -- 1.ipynb`    | Main feature extraction notebook using the phase-folded method.             |
| `MachineLearning -- 2.ipynb`| Applies LightGBM for multiclass and binary classification on extracted features. |
| `UnigCorrelation -- 3.ipynb`    | Cross-correlates features from phase-folded extraction with UniG features.    |
| `EcgDeliCorrelation -- 4.ipynb` | Compares phase-folded features with EcgDeli using Pearson correlation.       |
| `Thesis.pdf`                | Final MSc thesis document summarising the full methodology and findings.    |
| `README.md`                | Project overview and documentation.                                         |



## Citation
If using this project or methods, please cite:
> Agrawal, I. (2025). *Parameterising ECG Waveforms to Uncover Pathology: A Phase-Folded Approach*. MSc Thesis, University of Aberdeen.

## Contact
For questions or collaboration inquiries, feel free to reach out at: isha15aug@outlook.com

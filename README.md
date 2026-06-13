# OCR Assisted Chemical Identification and In Silico Screening of Dermal Permeability and Skin Toxicity

**A Mobile-Compatible Computational Platform for Rapid Dermatotoxicological Assessment**

---

## 📋 Overview

This repository contains the source code and supporting materials for an integrated computational platform that combines:

- **Optical Character Recognition (OCR)** for automated chemical identification from images or labels
- **Automated PubChem data retrieval** for physicochemical parameter extraction (MW, logP)
- **QSAR-based dermal permeability prediction** using the Potts and Guy equation
- **Electrophilicity index (ω)-based toxicity estimation** for preliminary skin sensitization screening
- **Flux and diffusion kinetic simulation** for dermal transport behavior
- **Mobile-compatible graphical user interface (GUI)** for field and clinical use

This tool is designed for rapid preliminary screening of chemical-associated skin exposure risks in occupational dermatology, cosmetic safety evaluation, pharmaceutical research, and environmental toxicology.

---

## 🔬 Scientific Background

Dermal exposure to industrial, pharmaceutical, and cosmetic chemicals is a major concern in occupational and clinical dermatology. This platform applies established in silico models to enable rapid screening without the need for laboratory infrastructure.

### Potts and Guy Equation (Skin Permeability)

```
log Kp = −2.72 + 0.71(logP) − 0.0061(MW)
```

Where:
- `Kp` = skin permeability coefficient (cm/s)
- `logP` = octanol/water partition coefficient
- `MW` = molecular weight (Da)

### Electrophilicity Index (Toxicity Estimation)

```
ω = μ² / 2η
```

Where:
- `ω` = electrophilicity index
- `μ` = chemical potential
- `η` = chemical hardness

### Steady-State Flux

```
J = Kp × C
```

### Diffusion Lag Time

```
T_lag = L² / 6D
```

---

## ⚙️ Features

| Feature | Description |
|--------|-------------|
| OCR Chemical Recognition | Extracts chemical names from uploaded images or labels |
| PubChem Integration | Automatically retrieves MW and logP for identified chemicals |
| Dermal Permeability Prediction | Classifies compounds as Low / Moderate / High permeability |
| Toxicity Estimation | Electrophilicity-based preliminary skin sensitization screening |
| Kinetic Simulation | Estimates flux, lag time, and peak absorption time (Tmax) |
| GUI Interface | User-friendly interface compatible with mobile and desktop platforms |
| Graphical Output | Visualizes prediction results numerically and graphically |

---


---


```

### Input Options

1. **Image Upload** — Upload a chemical label image; OCR will extract the chemical name automatically
2. **Manual Entry** — Type the chemical name directly into the input field
3. **Batch Mode** — Upload a list of chemical names via CSV for batch screening

### Output

- Permeability classification (Low / Moderate / High)
- Predicted logKp value
- Electrophilicity index (ω)
- Estimated flux (J) and lag time (Tlag)
- Graphical summary of results

---

## 📊 Validation

The platform was validated using 10 reference compounds with known dermal permeability characteristics:

| Chemical | MW (Da) | logP | Predicted | Reported |
|----------|---------|------|-----------|----------|
| Caffeine | 194.19 | −0.07 | Low | Low |
| Nicotine | 162.23 | 1.17 | Moderate | Moderate |
| Testosterone | 288.42 | 3.32 | High | High |
| Hydrocortisone | 362.46 | 1.61 | Moderate | Moderate |
| Benzoic acid | 122.12 | 1.87 | Moderate | Moderate |
| Ibuprofen | 206.28 | 3.50 | High | High |
| Salicylic acid | 138.12 | 2.26 | Moderate | Moderate |
| Lidocaine | 234.34 | 3.26 | High | High |
| Ethanol | 46.07 | −0.31 | Low | Low |
| Cortisone | 360.44 | 1.50 | Moderate | Moderate |

Classification accuracy: **10/10 (100%)** concordance with reported permeability categories.

---

## 📁 Repository Structure

open index.html
or download Apk file to install in mobile
```

---

## ⚠️ Limitations

- Validated on 10 reference compounds; broader validation is ongoing
- OCR accuracy depends on image quality and label clarity
- The Potts and Guy model is most reliable for passive diffusion of non-ionized, non-metallic compounds
- Electrophilicity-based toxicity assessment is a theoretical approximation, not a substitute for experimental testing
- Requires internet connectivity for PubChem data retrieval
- Not intended for clinical diagnosis or regulatory decision-making

---

## 📄 Citation

If you use this tool in your research, please cite:



## 👥 Authors

- **Muhammad Aziz** — Institute of Biochemistry, University of Balochistan, Quetta, Pakistan
  (aziz1sh@hotmail.com)
-**Zunaira**-Department of Electronics, BUITEMS,Quetta
- **A.N. Sheikh** — Pakistan Chemical Computational Society, Pakistan

---

## 📜 License

This software is protected under copyright registered with the Intellectual Property Office of Pakistan. It is freely available for academic and non-commercial research use, provided that the original publication is cited. 
Any commercial application requires prior written consent from the corresponding author (aziz1sh@hotmail.com).


*This tool is intended for research and preliminary screening purposes only. It does not replace experimental dermatotoxicological testing or clinical evaluation.*

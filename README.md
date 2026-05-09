# IFNepitope: Designing of Interferon-Gamma Inducing MHC Class-II Binders

Welcome to the official documentation for **IFNepitope**, a comprehensive computational tool developed to predict and design interferon-gamma (IFN-γ) inducing peptides. IFN-γ is a vital cytokine secreted by MHC class II-activated CD4+ T helper cells, playing a substantial role in controlling infections like *Mycobacterium tuberculosis*.

**Web Server:** [http://crdd.osdd.net/raghava/ifnepitope/](http://crdd.osdd.net/raghava/ifnepitope/)

---

## Citation

Dhanda, S. K., Vir, P., & Raghava, G. P. S. (2013). 
**Designing of interferon-gamma inducing MHC class-II binders.** *Biology Direct*, 8, 30. 
[https://doi.org/10.1186/1745-6150-8-30](https://doi.org/10.1186/1745-6150-8-30)

---

## About the Platform

IFNepitope is the first method developed to predict the specific type of cytokine (specifically IFN-γ) secreted by T-helper epitopes. While many tools can predict MHC class II binders, IFNepitope adds a crucial layer of functional annotation by determining if those binders will actually induce an IFN-γ response.

### Dataset Overview
The models were trained and validated on extensive datasets:
* **Main Dataset**: Contains 3,705 IFN-γ inducing and 6,728 non-IFN-γ inducing MHC class II binders.
* **IFNgOnly Dataset**: Contains 4,483 IFN-γ inducing epitopes and 2,160 epitopes that induce other cytokines.

---

## Key Features

### Prediction and Analysis
* **Induction Prediction**: Predicts whether a given peptide is an IFN-γ inducer or a non-inducer.
* **Motif Identification**: Utilizes motifs identified via MERCI software that are characteristic of IFN-γ inducing binders.
* **Positional Conservation**: Analyzes the positional conservation of residues at the N and C terminals to enhance prediction accuracy.

### Performance Metrics
* **Hybrid Approach**: The SVM-based models achieved high accuracy by utilizing amino acid composition and positional information.
* **Sequence Scans**: Users can scan entire protein sequences to identify potential IFN-γ inducing regions.

---

## Technical Overview

IFNepitope utilizes various sequence-based features to model the biological activity of T-helper epitopes.

* **Machine Learning**: Built using Support Vector Machines (SVM) and validated through 5-fold cross-validation.
* **Input Features**: Includes amino acid composition, dipeptide composition, and binary profiles.
* **Motif Library**: Incorporates a library of motifs that are significantly enriched in IFN-γ inducing peptides.

---

## Applications

* **Vaccine Design**: Identifying T-helper epitopes that will trigger a protective IFN-γ response.
* **Immunotherapy**: Designing therapeutic peptides to modulate cytokine production in autoimmune or infectious diseases.
* **Epitope Mapping**: Mapping functional regions in antigens that are responsible for cell-mediated immunity.

---

## Contact & Authors

**Prof. Gajendra P. S. Raghava** Bioinformatics Centre, CSIR-Institute of Microbial Technology, Chandigarh, India.  
**Email**: raghava@imtech.res.in

---

## License

This resource is open-access and distributed under the terms of the **Creative Commons Attribution License**, permitting unrestricted use and distribution provided the original work is properly credited.

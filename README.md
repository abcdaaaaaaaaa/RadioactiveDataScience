# RadioactiveSpaceData v5.0.0

## RadioactiveDataScience What can be create?
"The first and only Arduino library where Geiger Counter combine with Data Science"

## 1) Multidimensional Radioactive Decay Estimations
![3D_preview](https://github.com/user-attachments/assets/586d16b4-6088-4917-b9ea-e49ebb4a5876)
## 
![2D_preview](https://github.com/user-attachments/assets/1ddea30f-7e8e-4b35-a259-23b3520053ac)

This repository presents a multivariable exponential regression model to estimate **Average CPM** (counts per minute) based on **Time**, **Radiation dose rate (Usv/hr)**, **Standard Deviation of CPM (sdCPM)**, and **Total CPM Count**.

## 2) Development of a Unique Model Equation

The predicted average CPM is defined by the following equation:

<img width="750" alt="formullas" src="https://github.com/user-attachments/assets/6f94b3f0-cd1f-4432-82df-316aa9cb570a" />

Where:

<img width="750" alt="formullas2" src="https://github.com/user-attachments/assets/4ceb5d3a-1599-4932-bd29-cc81fadf0e23" />

## 3) Creation of Original Algorithm Logic

1. **Input features**:  
   - `Time`  
   - `Usv/hr` (radiation dose rate)  
   - `sdCPM` (standard deviation of CPM)  
   - `CPM Count` (total count)

2. Apply **natural logarithm** (`ln`) to all features except time to linearize exponential behavior.

3. Fit a **linear regression** model to:

<img width="750" alt="logformulla" src="https://github.com/user-attachments/assets/a9037f56-0f8d-488d-baa1-ff7c6fa4f279" />

4. Final prediction is obtained by **exponentiating** the output.

# RadioactiveSpaceData v5.5.4

## RadioactiveDataScience What can be create?
"The first and only Arduino library where Geiger Counter combine with Data Science"

## 1) Multidimensional Radioactive Decay Estimations in 3 Different Modes
### 3D Analysis
![3D_preview](https://github.com/user-attachments/assets/586d16b4-6088-4917-b9ea-e49ebb4a5876)
### Data Visualization
![2D_preview](https://github.com/user-attachments/assets/1ddea30f-7e8e-4b35-a259-23b3520053ac)
### Multi Graph
![multi_preview](https://github.com/user-attachments/assets/3d89f636-735f-4f85-aa7e-27be6caa7cae)

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


## Check out all our DataScience libraries under the SpaceData series!

<b> "The first and only Arduino library series where Gas Sensors and Geiger Counter combine with Data Science"

| Library | Scope |
|---------|---------|
| <a href="https://github.com/abcdaaaaaaaaa/MQDataScience">MQDataScience  | MQ2, MQ3, MQ4, MQ5, MQ6, MQ7, MQ8, MQ9, MQ131_LOW, MQ131_HIGH, MQ135, MQ136, MQ137, MQ138, MQ214, MQ216, MQ303A, MQ303B, MQ306A, MQ307A, MQ309A Gas Sensors  |
| <a href="https://github.com/abcdaaaaaaaaa/TGSDataScience">TGSDataScience  | TGS813, TGS822, TGS826, TGS2201, TGS2442, TGS2600, TGS2602, TGS2610, TGS2611, TGS2612, TGS2620, TGS6812, TGS8100 Gas Sensors |
| <a href="https://github.com/abcdaaaaaaaaa/MG811DataScience">MG811DataScience  | MG811 Gas Sensor  |
| <a href="https://github.com/abcdaaaaaaaaa/SP3S-AQ2DataScience">SP3S-AQ2DataScience  | SP3S-AQ2-01 Gas Sensor  |
| <a href="https://github.com/abcdaaaaaaaaa/RadioactiveDataScience">RadioactiveDataScience  | Geiger Counter  |

## For detailed explanation, You can also check out the github <a href="https://github.com/abcdaaaaaaaaa/RadioactiveDataScience/wiki">Wiki Page!

## You can access the library's article <a href="https://www.spacepedia.info/RadioactiveDataScience">Here!

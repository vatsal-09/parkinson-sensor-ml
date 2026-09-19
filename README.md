\# Parkinson Sensor ML



\### Sensor-Based Movement Analysis Using Accelerometer, Gyroscope and Magnetometer Data



A sensor-data machine learning and deep learning project for movement analysis using accelerometer, gyroscope, and magnetometer signals.



> \*\*Current Phase:\*\* Phase 1 - Pipeline validation using the IDNet sample dataset.



\## Project Overview



This project develops an end-to-end sensor-processing and machine-learning pipeline for movement analysis.



The pipeline includes:



\- Sensor data quality analysis

\- Multi-sensor synchronization

\- Fixed-length time-series windowing

\- Time- and frequency-domain feature extraction

\- Feature normalization

\- Machine learning models

\- Deep learning models

\- Multiple validation strategies

\- FAR / FRR analysis

\- Confusion matrix analysis

\- Ensemble evaluation



\## Sensors



\- Accelerometer: X, Y, Z

\- Gyroscope: X, Y, Z

\- Magnetometer: X, Y, Z



Total: \*\*9 sensor channels\*\*



\## Pipeline



Raw Sensor Data

â†“

Data Quality Checking

â†“

Sensor Synchronization

â†“

60 Hz Common Timeline

â†“

5-second Windows

â†“

Feature Extraction

â†“

Normalization

â†“

Machine Learning / Deep Learning

â†“

Validation and Evaluation



\## Models



\- Random Forest

\- Support Vector Machine

\- 1D CNN

\- CNN-LSTM



\## Phase 1 Results



The strongest completed validation configuration was:



\*\*Stratified 5-Fold + Linear (Min-Max) + SVM\*\*



\- Accuracy: \*\*89.45%\*\*

\- FAR: \*\*2.73%\*\*

\- FRR: \*\*19.34%\*\*



\## Important Finding



The experiments showed a substantial validation-to-test gap for the CNN-LSTM model, demonstrating the importance of recording-level splitting and careful evaluation for sensor-based machine learning.



\## Dataset



The raw dataset is \*\*not included\*\* in this repository.



The repository contains the processing pipeline, experiments, results, and documentation.



\## Documentation



See:



`docs/Phase1\_Project\_Diary.pdf`



for the detailed Phase 1 methodology and experimental record.



\## Project Status



\### Completed



\- Data preprocessing

\- Sensor synchronization

\- Windowing

\- Feature extraction

\- Random Forest

\- SVM

\- 1D CNN

\- CNN-LSTM

\- Normalization experiments

\- Four validation strategies

\- FAR / FRR analysis

\- Confusion matrices

\- Ensemble evaluation



\### Next Phase



Application of the validated pipeline to the actual Parkinson-labelled dataset.



\## Requirements



Install dependencies using:



```bash

pip install -r requirements.txt

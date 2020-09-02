# DS-challenge-Fault-Detection
Goal: Detect the faulty modes by building a ML model on the time series data

The DS challenge was offered by Tagup. The data contains four time series measurements of each machine. There are three states that the machine can be in: normal mode, faulty mode, and failed mode. The machine started in normal mode, and may enter the faulty mode and then may fail. To prevent the machine from entering the failed mode, we would like to detect if the machine has already entered the faulty mode and halt the machine before further damage occurs. 

To solve this task, I built a SVM classifier with appropriate feature extractions. The performance of the algorithm is visualized in the end, which can show that the model detected the faulty state effectively. 

The original data contains substantial background noise due to communication errors. To effectively learn the features of each operation mode, I removed the noise by using a median-filter.

**keywords:** Fault Detection, Time Series, Smoothing Technique, SVM, Spectrum Analysis, Data Visualization

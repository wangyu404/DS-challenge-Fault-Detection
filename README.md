# DS-challenge-Fault-Detection
Goal: Detect the faulty modes by building a ML model on the time series data

The DS challenge was offered by Tagup. The data contains four time series measurements for each machine. There are three states that the machine could be in: normal mode, faulty mode, and failed mode. The machine started with the normal mode, and may enter the faulty mode and then may fail. To prevent the machine to enter the failed mode, we would like to detect is the machine has already entered the faulty mode and halt the machine before further damage occurs. 

To solve this task, I built a SVM classifier with appropriate feature extractions. The performance of the algorithm is visualized in the end and it detected the faulty state effectively. 

The original data contains many background noise due to communication errors. To effectively learn the features of each operation mode, I removed the noise by using a median-filter.


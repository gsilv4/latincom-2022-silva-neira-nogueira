# A Deep Learning-based System for DDoS Attack Anticipation

This is the official repository for our [paper](https://ieeexplore.ieee.org/document/10000427) published at the 2022 IEEE Latin-American Conference on Communications.

### How is this repository organized?
- **experiment.ipynb:** Notebook file containing all the code needed to train the model described in our paper and display the evaluation metrics.
- **full_capture20110818_preprocessed_1s.csv:** CSV file containing the preprocessed data used as the network input to train the model.
- **lstm_autoencoder_ctu13_cap51_2.h:** The saved model file that was obtained at the end of our experiment. It can be used to reproduce the experiment without having to train the model from scratch.
- **preprocessing:** A folder containing the scripts used in the data preprocessing step. First, the `data_preprocessing.py`.py script must be used to extract the selected features of each network traffic packet and then the `data_transformation.py` script must be used to apply the statistical measures and obtain the final data format used for training the model. The raw data can be obtained from the official dataset [website](https://mcfp.felk.cvut.cz/publicDatasets/CTU-Malware-Capture-Botnet-51/).

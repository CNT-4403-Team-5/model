# Machine Learning for Traffic Analysis

*Florida Atlantic University - Fall 2021*

*CNT 4403 - Foundations of Cybersecurity / Team 5*

<p>&nbsp;</p>

This project focuses on predicting normal from malicious traffic, specifically DoS attacks. The UNSW-NB15 dataset (https://research.unsw.edu.au/projects/unsw-nb15-dataset) is used as a baseline to be compared to simulated DoS attack data and captured normal traffic from an isolated environment. Two literature models are implemented, along with a custom model.

The literature models replicated/referenced are from the following paper: 

    'DEEP-INTRUSION DETECTION SYSTEM WITH ENHANCED UNSW-NB15 DATASET BASED ON DEEP LEARNING TECHNIQUES'

    A.M. ALEESA, MOHAMMED YOUNIS, AHMED A. MOHAMMED, NAN M. SAHAR

<p>&nbsp;</p>

Group members
- **Alena Krause** (team lead - data capturing, DoS simulation, machine learning assistance)
- **Shannon Soulard** (DoS simulation, isolated environment setup)
- **Shelly Davidashvilly** (machine learning)

<p>&nbsp;</p>

---

<p>&nbsp;</p>

## Running Code
To run the code, first install necessary packages by navigating to the directory and running requirements.txt as follows:
```
pip install -r requirements.txt
```

Any other packages that need to be installed can be done so by running
```
pip install PACKAGE_NAME
```
---

<p>&nbsp;</p>

## Files Information
* ann.ipynb, dnn.ipynb, custom_model.ipynb include the respective models trained on the UNSW-NB15 data
* simulated_data_models include the same model architectures trained on the simulated data
* data_preprocessing.ipynb and simulated_data_pred.ipynb include data preparation of the UNSW-NB15 and simulated data, respectively
* data_analysis.ipynb does exploratory data analysis on the UNSW-NB15 data
* trained models are stored in /trained_models
* images from exploratory data analysis and model training/evaluation are stored in the /img folder

---

<p>&nbsp;</p>

## Datasets Information
* **data.npz** - the UNSW-NB15 data prepared with scaling and into train/val/test sets
* **data_sim.npz** - the simulated data prepared with scaling and into train/val/test sets
* **balanced_data.npz** - the balanced UNSW-NB15 dataset (done in data preprocessing)
* **UNSW-NB15_{1-4}** - the raw UNSW-NB15 data files, available from https://cloudstor.aarnet.edu.au/plus/index.php/s/2DhnLGDdEECo4ys?path=%2FUNSW-NB15%20-%20CSV%20Files
* **wshark_dos** - the simulated DoS attack data
* **wshark_norm** - the simulated normal traffic
* **merged.csv** - has the normal and DoS traffic combined into a single file, for data preprocessing purposes
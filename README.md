# BATADAL Dataset

## Overview

This folder contains the datasets used to evaluate a hybrid framework that combines blockchain verification with unsupervised machine learning for anomaly detection in Industrial Control Systems (ICS) and Supervisory Control and Data Acquisition (SCADA) systems.

The BATADAL dataset was selected because it provides realistic water distribution system data containing both normal operations and cyberattack scenarios. The dataset was used to evaluate the effectiveness of blockchain verification in improving the reliability of anomaly detection.

## Dataset Source

The BATADAL (BATtle of the Attack Detection Algorithms) dataset was developed to support research in cyberattack detection for water distribution systems.

**Dataset Website:** https://batadal.net

## Files Included

### Original Datasets

#### BATADAL_Training Dataset 1 does not contain any attacks.csv

* Contains normal operational data.
* Used to establish baseline system behavior during model training.

#### BATADAL_test_dataset.csv

* Contains both normal and attack data.
* Used to evaluate anomaly detection performance.

### Blockchain-Verified Datasets

#### BATADAL_Training_Dataset1_with_hashchain.csv

* Blockchain-verified version of the training dataset.
* Includes hash-chain fields for data integrity verification.

#### BATADAL_test_dataset_with_hashchain.csv

* Blockchain-verified version of the test dataset.
* Includes hash-chain fields for data integrity verification.

## Research Usage

The dataset was used to evaluate a hybrid framework consisting of:

* Blockchain verification
* Isolation Forest
* DBSCAN
* One-Class SVM

The blockchain component verifies data integrity before machine learning analysis is performed. The machine learning models then analyze the verified data to identify anomalous behavior.

## Evaluation Benchmarks

The framework was evaluated using the following performance benchmarks:

* Data Integrity ≥ 95%
* Detection Accuracy ≥ 90%
* Detection Latency ≤ 1 Minute
* False Positive Reduction ≥ 10% Under Tampered Conditions

## Notes

* The original BATADAL dataset was not modified except for preprocessing required for machine learning analysis.
* Blockchain-verified versions include additional fields used to support data integrity verification and tamper detection.
* These datasets are provided for academic and research purposes only.

## Citation

If you use the BATADAL dataset in your research, please cite the original dataset creators and associated publications according to their citation requirements.

## Praxis Context

This repository supports the Doctor of Engineering praxis research:

**A Hybrid Blockchain-Machine Learning Approach for Securing ICS and SCADA Systems Against State-Sponsored Cyberattacks**

The research evaluates how blockchain verification can improve confidence in anomaly detection results by ensuring data integrity before analysis is performed.


## Reproducibility

The file April_Jacque_BATADAL_Test_Final.ipynb contains the complete experimental workflow used in this research.

The notebook contains the complete workflow for:

- Data preprocessing
- Hash-chain generation
- Blockchain verification
- Anomaly detection modeling
- Performance evaluation
- Statistical analysis
- Results

Users may reproduce the experiments by opening the notebook and following the documented workflow.

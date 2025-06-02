# Gamma-Ray Burst Detection from Radio Signals Using CNN-LSTM

This repository contains the code for a project on detecting gamma-ray bursts (GRBs) using neural networks (CNN + LSTM), processing radio signal data.

### Project Structure

- **Data/**  
  Contains:
  - `grb_txt/`: raw signal data (txt) from the original dataset.
  - `GRL2015.pdf`: the scientific paper we relied on; the source of the dataset.

- **data_preprocesing/**  
  Code for data preparation, to be run in the following order:
  1. `txt_to_csv.ipynb`: converts raw txt files to csv format.
  2. `detect_peak.ipynb`: detects peaks and creates a readable table.
  3. `data_for_uniq.ipynb` or `data_for_3sec.ipynb`: prepares datasets for 30-second or 5-second bins.
  4. `united_sample.ipynb` or `united_3sec.ipynb`: merges all data into a final table.
  5. `grafs.ipynb`: visualizes graphs for comparison with results from `GRL2015.pdf`.

- **model_training/**  
  Contains:
  - `experiment_1.ipynb`, `experiment2.ipynb`, `experiment3.ipynb`: code for three experiments described in the paper.
  - `experiment_1.h5`, `experiment_2.h5`, `experiment_3.h5`: saved trained models for each experiment.

### Usage

The workflow is designed to be run in Jupyter Notebook. Simply follow the notebook sequence as described.

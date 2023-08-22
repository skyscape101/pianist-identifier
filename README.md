# pianist-identifier
To get started with our project, you'll first need to download the dataset. You can find the dataset and its related files in this GitHub link:
https://github.com/BetsyTang/ATEPP/blob/master/disclaimer.md

In this project, we use **Version-1.1**, and make sure to unzip the same file root with code.


# Introduce **0.Data**

**MIDI Data Processing and Feature Extraction**

This repository contains a series of Python scripts designed to process and extract features from MIDI files, specifically focusing on compositions by Ludwig van Beethoven.

**Overview**

The code performs the following main tasks:

Data Loading and Filtering: Loads a CSV metadata file and filters out compositions by Ludwig van Beethoven.

Data Sampling: From the top artists with the most records, it randomly selects 300 records for each artist.

Data Encoding and Splitting: Encodes the artist names and splits the data into training and testing sets.

MIDI to Piano Roll Conversion: Converts MIDI files to padded piano roll representations.

Feature Extraction: Extracts various musical features from MIDI files, such as **Inter-Onset Interval (IOI), Off-Time Duration (OTD), dynamic levels, polyphony, pedal usage, and legato/staccato ratios**.

Final Outputs

Padded Piano Rolls: The processed MIDI files are converted into piano roll representations and saved as:

X_train_padded2.npy

X_test_padded2.npy

Extracted Features: The extracted features from the MIDI files are saved as:

X_train_features4.npy

X_test_features4.npy


## Prerequisites:

Ensure you have the required libraries installed:

pip install pandas scikit-learn pretty_midi mido tqdm numpy

## Running the Script:

Simply execute the provided Python script. Ensure that the ATEPP-metadata-1.1.csv file is in the same directory or provide the appropriate path.

## Output Files:

After execution, you should find the .npy files in the same directory, which contain the processed data and extracted features.

# Introduce **0.1 Visualization of piano roll**
Simple polt function to visualize first output of piano roll

# Introduce **1. CNN+MLP Final**


# DEAP Dataset Behavioral & EEG Analysis Pipeline

This repository holds the Python code I used to analyze physiological and behavioral responses using the DEAP dataset for my human behavioral research project. 
this pipeline handles everything from pulling the dataset via KaggleHub to mapping participant metrics and outputting multi-page PDF performance reports.

## What This Code Does
1. Data Ingestion:Automatically downloads and pulls the DEAP dataset using KaggleHub and loads the official metadata tracks.
2. Data Cleaning & Timestamp Formatting: Filters down to the 40 experimental tracks and formats track start/end timestamps into clean `MM:SS` strings.
3. Statistical & Behavioral Merging:Merges multi-subject ratings, calculates acoustic properties, and computes normalized focus scores (Z-scores) across experimental trials.
4. Automated PDF Generation:Loops through the subjects, picks out peak focus events, and uses Matplotlib to batch-generate clean multi-page PDF visualization dashboards.

## Tech Stack
Python 3
Google Colab 
Pandas, NumPy, Matplotlib, SciPy, PyDub, KaggleHub

## How to View or Run
You can open and test the code directly in Google Colab using the badge below:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1S1UGS21HiRvutblvBGfql5JrNxABHrAy?usp=sharing)

(Note: You will need a Kaggle account/API setup to let KaggleHub pull the dataset successfully when running the notebook.)

## Ethics & Compliance
In line with data privacy guidelines, this repository doesn't contain raw participant files—everything runs using the standardized, open-access DEAP benchmark dataset.
Generative AI (Google Gemini) was used as a coding assistant to help draft, structure, and debug parts of this Python data analysis pipeline.

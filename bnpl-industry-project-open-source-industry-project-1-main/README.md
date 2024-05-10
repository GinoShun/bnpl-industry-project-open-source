[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/wNN69YNG)
# Generic Buy Now, Pay Later Project

## MAST30034 Project 2 README.md
# Group 1
- Zi Han Wu, 1266716
- Mei Hui Wang, 1266291
- Jinuo Sun, 1214174
- Yulin Dong, 1156680

**Research Goal:** The research goal is to find optimal propties for BNPL company to choose merchant, based on this properties to establish a comperhensive ranking system, and therefore found the top 100 merchants for paternership. 

**Timeline:** The timeline for the research area is 2021 to 2022. 20 months transaction in between merchants and consumers.  

# Pipeline
## Summary Notebooks
Summary notebook summaries the progress of the project, step through: dataset information --> feature prediction (fraud and next year) --> rank model --> result --> insight & recommendation --> limitation and assumption --> business benefit
Instruction: To run the summary notebook, should run all the main notebook first.

## Main Notebooks
To run the main noteboook pipeline, please visit the `notebook` directory and run the files in order:
1. `0. Data Download.py`: This notebook create the file path to store the curated data into 6 sub folders under the main `data/curated`. Moreover, it downloads the external data into the `data/external` directory. Also create `notebooks/extra` path to store additional work in this project.
2. `1. Data Reading.ipynb`: This notebook reads all internal datasets, including transaction, merchant, and consumer data. Data preprocessing and preliminary analysis have been conducted here. All newly generated data is stored in subfolders curated according to the data category.
3. `2. Consumer Preprocessing.ipynb`:  This notebook visualizes the consumer data.
4. `3. Merchant Preprocessing.ipynb`: This notebook visualizes the merchant data.
5. `4. Transaction Preprocessing.ipynb`: This notebook remove the noise and less interpreted data in the transaction data, and visualizes the transaction amount.
6. `5. Geospatial.ipynb`: This notebook process with external data and visualizes them into geospatial plot. 
7. `6. Consumer fraud prediction.ipynb`: This notebook predict the consumer fraud probability (safe, unsre, fraud).
8. `7. Merchant fraud prediction.ipynb`: This notebook predict the merchant fraud probability (safe, risky). 
8. `8. Merchant features model.ipynb`: This notebook predict the next year features that will use for ranking system. 
9. `9. Rank model.ipynb`: This notebook build the comperhensive ranking system to predict the top 100 merchans. 
11. `10. Segment trend.ipynb`: This notebook shows the five segment trends based on rank model, provide insight for BNPL to choose merchant. 

## Extra Notebooks
Extra notebooks are developed alongside the main notebook, but due to time constraints, they have not been finalized yet. They are primarily preparation work for the presentation, but may not add significant value if included in the main notebook.

1. For extra work we have considering noise detection due to there is 10% noise in the transaction data, however, due to time limit, it is not complish, the progress of noise detection is store in noise detection.ipynb. 
2. For presenatation preparetion, we have one extra notebook store all plots that we want to present in the presentation. 

# Guide to code
Run the code by the ordered notebooks, for each notebook, press 'run all' to get result, or run by each cell in order.

# Dataset Info
1. External Dataset store in `data/external`.
2. Internal Dataset store in `data/tables`.
3. Curated Dataset store in `data/curated`.   
- Sub section in curated dataset store all curated dataset for further process.
4. Predicted feature Dataset store in `data/predicted`.
5. Predicted top 100 merchant store in `data/final result`.

# Plots Info
All useful plots are store under `plots` folders.
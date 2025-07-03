# Data-Driven Market Expansion: Identifying High-Potential Banking Zones
This repository contains the supporting code for our master's thesis at the Barcelona School of Economics. 2024-2025

Group Members: Soledad Monge, María José Alemán and Marta Sala

# Project Overview
This project supports a leading global bank in identifying the 10 most attractive locations for new branch openings in Madrid and Cataluña, based on sociodemographic, business activity, and competition variables. We worked with municipality-level data and engineered relevant features—both in absolute terms (frequencies) and as population-adjusted ratios—focused on attributes of strategic interest to the bank, such as affluent individuals, professionals, and profitable businesses. Using Principal Component Analysis (PCA), we derived variable weights to construct a composite zone score that reflects each municipality’s alignment with the bank’s ideal expansion profile. Additionally, we applied the HDBSCAN clustering algorithm to uncover groups of municipalities with similar structural and commercial characteristics.

This thesis was done in collaboration with Deloitte, who have been kind enough to present us with this challenge, and who have taken on a guiding role throughout this project.


# Structure of repository
- The folder **`/data`** contains:
  - The original datasets provided by Deloitte, including sociodemographic and banking datasets. We were unable to upload the business data and shapefile because they exceed the size allowed on Git Hub, but you can access the file through this link: https://drive.google.com/drive/folders/1FqO2NVBoLpE6uLlmhYIPkJf8dN5UB8UW?usp=sharing)
  - The **processed datasets** generated in `main.ipynb`: `df_merged.csv`, `madrid.csv`, `cataluna.csv`, `municipalities_madrid.geojson` and `municipalities_cataluna.geojson`.
  - `municipality_map_dict.xlsx`: INE dictionary with municipality names

- The notebook **`main.ipynb`** contains the core workflow, including: data preprocessing and merging, Feature engineering, EDA, Zone score calculation and Clustering with HDBSCAN. 

- The notebook **`top10sectors.ipynb`** documents the methodology used to identify the top 10 economic sectors, including a ranking based on growth, size, profitability, and correlation with bank presence  




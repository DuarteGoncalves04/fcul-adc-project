# Analyzing Social Structures: Blogger Ego Networks on Google+ - A Complex Data Analysis Project

This repository contains our implementation and analysis of various bloggers ego networks from the late social media website google+, using Jupyter Notebook. This project was made for the course Complex Data Analysis at Faculty of Science of University of Lisbon (FCUL) on the year of 2024/2025.

---

## Table of Contents

1. [Overview](#overview)
2. [Project Structure](#project-structure) 
3. [Requirements](#requirements)
4. [Running the Project](#running-the-project) 
5. [Author and Contact](#author-and-contact)

---

## Overview

This project extracts and analyzes ego networks from a dataset by filtering users with a specific feature, in this case, the job title of "blogger." The extracted data is then transformed into network structures, allowing for further analysis of nodes, edges, and relationships.

---

## Project Structure

```
fcul-adc-project/
├─ docs/
|   ├─ Project_statement.txt // Statement
|   └─ Report_G3.pdf         // Final report
├─ code/
│   ├─ ADC_project.html  // Project in HTML
│   ├─ ADC_project.ipynb // Project in Jupyter Notebook
│   ├─ files/
│   │   ├─ gplus/
│   │   │   ├─ [EgoID].circles   // List of Circles and their Members in Ego Network [EgoID]
│   │   │   ├─ [EgoID].edges     // Edges connection in Ego Network [EgoID]
│   │   │   ├─ [EgoID].egofeat   // Features of the ego in Ego Network [EgoID]
│   │   │   ├─ [EgoID].feat      // Features of the members in Ego Network [EgoID]
│   │   │   ├─ [EgoID].featnames // All features names in Ego Network [EgoID]
│   │   │   ├─ [EgoID].followers // List of followers in Ego Network [EgoID] 
│   │   │   └─ ...
│   │   ├─ gplus_combined (Need Download) // Full dataset in TXT
│   │   └─ readme-Ego.txt    // ReadMe file of dataset
|   └─ output/
│       ├─ [EgoID]  // Information extracted from Ego Network [EgoID]
│       │   └─ ... 
│       └─ ...
└─ README.md // This file
```

---

## Requirements

- **Anaconda** 24.9.1+ (Tested in 24.9.1)
    Download from [Anaconda](https://www.anaconda.com/download/success)
- **Python** 3.11.10
    Download from [Python](https://www.python.org/downloads/)
- **NetworkX**
- **Pandas**
- **Matplotlib**

---

## Running the Project

**!!!ATTENTION!!!!**
The code will not work as it is, because its missing the "**gplus_combined.txt**" file. This file can be found at the [Stanford site](https://snap.stanford.edu/data/ego-Gplus.html), download it and insert it inside the files folder.

For full visualization of graphs **(At least +16Gb of RAM Required)**, comment the line:
```python
    if egoGraphs[i][1] == '107489144252174167638':
        continue
```

If everything is as demonstrated in Project Structure, than it may proceed to execution, however the project full execution may take more than 20 hours!

---
## Author and Contact

- **Duarte Gonçalves** - [duarte.dapg@gmail.com](mailto:duarte.dapg@gmail.com)
- **Enzo Chatalov** - [enzobchatalov@gmail.com](mailto:enzobchatalov@gmail.com)
- **Daniel Câmara**
- **Luís Reis**

For any questions or suggestions, feel free to open an issue or reach out by email. Pull requests to improve or extend the analysis are also welcome!

---






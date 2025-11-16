# README

## Overview
This repository provides a simple pipeline that converts a legal **PDF judgment** and **LLM-extracted entities** into a structured JSON file.  
The generated JSON file is then used by `index.html` to create the final visualization.

---

## How to Use

### 1. Run the `.ipynb` notebook first
- Open the Jupyter Notebook (e.g., `pipeline.ipynb`).
- Input:
  - **PDF file**
  - **Entities extracted using LLMs** (person, time, location, event, etc.)

Notebook saare processing steps run karega and at the end:

**Output:**  
data_X.json


---

### 2. Use the generated json file in the index.html file
- Take the generated `data_X.json`
- Place it in the same folder as `index.html`
- Start python server using:
    - **python3 -m http.server 8000**
    - Open the index.html file using the URL: **http://localhost:8000/index.html**
    - The page will automatically load `data_X.json` and generate the visualization.


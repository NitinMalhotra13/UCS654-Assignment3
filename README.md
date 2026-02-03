## TOPSIS Decision Making System

**Name:** Nitin Malhotra  
**Course:** UCS654 – Predictive Analytics  

---

## Live Web App

Streamlit Link:  
https://topsis-nitin-102303918.streamlit.app/

---

## About This Project

This project implements **TOPSIS (Technique for Order Preference by Similarity to Ideal Solution)** in three ways:

1. **Command Line Program (CLI)**
2. **Python Package on PyPI**
3. **Web Application using Streamlit**

TOPSIS is used to **rank options based on multiple criteria**.  
Higher score = better option.

---

## Folder Structure
UCS654-Assignment3/

├─ part1-cli/

├─ part2-package/

├─ part3-webservice/

└─ README.md

---

# Part 1 – CLI Program

### Run Command

`python topsis.py InputFile Weights Impacts OutputFile`

### Example

python topsis.py data.csv "1,1,1,1" "+,+,+,+" result.csv

### Checks Performed

- File must exist  
- Minimum 3 columns  
- First column = names  
- Other columns must be numbers  
- Criteria count = Weights count = Imapcts count 
- Impacts must be `+` or `-`  

---

## CLI Screenshots

**CLI Run**  
<img width="1663" height="93" alt="image" src="https://github.com/user-attachments/assets/ab04acd7-6435-4f3f-a4f8-fc43424e8690" />

**CLI Output File Example** 
<img width="777" height="266" alt="Screenshot 2026-02-03 213242" src="https://github.com/user-attachments/assets/f7341560-4881-45f6-8a00-83a7c5d2f102" />

---

# Part 2 – Python Package (PyPI)

### Package Name
topsis-nitin-102303918

### Install
`pip install topsis-nitin-102303918`

### Run Example
`topsis data.xlsx "1,1,1,1" "+,+,+,+" result.csv`

---

## PyPI Screenshots

**PyPI Page**  
<img width="1696" height="1025" alt="image" src="https://github.com/user-attachments/assets/b3074885-a7b9-4e60-a920-4c0fa6479335" />

---

# Part 3 – Web Application (Streamlit)

### Live Link
https://topsis-nitin-102303918.streamlit.app/

### Features

- Upload CSV or Excel file  
- Enter weights and impacts  
- Enter email  
- Result sent to email  
- No file saved on server  
- Dark theme UI  

---

## Web App Screenshots
**Home Page**  
<img width="1919" height="1144" alt="image" src="https://github.com/user-attachments/assets/aba7388a-f3b1-47a7-96ee-1991762659ef" />

**Form Submission**
<img width="1919" height="1136" alt="image" src="https://github.com/user-attachments/assets/e2ab3730-d948-4ac3-b46d-9628af4676e6" />


**Email Result**  
<img width="1420" height="554" alt="image" src="https://github.com/user-attachments/assets/97ef9d50-147c-4e58-9c49-2f38bf4f0d3d" />

---

# How TOPSIS Works (Simple)

1. Normalize values  
2. Apply weights  
3. Find best and worst values  
4. Measure distance  
5. Calculate score  
6. Rank options  

---

# Technologies Used

- Python  
- Pandas  
- NumPy  
- Streamlit  
- GitHub  
- PyPI  

---

# Run Web App Locally

`pip install streamlit pandas numpy openpyxl`

`streamlit run app.py`

---

# Security

Email credentials are stored using **environment variables / Streamlit secrets**, not in the code.

---

# Author

**Nitin Malhotra**

---

# License

For academic use only.

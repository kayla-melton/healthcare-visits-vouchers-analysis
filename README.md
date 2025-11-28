# 📊 Healthcare Visits & Vouchers Analysis  
*Data analytics project using Python, Pandas, and Jupyter Notebook*

---

## 🏥 Project Overview  
This project analyzes **clinic visits**, **voucher usage**, **patient demographics**, and **unpaid balances** to identify trends that influence healthcare costs and access.

You’ll find:  
- Cost comparisons across clinic types  
- Voucher expiration analysis  
- Visit trends by age and gender  
- Most common medical conditions  
- Actionable operational recommendations  

---

## 🏷️ Badges  
![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)  
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)  
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37726?logo=jupyter)  
![NumPy](https://img.shields.io/badge/NumPy-Scientific-013243?logo=numpy)  
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-11557C)  

---

## 📁 Project Structure  

```
Healthcare_Visits_Voucher_Project/
│
├── Data/
│   ├── Clinic_filled_utf.csv
│   ├── Patients_filled_utf_1.csv
│   ├── Medical_Condition_filled_utf.csv
│   ├── Visit_filled_utf.csv
│   ├── Visit_condition_filled_utf.csv
│   ├── Voucher_filled_utf.csv
│
├── Healthcare Visits Voucher Analysis.ipynb
└── README.md
```

---

## 🧠 Key Questions Answered  

### **1. Which clinic types are most expensive?**  
We compare average bills across **8 clinic types**.

### **2. Which patients visit the most?**  
We segment by **age group** and **gender**.

### **3. How many vouchers are at risk of expiring?**  
We examine expiration windows (180 days → expires soon).

### **4. What are the top medical conditions?**  
We analyze frequency counts.

### **5. Who carries the highest unpaid balances?**  
We look at clinic type, demographics, and visit counts.

---

## 🧭 Project Highlights  

### ⭐ Clean, well-structured healthcare dataset  
Merged from multiple tables: **patients**, **visits**, **vouchers**, **clinic**, **conditions**.

### ⭐ Advanced data transformations  
Including:  
- Joining tables  
- Creating age bands  
- Calculating expiration timelines  
- Aggregations by clinic type and gender  

### ⭐ Visual insights  
Multiple bar charts comparing:  
- Cost by clinic type  
- Unpaid balances  
- Visit counts  
- Age × gender trends  

### ⭐ Actionable business recommendations  
Built directly from insights.

---

## 📈 Mermaid Diagram — Project Flow  
*(GitHub renders this automatically!)*

```mermaid
flowchart LR
    A[Raw CSV files] --> B[Data Cleaning]
    B --> C[Feature Engineering]
    C --> D[Analysis & Aggregations]
    D --> E[Visualizations]
    E --> F[Final Insights & Recommendations]
```

---

## 📊 Key Insights

### **1. Visit Frequency by Patient**
Patients with **4+ visits** tend to:  
- Visit clinics more consistently  
- Accumulate higher unpaid balances  
- Appear in multiple clinic types  

### **2. Cost Differences by Clinic Type**

| Clinic Type       | Avg Total Bill |
|-------------------|----------------|
| **Surgery Center** | **$745** |
| **Hospital**       | **$549** |
| **Imaging Center** | **$490** |
| **Urgent Care**    | **$268** |
| **Medical Office** | **$245** |
| **Rehab Center**   | **$219** |
| **Clinic**         | **$212** |
| **Dental Clinic**  | **$170** |

**Surgery Centers** are the most expensive and have the **highest unpaid bills**.

### **3. Age × Gender Trends**
- Most visits occur in **two age bands**:  
  **0–17** and **18–34**  
- **Female patients** consistently have higher visit counts  
- **“Other” gender** group is smaller but steady across ages

---

## **4. Clinic Cost Comparison**

### **Average Visit Cost (Highest → Lowest)**

1. **Surgery Center** — *$745 average bill*  
2. **Hospital** — *$549 average bill*  
3. **Imaging Center** — *$490 average bill*  
4. **Urgent Care** — *$268 average bill*  
5. **Medical Office** — *$245 average bill*  
6. **Rehab Center** — *$219 average bill*  
7. **Clinic** — *$212 average bill*  
8. **Dental Clinic** — *$170 average bill*  

---

## **5. Gender-Based Healthcare Spending**
- Male patients spend **slightly more on average**.  
- Driven mostly by clinic types visited (e.g., Surgery Center).

---

## **6. Voucher Expiration Risk**
- Vouchers expire **180 days** after issue.  
- Patients with vouchers expiring in the next **30 days** should be prioritized for scheduling.

---

## **7. Most Common Medical Conditions**
The most frequent conditions include:  
- 🇨🇦 Flu  
- 💢 Back Pain  
- 🤧 Allergies  
- 🤕 Injury  
- 🦷 Dental issues  

## 🛠️ How to Run This Project

### **1️⃣ Clone the repository**
```bash
git clone https://github.com/kayla-melton/healthcare-visits-vouchers-analysis.git
```

### **2️⃣ Install required libraries**
```bash
pip install pandas numpy matplotlib jupyter
```

### **3️⃣ Launch Jupyter Notebook**
```bash
jupyter notebook
```

Open:  
[**Healthcare Visits Voucher Analysis.ipynb**](Healthcare%20Visits%20Voucher%20Analysis.ipynb)

### **4️⃣ Run each cell**
The notebook is organized into:  
- Data loading  
- Cleaning  
- Transformations  
- Analysis  
- Visualization  
- Recommendations  

---

## 💡 Business Recommendations

### **1. Prioritize Surgery Center & Hospital Collections**
They generate the **highest bills and highest unpaid balances**.

### **2. Automate Voucher Expiration Alerts**
Flag vouchers **30 days before expiration**.

### **3. Expand Youth & Young Adult Programs**
Most visits come from **0–17** and **18–34** age groups.

### **4. Balance Clinic Staffing Based on Peak Groups**
Females have the **highest visit volume**, especially in imaging + clinics.

### **5. Create a Standard Care Pathway for Top Conditions**
Focus on:  
- Flu  
- Back pain  
- Allergies  
- Dental issues

---
## 🧰 Skills Demonstrated

### 🔹 **Python for Data Analysis**
- Data wrangling with Pandas  
- Cleaning inconsistent and missing data  
- Merging multi-table healthcare datasets  
- Creating new calculated fields (age, expiration timelines, unpaid balances)

### 🔹 **Exploratory Data Analysis (EDA)**
- Groupby aggregations  
- Pivot-style summaries  
- Age band segmentation  
- Patient + clinic utilization patterns  
- Frequency counts of medical conditions  

### 🔹 **Visualization**
- Matplotlib bar charts and comparisons  
- Visualizing clinic costs, visit patterns, and demographic trends  
- Chart formatting and labeling for storytelling  

### 🔹 **Feature Engineering**
- Converting DOB → Age  
- Age band categorization  
- Voucher expiration windows  
- Cost per clinic type calculations  
- Joining visits + vouchers + conditions into a unified dataset  

### 🔹 **Business Analytics**
- Identifying high-cost clinics  
- Flagging expiring vouchers  
- Recognizing high-frequency patient groups  
- Recommending staffing + program improvements  
- Connecting data insights to operational decisions  

### 🔹 **Jupyter Notebook Workflow**
- Organized cells with narrative explanations  
- Reproducible code blocks  
- Clear visual storytelling through combined code + charts  

### 🔹 **Git & GitHub**
- Version control using Git  
- Organized project structure  
- README documentation + diagrams  
- GitHub-hosted notebook for recruiter review

---

## 📬 Contact

If you'd like to discuss this project or collaborate:

**Kayla Melton**  
📧 Email: kaylamelton22@icloud.com    
💼 LinkedIn: https://www.linkedin.com/in/jakayla-melton-001a782bb/  
🗂️ GitHub: https://github.com/kayla-melton  

---

## ⭐ If you found this project helpful…
Please consider giving the repo a **star**! ⭐


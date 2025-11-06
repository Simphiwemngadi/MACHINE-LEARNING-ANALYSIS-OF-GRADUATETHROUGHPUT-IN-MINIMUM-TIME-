# Machine Learning Analysis of Graduate Throughput  
### Bachelor of Engineering Technology in Civil Engineering  

## Overview  
This project examines the factors influencing how Civil Engineering students complete their degree in minimum time. Using machine learning methods, the study analyzes academic performance, demographic characteristics, and institutional data to identify the strongest predictors of student success.  

The aim is to provide data-driven insights that can help improve academic planning, student support, and overall graduate throughput rates within the Bachelor of Engineering Technology in Civil Engineering program.  

---

## Objectives  
- Combine and clean multiple institutional datasets into a single analytical file.  
- Conduct detailed exploratory data analysis (EDA) to understand relationships between student attributes and throughput.  
- Build predictive models that classify whether a student is likely to graduate in minimum time.  
- Identify and interpret the most influential variables affecting throughput outcomes.  

---

## Data Sources  
Three primary datasets were used in this study:  

1. **Applications.csv** – Contains applicant information including matric subjects, scores, and demographics.  
2. **Enrolments.csv** – Details on qualifications, faculties, and study progression.  
3. **Residence.csv** – Records of student accommodation and years in residence.  

All three datasets were merged using a unique student identifier to create an integrated dataset for analysis.  

---

## Data Preparation and Cleaning  
Key data preparation steps included:  
- Handling missing values using techniques such as **KNN imputation** and mode substitution.  
- Removing redundant features and columns with excessive missing data.  
- Encoding categorical variables using **binary** and **one-hot encoding** methods.  
- Creating new engineered features, including residence status (*In Residence* or *Not in Residence*).  
- Addressing class imbalance in the target variable (*Minimum Time*).  

---

## Exploratory Data Analysis (EDA)  
Extensive univariate and bivariate analyses were performed using **Seaborn** and **Matplotlib** to explore patterns in the data.  

Key findings include:  
- Strong relationships between **language**, **mathematics**, and **physical sciences** marks with throughput success.  
- Students’ **age at enrolment** and **years in residence** were associated with performance differences.  
- High school subject performance, particularly **Life Orientation** and **English**, also contributed meaningfully to throughput outcomes.  

---

## Machine Learning Approach  
The predictive modeling phase involved several steps:  

1. **Data Preparation**  
   - Feature scaling and dimensionality reduction using the Variance Threshold method.  

2. **Modeling**  
   - Implemented and compared multiple classifiers:  
     - XGBoost  
     - Random Forest  
     - Logistic Regression  

3. **Evaluation**  
   - Models were evaluated using metrics such as **accuracy**, **precision**, **recall**, and **AUC**.  

### Feature Importance  
XGBoost identified the following top predictors of throughput in minimum time:  
1. Other South African Language  
2. Physical Sciences  
3. Life Orientation  
4. English  
5. Gender  
6. Life Sciences  
7. Years in Residence  
8. Age at Enrolment  

These results demonstrate that both academic preparation and demographic factors influence completion time.  

---

## Tools and Technologies  
| Category | Tools Used |
|-----------|-------------|
| Programming | Python |
| Data Handling | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn, XGBoost |
| Imputation | KNNImputer |
| Feature Selection | VarianceThreshold |

---

## Results Summary  
The analysis showed that students with strong matric performance, particularly in science and mathematics, and those with stable residence conditions were more likely to complete their qualification in minimum time.  

The findings highlight the importance of academic preparedness and living environments as key determinants of success in tertiary education.  



## Author  
**Simphiwe Mngadi**  
Final-Year Student – Mathematical Sciences  
Cape Peninsula University of Technology  


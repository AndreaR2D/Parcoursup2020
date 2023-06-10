# Parcoursup2020

Dataset Link: https://data.enseignementsup-recherche.gouv.fr/explore/dataset/fr-esr-parcoursup_2020/table/?sort=tri

This dataset provides a list of all the programs available on Parcoursup 2020.
The provided data includes: Program name, level, degree, institution name, candidates count, ...

This project focuses on candidates profiling and the occupancy rate, with a specific emphasis on economics degrees in the Île-de-France region.

## 🛠 Tools used 
Excel, Python, PowerBI

## 🔍 Dataset exploration 

- 12 760 rows
- 115 fields / Types count: 
- Types occurence count:
  - int64:      47
  - float64:    46
  - object:     22

## 🎡 Data Cleaning
Quality checklist:
- Missing values
- Types
- Outliers
- Duplicates

Check results:
- Missing values: 
  - GPS coordinate missing x179
  - Capacity x1
  - Acces rate x234

- Types: Type casting needed
- Outliers: OK
- Duplicates: OK

Cleaning journal:
- Missing values:
  - Missing GPS: using the imputation method with a GPS DB
  - Capacity: Row delete
  - Acces rate: Replacing NaN with 0
- Types:
Typecasting
  - Float to Int ➡ Capacite; Candidats_Prop
  - Int to Object ➡ ID
  - Object to Float ➡ GPS_X & Y

## 🔍 EDA

- Schools types
- Candidates profiles
- Diplomas


## 🔍 Functionnal Analysis

On economics degrees in the Île-de-France region.

### EDA
- Candidates wishs and profiles
- Schools offers
- Admitted candidates
- Capacity
- Training count

### Occupency rate
Exploration of program occupancy rate:
- In number of students
- In percentage compared to capacity

### Selectivity
Measuring school selectivity with Access Rate

### Correlations

- Is selectivity a cause of under-enrollment in programs?
- Is the number of offers related to selectivity?
- Do candidates accept offers from selective institutions?

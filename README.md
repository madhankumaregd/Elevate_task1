# Elevate_task1
Medical Appointment Data Cleaning Project

## 📋 Project Overview
This project cleans and preprocesses the Medical Appointment No-Show dataset to prepare it for analysis.

## 📊 Dataset Information
- **Source**: Kaggle - Medical Appointment No Shows
- **Original Rows**: [Your count]
- **Original Columns**: 14
- **Final Rows**: [Your count]
- **Final Columns**: [Your count]

## 🛠️ Cleaning Steps Performed

### 1. Data Loading & Initial Exploration
- Loaded CSV file using pandas
- Checked basic info, shape, and data types
- Identified missing values and duplicates

### 2. Column Names Standardization
- Converted to lowercase
- Replaced hyphens with underscores
- Made names consistent

### 3. ID Columns Handling
- Converted `PatientId` and `AppointmentID` to strings
- Removed scientific notation

### 4. Date Processing
- Converted to datetime format
- Extracted date components:
  - Scheduled date
  - Appointment date
  - Scheduled time
  - Day of week
  - Month
- Calculated wait time (days)

### 5. Gender Standardization
- Converted to uppercase
- Handled invalid values
- Filled missing with mode

### 6. Age Cleaning
- Removed negative ages
- Capped unrealistic ages (>100)
- Created age groups:
  - 0-17, 18-34, 35-49, 50-64, 65-99, 100+

### 7. Neighbourhood Cleaning
- Standardized to title case
- Filled missing with 'Unknown'

### 8. Binary Columns
Ensured all are 0 or 1:
- Scholarship
- Hipertension
- Diabetes
- Alcoholism
- Handcap (capped at 4)
- SMS_received

### 9. No-Show Column
- Standardized to Yes/No
- Created binary column for analysis

### 10. Duplicate Removal
- Removed [X] duplicate rows
- Checked for near-duplicates

### 11. Missing Values
- Dropped rows with missing dates
- Filled categorical missing with mode/Unknown
- Filled numerical missing with 0

## 📈 Key Statistics

| Metric | Value |
|--------|-------|
| Total Patients | [count] |
| Total Appointments | [count] |
| Gender Distribution | F: [X]%, M: [Y]% |
| Average Age | [X] years |
| No-Show Rate | [X]% |
| Average Wait Time | [X] days |

## 📁 Files in this Repository

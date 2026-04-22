# SpendSmart - A Financial Awareness Tool
SpendSmart is a simple, browser‑based financial awareness tool designed to help users estimate their annual spending and compare it to median household income levels in Georgia (2025) based on three different household types: Family, Married‑Couple, or Nonfamily.

## Features

### **Household Type Selection**
The home page allows users to choose between the following household options:
- Family  
- Married‑Couple  
- Nonfamily  

Each selection displays the corresponding median income from the included JSON dataset whilst unlocking the appropriate calculator page for that household type.

### **Interactive Spending Calculator**
Each household page:
- Accepts user input for common annual expenses  
- Validates all fields (no empty values, no letters, no negatives, no leading zeros)  
- Calculates total spending  
- Compares spending to the user’s income  
- Displays warnings if:
  - Spending exceeds their annual income  
  - Savings fall below 20% of income  

### **Dynamic Table Generation**
After submission, a table is generated showing:
- Each expense category  
- Total annual spending  
- Percentage of income spent  
- Color‑coded financial health indicator via percentage
    - 🟢 Green — User spending < 80% of income
    - 🟠 Orange — User spending between 80% and 99%
    - 🔴 Red — User spending ≥ 100%

### **Data Driven Income Data**
Georgia median income values are loaded from a JSON Object based on data from https://data.census.gov/:
('AnalysisEngine/ga_census_data.json')

### **How to Run SpendSmart**
SpendSmart includes a VS Code launch configuration for the browser known Microsoft Edge.
1) Open the project folder in VS Code
2) Press F5 on your keyboard
3) The application will automatically open index.html in Microsoft Edge

No additional setup or dependencies are required.
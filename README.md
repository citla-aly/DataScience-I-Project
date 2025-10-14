# DataScience-I-Project
Comparative analysis of the financial structure and solvency of the insurance sector in EU countries: approach based on Solvency II indicators

1. Background and Motivation
As future actuaries, we are expected to ensure that the safety and soundness of insurance companies are not compromised, while as consumers, we rely on insurers to have sufficient capital to meet their obligations even under extreme scenarios. 
Since its implementation in 2016, the Solvency II Directive has been the basis of Europe’s insurance regulation, promoting financial stability, transparency, and policyholder protection through a risk-based framework. However, despite this uniform structure, significant differences persist among EU countries in terms of financial composition, solvency ratios, and capital management practices. Understanding and comparing these Solvency II indicators across the EU is not only essential for evaluating the sector’s financial strength and resilience, but also personally relevant for us as actuaries and consumers who depend on the reliability and solvency of the insurance system.

2. Project Objectives 
We have 2 main objectives, the first one being the exploratory analysis of the financial structure (assets, equity, technical provisions, etc.) and insurance activity (premiums, claims, expenses) over EU countries. It also examines how solvency has evolved over the years in relation to claims or operating expenses across these countries. 
Create visualizations to: i. Compare key indicators, such as: solvency, profitability, expense control within the European countries.  ii. Identify regional patterns in the insurance sector's financial indicators. 

3. Research Questions
 * How do solvency patterns vary across the European Union countries and does solvency impact the countries’ profitability?
 
* To what extent does the relationship between assets and liabilities correlate with premiums collected and claims paid across EU countries?

* To what extent does the financial structure and asset allocation (e.g., investments in bonds)  of insurers correlate with the volume of premiums collected across EU countries?

* Is there a relationship between the premiums earned in each country relative to their GDP?

5. Data Source
   
We are obtaining our datasets from the European Insurance and Occupational Pensions Authority. → https://www.eiopa.europa.eu/tools-and-data/insurance-statistics_en
This source provides statistical data and downloadable datasets about insurance companies in the EU / EEA. The data covers European (re)insurance undertakings and groups reporting regularly under Solvency II.
The main limitation we encountered relates to the methodology required to merge datasets and compute various ratios and measures from different databases, while maintaining an optimal data structure for analysis. However we are confident we can obtain the needed indicators.
Balance Sheet: https://register.eiopa.europa.eu/_layouts/15/download.aspx?SourceUrl=https://register.eiopa.europa.eu/Publications/Insurance%20Statistics/SA_Balance_Sheet.csv
Premiums, claims and expenses: https://register.eiopa.europa.eu/_layouts/15/download.aspx?SourceUrl=https://register.eiopa.europa.eu/Publications/Insurance%20Statistics/SA_Premiums_Claims_Expenses.csv
7. Data Description
Balance Sheet:  cvs format, yearly, size (22865, 8)
Variables:  (['Reporting country', 'Reference period', 'Undertaking type', 'Value', ‘Item name', 'Item code','Number of submissions (per reporting country, reference date and undertaking type)', 'Date of extraction (yyyymmdd)']

Premiums, claims and expenses: cvs format, yearly, size (24588, 8) 
Variables: ['Reporting country', 'Reference period', 'Item', 'Business type', 'Item code', 'Value', 'Date of extraction (yyyymmdd)', 'Number of submissions (per reporting country, reference date and undertaking type)'] 
Relevant variables for our analysis: 
'Reporting country', 'Reference period', ‘Item name (Balance Sheet)', 'Value (Balance Sheet)’ ,'Undertaking type', ‘Item name (PCE)', 'Value ( PCE)’ ,’Item name (Own Funds)', 'Value' ( Own Funds) 

Cleaning steps foreseed:
Handling Missing Values, depending on the context we will remove, or impute missing data to ensure consistency across the data bases.
Restructuring Data, reordering variables that are currently stored as values in a single column into separate columns.
Creating Variables of Interest, as our goal is to compare financial ratios and indicators we need to do the corresponding operations to get these new variables.
Outlier Treatment, we need to Identify and remove extreme or anomalous values that could distort results.
Removing Duplicates in case of existence.

# Solvency and Financial Structure in EU Insurance Markets: A Comparative Study Based on Solvency II Indicators
### Background and Motivation
As future actuaries, we are expected to ensure that the safety and soundness of insurance companies are not compromised, while as consumers, we rely on insurers to have sufficient capital to meet their obligations even under extreme scenarios. 
Since its implementation in 2016, the Solvency II Directive has been the basis of Europe’s insurance regulation, promoting financial stability, transparency, and policyholder protection through a risk-based framework. However, despite this uniform structure, significant differences persist among EU countries in terms of financial composition, solvency ratios, and capital management practices. Understanding and comparing these Solvency II indicators across the EU is not only essential for evaluating the sector’s financial strength and resilience, but also personally relevant for us as actuaries and consumers who depend on the reliability and solvency of the insurance system.
### Project Goals
We define the following **principal objectives**:
- Identify structural diversity in insurance markets.
- Examine differences in investment composition.
- Provide an evidence-based understanding of how national economic contexts shape distinct solvency and financial patterns, despite the presence of a common regulatory framework (Solvency II).
  
To accomplish the above mentioned objectives, we established the following **methodological objectives**:
-Exploratory Data Analysis (EDA): Perform a descriptive analysis of insurers’ financial structures detailed by quarterly performance, and conduct a univariate analysis of key variables.
  - Key variables include: Assets, Liabilities, Solvency Capital Requirement (SCR) ratio, Minimum Capital Requirement (MCR) ratio, etc.
-Development of Visual Tools: Produce visualizations that facilitate interpretation and highlight key differences across countries and over time.
  - Visualization types: maps, histograms, correlation matrices, scatter charts, and comparative plots.
  - Time Horizon: The analysis will cover the period from 2017 to 2024.

### Research questions
Trying to connect the previous ideas about how financial structure affects solvency and profitability, and how these dimensions relate to each other, we construct the following research questions:
- How do solvency patterns vary across European Union countries, and to what extent does solvency influence the profitability of their insurance sectors?
- How do the levels of insurers’ assets and liabilities correlate with country-level premiums written and claims incurred across EU insurance markets?
- How does the financial structure and asset allocation of insurers (e.g., the share of investments in bonds) correlate with the volume of premiums collected across EU countries?
  
We are obtaining our datasets from the European Insurance and Occupational Pensions Authority. → https://www.eiopa.europa.eu/tools-and-data/insurance-statistics_en
This source provides statistical data and downloadable datasets about insurance companies in the EU / EEA. The data covers European (re)insurance undertakings and groups reporting regularly under Solvency II. 

The main limitation we encountered relates to the methodology required to merge datasets and compute various ratios and measures from different databases, while maintaining an optimal data structure for analysis. However we are confident we can obtain the needed indicators.
- **Balance Sheet**
- **Premiums, claims and expenses**
- **Own Funds**

### Project Structure
The HTML report is organized as follow. Section 1 is composed of the project goals, the related work and presents the 3 research questions. Section 2 reviews the related work. Section 2 includes the Data, with Section 2.1 detailing the dataset alongside the preprocessing and data-cleaning procedures. Sections 3.1, 3.2, and 3.3 then present the analyses corresponding to Research Questions 1, 2, and 3. Finally, Section 4 concludes the study by summarising the key findings from the perspective of both insurers and consumers. 

### How to run the code
- Clone the repository
- Install dependencies, inside DataScience-I-Project:  pip install -r requirements.txt
- Render report: quarto render "path where the repository was cloned" + /DataScience-I-Project/final_l.qmd
- To shows all file size information: ls -lh final_l.html
  
Open file:

- To open the HTML file in Linux: xdg-open final_l.html
- To open the HTML file in Windows : start final_l.html





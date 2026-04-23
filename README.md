# Public Finance Fiscal Analysis Model

## Overview

This project analyses political party manifestos sing data from party manifesto's. 

The goal is to help voters understand:

- The **real cost** of election promises
- The impact of such politices on **state finances**
- Which policies are **sustainable & not**

---

## Data Sources

- Tamil Nadu Budget Analysis (2025-26)
- Party Manifestos
- Cenus 2011
- Government scheme benchmarks

---

## Methodology

### 1. Population Estimation

The population estimation was done based on census 2011, It was adjusted using a +10% growth factor to reflect real population changes. Primary purpose of this data is estimate the number of policy beneficiaries

--- 

### 2. Cost Estimation 

Each policy is modeled using 

Total cost = (Target Population * Unit Cost) / 1,00,00,000

Unit costs are benchmarked, extracted and derived from chatgpt using the following resources

- Existing government branches
- Market benchmarks 
- Policy approximations

--- 

### 3. Fiscal Impact Model

`Annual Cost = Total Cost / Timeframe`

`Fiscal Impact = Annual Cost * Fiscal Sign`

Where:

| Impact Type | Sign |
|------------|------|
| Expense Increase | -1 |
| Expense Decrease | +1 |
| Revenue Increase | +1 |
| Revenue Decrease | -1 |
| Neutral | 0 |

### 4. Standardization

`% of GDP = Fiscal Impact / State GDP`

Tamil Nadu GDP used:
**Rs. 35,656,000,000**

--- 

## Output Metrics

At the party level, the model handles

- Total Fiscal Impact
- % of GDP
- Average Policy Score
- Risk Level

---
## Limitations & Margin of Error

- Since manifesots lack detailed implementation clarity, it is hard to come up with accurate estimates
- Some costs are estimated by relevant proxy schemes across the nation
- Policies that change the structure are difficult to quanitfy, and thus increases the error margin
- Population estimates are based on approximations, real population might be higher or lower than the estimated value

Estimated Margin of Error: Upwards of **25-30%** 

--- 

### AI Disclosure

ChatGPT was used for the following purpose

- Extracting policy information
- Benchmarking costs using comparable government schemes
- Documentation support


---

### How to Contribute

1. Forth the repository
2. Create a new branch
3. Make your changes
4. Commit your changes to the new branch
6. Open a pull request

### Guidelines to Contributors

I request you to keep changes clear & well documented, maintain consistency in design and units. Since this project aims to promote transparent analysis. Contributors that will improve clarity and accuracy are highly encouraged

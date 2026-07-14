# Life Insurance Block Valuation & Experience Monitoring Model
 
A whole life insurance valuation model built in Excel — pricing, reserving, and
experience monitoring for a small block of policies.
 
## Goals
 
- Build a life insurance model from real actuarial data and formulas, not templates
- Understand and apply core actuarial concepts: net premium pricing, reserve
  roll-forwards, and experience monitoring (A/E analysis)
- Be able to explain every part of the model end-to-end
## Data used
 
- **2017 CSO Select & Ultimate mortality table** (from mort.soa.org), 5% interest
- Two anchor policies used throughout for comparison:
| Policy | Issue Age | Sex | Face Amount |
|---|---|---|---|
| POL1015 | 27 | Female | $250,000 |
| POL1014 | 42 | Male | $100,000 |
 
## What's done
 
- Imported the 2017 CSO mortality table and built lookup logic for select/ultimate rates
- Built a 20-policy seriatim block with age/duration-based mortality lookups
- Calculated net premiums using the equivalence principle
- Built year-by-year projections (survival probabilities, discount factors, insurance
  and annuity values)
- Built a reserve roll-forward for POL1015
- Simulated 5,000 policy-years of mortality experience and built an A/E (Actual vs.
  Expected) dashboard by age band and duration band
## What's in each sheet
 
| Sheet | What it contains |
|---|---|
| README | In-workbook overview |
| Mortality_Table_Male / Female | 2017 CSO Select & Ultimate mortality rates |
| Lapse_Assumptions | Lapse rates by policy duration |
| Expense_Assumptions | Expense assumptions used in pricing |
| Policy_Data | The 20-policy block, with mortality lookups |
| Premium Calculation | Net premium calculation and projections for both anchor policies |
| Reserve Calculation | Reserve roll-forward for POL1015 |
| Experience Study | Mortality tracking for the anchor policies |
| Experience_Study_Synthetic | 5,000 simulated policy-years used for the A/E dashboard |
 
## Tools
 
Built in Microsoft Excel. Mortality data from the Society of Actuaries'
[mort.soa.org](https://mort.soa.org).

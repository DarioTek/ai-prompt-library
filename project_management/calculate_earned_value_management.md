# Calculate Earned Value Management
A software development project has a $100K budget and a timeline for 6 months. After 3 months, the actual cost (AC) is $60K and the project is 50% complete.

Am I over or under budget? Behind or ahead of schedule? And what is the earned value (EV), estimate to complete (ETC), and value added control (VAC).
Show this in a table format and highlight the explanation in bold.

Generate GitHub-Flavored Markdown suitable for VS Code Preview. Generate a downloadable .md file.
 
Use:
- Markdown headings
- Markdown tables (not code fences)
- Bold totals and key numbers
- Bullet points for recommendations
- No HTML unless needed for styling

### Sample Respose (from Microsoft Copilot)
# Earned Value Management (EVM) Analysis

## Project Information

| Item | Value |
|------|------:|
| Budget at Completion (BAC) | $100,000 |
| Project Duration | 6 Months |
| Current Time Elapsed | 3 Months |
| Actual Cost (AC) | $60,000 |
| Actual Progress | 50% Complete |

## EVM Calculations and Definitions

| Metric | Definition | Formula | Result |
|---------|------------|---------|---------:|
| BAC (Budget at Completion) | Total approved project budget. | Given | **$100,000** |
| PV (Planned Value) | Budgeted value of work scheduled to be completed by the status date. | Planned % × BAC | **$50,000** |
| EV (Earned Value) | Budgeted value of the work actually completed. | Actual % Complete × BAC | **$50,000** |
| AC (Actual Cost) | Actual amount spent on the project to date. | Given | **$60,000** |
| CV (Cost Variance) | Difference between earned value and actual cost. Indicates budget performance. | EV − AC | **−$10,000** |
| SV (Schedule Variance) | Difference between earned value and planned value. Indicates schedule performance. | EV − PV | **$0** |
| CPI (Cost Performance Index) | Measures cost efficiency. For every $1 spent, how much value is earned. | EV ÷ AC | **0.83** |
| SPI (Schedule Performance Index) | Measures schedule efficiency. | EV ÷ PV | **1.00** |
| ETC (Estimate to Complete) | Estimated additional cost required to finish remaining work. | (BAC − EV) ÷ CPI | **$60,000** |
| EAC (Estimate at Completion) | Forecasted total project cost at completion. | AC + ETC | **$120,000** |
| VAC (Variance at Completion) | Expected budget surplus or deficit at project completion. | BAC − EAC | **−$20,000** |

## Project Health Summary

| Question | Answer |
|----------|--------|
| Over or Under Budget? | **Over budget by $10,000 because AC ($60,000) exceeds EV ($50,000).** |
| Ahead or Behind Schedule? | **On schedule because EV equals PV ($50,000) and SPI = 1.00.** |
| Earned Value (EV) | **$50,000** |
| Estimate to Complete (ETC) | **Approximately $60,000 additional funding is required to finish the project if current cost performance continues.** |
| Variance at Completion (VAC) | **−$20,000, indicating the project is forecasted to finish over budget.** |

## Quick Interpretation Guide

| Metric | Interpretation |
|--------|----------------|
| **CV > 0** | Under Budget |
| **CV < 0** | Over Budget |
| **SV > 0** | Ahead of Schedule |
| **SV < 0** | Behind Schedule |
| **CPI > 1** | Cost Efficient |
| **CPI < 1** | Cost Overrun |
| **SPI > 1** | Progressing Faster Than Planned |
| **SPI < 1** | Progressing Slower Than Planned |
| **VAC > 0** | Expected Budget Surplus |
| **VAC < 0** | Expected Budget Deficit |

## Recommendations

- Monitor project spending closely to improve the Cost Performance Index (CPI).
- Investigate the causes of the current cost overrun.
- Implement cost-control measures for the remaining work.
- Continue maintaining schedule performance since the project is currently on track.
- Reforecast project costs regularly to validate the current EAC and VAC estimates.

## Conclusion

**The project is currently over budget because it has spent $60,000 while earning only $50,000 worth of completed work (CPI = 0.83 and CV = −$10,000). However, it is exactly on schedule because the Earned Value equals the Planned Value (SV = $0 and SPI = 1.00). If the current spending trend continues, the project is forecasted to complete at approximately $120,000, resulting in a Variance at Completion (VAC) of −$20,000.**

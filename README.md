# T06 – Expense Claim Policy Checker

**Student:** Arpit Gupta  
**Programme:** MBA (DS & DA), SCIT  
**Task ID:** T06  
**Theme:** A. No-code apps & dashboards

## Project Overview

The **Expense Claim Policy Checker** is a no-code Excel-based solution designed to automatically check expense claims against applicable travel and expense policy rules.

The checker processes **400 expense claims** and identifies whether a claim is compliant with the checked rules or has one or more policy violations.

## Solution Approach

The project follows these steps:

1. Profile the expense-claim data and identify which policy rules can be checked using the available fields.  
2. Convert the applicable policy rules into Excel-based checks.  
3. Store policy thresholds and parameters separately in the `Parameters` sheet.  
4. Apply the checker across all 400 claims.  
5. Verify the logic using test cases and independent reconciliation.  
6. Manually audit 30 flagged claims.  
7. Summarise the findings and recommendations for the CFO.

The checker is built using **Excel formulas only** and does not use macros.

## Key Results

- **Total claims:** 400  
- **Flagged claims:** 231  
- **Compliant claims:** 169  
- **Total rule flags:** 279  
- **Flagged claim value:** ₹14,53,124  
- **Test cases:** 55  
- **Test cases passed:** 55/55  
- **Manual audit sample:** 30 flagged claims  
- **Confirmed false alarms:** 0  
- **Cannot verify:** 14 of 30 audited flags

The audit results are reported with appropriate limitations because some policy checks depend on information that is not available in the claim data.

## Rule Coverage

The checker covers **8 of the 15 policy rules** based on the available claim fields.

Four checked rules are treated as definite-basis checks, while four depend on assumptions or information that is not recorded in the claim row.

The remaining seven rules are not checked because the required fields are unavailable in the provided dataset.

## Workbook Structure

The Excel workbook contains the following key sheets:

- **Claims** – original expense-claim data  
- **Parameters** – policy thresholds and configurable values  
- **Checker** – rule-by-rule automated checking  
- **Summary** – overall results  
- **Analytics** – analysis of violations and flagged values  
- **Audit** – manual audit of selected flagged claims  
- **Verification** – reconciliation and independent checks  
- **Test\_Cases** – boundary and functional test cases  
- **CFO\_Summary** – management-level findings  
- **Final\_Results** – final checker outputs  
- **AI Use Log** – documentation of AI assistance and iterations

## Verification

The solution was verified through:

- 55 test cases, including synthetic boundary cases  
- Reconciliation checks  
- Independent recalculation  
- Cross-checking of summary and analytics values  
- Manual audit of 30 flagged claims

All 55 test cases passed, and the reconciliation checks reported zero differences.

## Audit & Limitations

The manual audit was performed by the author against the policy text and available claim fields.

Some flagged claims could not be conclusively verified because the dataset does not contain information such as:

- Number of hotel nights  
- Number of meal/DA days  
- Late-booking approval  
- Train class  
- Cab type  
- International-travel approvals  
- Personal-extension details  
- Approval-chain information  
- Cancellation information  
- Traveller/relationship information

Therefore, a **0% confirmed false-alarm rate should not be interpreted as proof that the overall checker has no false alarms**.

## AI Use

Claude was used during the project for activities such as:

- Translating policy text into rule logic  
- Assisting with Excel formulas  
- Drafting and reviewing test cases  
- Independent recalculation/checking  
- Challenging assumptions and audit methodology  
- Reflection on the final approach

Final decisions regarding assumptions, audit verdicts and interpretation remained with the author.

Demo Video

The project demonstration video is available here:  
[**(https\://drive.google.com/file/d/1D7mAORhD7cBGRs6ZUrdremaER7XQdWwf/view?usp=sharing)**](https://drive.google.com/file/d/1D7mAORhD7cBGRs6ZUrdremaER7XQdWwf/view?usp=sharing)

## Files

- `T06_Arpit_Gupta.xlsx` – complete Excel-based checker and analysis  
- `T06_Arpit_Gupta.docx` – project report

## Author

**Arpit Gupta**  
MBA (DS & DA) | SCIT  
Task T06 – Expense Claim Policy Checker
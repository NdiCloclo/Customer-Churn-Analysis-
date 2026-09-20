# HealthConnect Clinic Analytics — Week 7

## Project Overview

Week 7 focuses on validation, KPI refinement, and decision support for the HealthConnect Clinic appointment no-show analysis.

The objective is to strengthen the interpretation of Week 6 findings, improve consistency between Analytics and Data Science, and define additional validation steps for future analysis.

## Key Findings

* **Attendance Rate:** 46.28%
* **Overall No-Show Rate:** 48.46%
* **Cancelled Appointments:** 5.26%
* **No-Show Rate (Attended vs No-Show Only):** Approximately 51.15%
* **Follow-up No-Show Rate:** 51.23%

### Reminder Channel Analysis

* Email: 48.41%
* No Reminder: 51.39%
* SMS: 45.75%
* WhatsApp: 49.77%

Reminder-channel differences represent observational associations and should not be interpreted as proof of causation.

### Main Analytical Insights

1. Previous no-show history appears to be a relevant candidate factor for future no-show behavior.
2. Follow-up appointments require additional investigation because of their relatively high no-show rate.
3. Reminder coverage and missing reminder-channel values should be reviewed.
4. Distance to the clinic and waiting time did not show clear relationships with appointment attendance.
5. KPI definitions and denominator rules must be standardized across analytical tracks.

## Week 7 Validation Status

The planned Power BI validation tests included:

* Outcome count reconciliation.
* Percentage reconciliation.
* Follow-up appointment filter testing.
* Dashboard verification against source data.

**Status:** Pending.

The DAX measures created for the reconciliation test caused instability in the Power BI table visual. Consequently, no successful validation result is claimed without supporting Power BI evidence.

## Recommendations

1. Prioritize patients with repeated no-show history for proactive follow-up.
2. Improve the completeness of reminder-channel data.
3. Compare reminder performance across appointment types.
4. Standardize KPI definitions and denominator rules.
5. Complete the Power BI validation tests after resolving the DAX issue.

## Cross-Track Collaboration

The Analytics and Data Science tracks used different approaches to handling cancelled appointments and missing reminder-channel values.

Data Science excluded 263 cancelled appointments before comparing attended and no-show outcomes, while Analytics retained cancelled appointments in the primary dataset. These differences highlight the need for shared population definitions and consistent analytical methods.

## Limitations

* The analysis is observational and does not establish causation.
* Missing values may affect reminder-channel comparisons.
* Differences in cancelled-appointment treatment can change KPI results.
* Small population segments require additional verification.
* The analysis is not a production predictive model.

## Conclusion

Week 7 builds on the HealthConnect Clinic Analytics project by emphasizing KPI consistency, cross-track collaboration, and validation. The existing findings provide useful directions for operational decision-making, while the pending Power BI tests represent the next step toward a more reliable analytical workflow.

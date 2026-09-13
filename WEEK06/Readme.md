# HealthConnect Clinic — Week 6

## Advanced Analytics & Decision Support

### Project Overview

Week 6 builds on the Week 5 HealthConnect analysis by moving from initial exploration toward deeper validation, segmentation, and decision support.

The analysis focuses on the strongest Week 5 findings, particularly previous no-show history, reminder patterns, and appointment type.

## Objectives

- Validate the most important Week 5 findings.
- Investigate patterns across relevant patient and appointment segments.
- Analyse factors associated with attendance and no-shows.
- Validate and refine key KPIs.
- Translate analytical findings into actionable business recommendations.
- Provide relevant analytical evidence to the Data Science track.

## Key Findings

- **Attendance Rate:** 46.28%
- **Overall No-Show Rate:** 48.46%
- **Cancelled Appointments:** 5.26%
- **Follow-up No-Show Rate:** 51.23%
- **Attended vs No-Show No-Show Rate:** 51.15%
- No-show rates generally increase as previous no-show history increases, reaching approximately 97% for patients with five previous no-shows in the displayed analysis.
- **No Reminder** has the highest overall no-show rate among the displayed reminder categories at 51.39%.
- Reminder performance varies across appointment types, meaning no single reminder channel can be considered universally optimal.
- Distance to clinic and waiting time did not show meaningful relationships with appointment outcome in the previous analysis.

## Cross-Track Validation

A collaboration with the Data Science track identified a methodological difference in the treatment of cancelled appointments.

Data Science excluded **263 Cancelled appointments** before comparing Attended and No-show outcomes, while the Data Analytics analysis retained them in the primary dataset.

This difference affects the denominator and therefore the resulting no-show and reminder estimates. The Data Science analysis found an approximately **5-percentage-point difference** in no-show rate between reminder conditions after excluding Cancelled appointments.

The Week 6 analysis therefore treats reminder status as an observed association rather than causal evidence and explicitly distinguishes between analyses that include or exclude Cancelled appointments.

## Business Recommendations

1. Prioritize patients with repeated previous no-shows for targeted intervention.
2. Strengthen reminder coverage and monitor outcomes by reminder channel.
3. Evaluate reminder strategies by appointment type rather than applying one channel universally.
4. Investigate the factors contributing to elevated no-show rates among Follow-up appointments.
5. Maintain clear and consistent KPI definitions when comparing analyses.

## Limitations

- The analysis is observational and does not establish causality.
- Extreme previous no-show groups may contain fewer observations and require further validation.
- Reminder-channel comparisons may be influenced by differences between patient and appointment groups.
- Missing values and unavailable variables introduce some uncertainty.
- Week 6 provides decision support and validation rather than a production predictive model.

## Week 7 Testing Priorities

- Validate the relationship between previous no-show history and future no-shows.
- Reassess reminder performance using a consistent outcome definition.
- Test whether the Follow-up no-show pattern persists across relevant segments.
- Monitor KPI trends and verify dashboard calculations against the underlying data.
- Share validated analytical findings and candidate variables with Data Science.

## Tools

- Python / Jupyter Notebook
- Power BI
- DAX
- CSV

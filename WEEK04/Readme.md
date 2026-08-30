HealthConnect Clinic  Appointment Attendance Analysis

Overview

This project explores appointment data from HealthConnect Clinic, a fictional healthcare clinic, to better understand patterns associated with appointment attendance and no-shows.

The analysis focuses on factors such as appointment characteristics, reminders, previous no-shows, waiting time and distance from the clinic.

Key Questions

- Does appointment type relate to appointment outcomes?
- Do reminders influence appointment attendance?
- Which reminder channels are associated with higher attendance?
- Do previous no-shows relate to future appointment outcomes?
- Does distance from the clinic relate to attendance?

Initial Findings

The dataset contains 5,000 records and 18 variables.

During the initial data quality assessment, "reminder_channel" had 1,366 missing values (27.32%). Further investigation showed that all of these records corresponded to appointments where no reminder was sent, indicating structural missingness rather than unexplained missing data.

Tools

- Python
- Pandas
- JupyterLab
- Matplotlib

Project Status

In progress. The next stages will focus on deeper exploratory analysis, visualisation and identifying patterns that could support recommendations for improving appointment attendance.

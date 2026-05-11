**Work in Progress**  
> This repository contains ongoing work for a master’s thesis.  
> The data, code, and documentation are still being refined and may change.

# Student Politics as a Pathway to Parliament: A Case Study from the University of Iceland, 1931–2024

Master’s thesis completed as part of the M.A. in Quantitative Methods for the Social Sciences at Columbia University.

## Abstract
Political pathways into national office shape who becomes part of the political elite and whose
interests and experiences are represented in democratic institutions. This study provides the first
empirical examination of whether leadership in student politics at the University of Iceland is
associated with subsequent entry into parliament between 1931 and 2024. Using an original
longitudinal dataset of 856 student political leaders, compiled from archived student newspapers
and parliamentary records, the study analyzes parliamentary entry through logistic regression and
Cox proportional hazards models. The results present evidence of a systematic relationship,
suggesting that student politics may serve as an early-stage pathway into national office. Of the
856 individuals subject to analysis, 67 entered Alþingi at some point, at any capacity, between
1931 and 2025, yielding **a total parliamentary entry rate of 7.8%**, substantially higher than the
estimated 0.34% parliamentary participation in the general population. Cohort effects dominate
the results, with later cohorts generally less likely to enter parliament and tending to do so later
than those in the earliest cohort. Associations and gender do not display a consistent statistically
significant relationship with parliamentary entry in the multivariable models. **The findings
suggest that student politics at the University of Iceland functioned as a pathway into national
political office during the period of analysis.**

## Data
An original dataset was compiled from two primary sources: archived student publications available via [*timarit.is*](https://timarit.is/), and parliamentary records from the [*althingi.is*](https://www.althingi.is/altext/cv/is/?cstafur=S) biographies pages.

Refer to the [*source inventory*](data/documentation/source_inventory.md) for an exhaustive list of sources.

## Data Construction
The dataset was constructed by identifying individuals who ran for either the student council or the university council at the University of Iceland between 1931 and 2024. 

Individuals were matched to parliamentary records using the biographies to determine whether and when they entered national office.

Only individuals who ran for council were included in the analytical sample to ensure comparability. Individuals holding positions without candidacy (e.g., board-only roles) were excluded.

## Data Description
| Variable               | Description                                                     | Type        |
|----------------------|-----------------------------------------------------------------|------------|
| name                 | Full name of individual                                         | Identifier |
| student_association  | Student political association affiliation                       | Categorical|
| year_student_pol     | Last year of participation in student politics                  | Numeric    |
| student_year_decade  | Decade of student political activity                            | Categorical|
| cohort               | Aggregated historical cohort (e.g., 1930s–1950s)                | Categorical|
| position             | Role in student association (e.g., Chairman, Board Member)      | Categorical|
| gender               | Gender of individual (m/f)                                      | Binary     |
| ran_for_council      | Ran for student or university council (1 = yes, 0 = no)         | Binary     |
| ticket_position      | Position on electoral list (1–5; 99 = missing/NA)               | Ordinal    |
| student_council      | Candidate for student council (1 = yes, 0 = no)                 | Binary     |
| university_council   | Candidate for university council (1 = yes, 0 = no)              | Binary     |
| parliamentarian      | Entered national parliament (1 = yes, 0 = no)                   | Binary     |
| minister             | Became minister (1 = yes, 0 = no)                               | Binary     |
| party                | Political party affiliation (if applicable)                     | Categorical|
| year_parliament      | Year of entry into parliament                                   | Numeric    |

**Notes:**
- Value `99` indicates missing or not applicable.
- The analytical sample includes only individuals who ran for student or university council.
- Final sample size: N = 856; parliamentary entries: 67.

## Sample Composition
| Outcome              | N   | %      |
|---------------------|-----|--------|
| Parliamentarian     | 67  | 7.83%  |
| Not parliamentarian | 789 | 92.17% |
| Total               | 856 | 100%   |

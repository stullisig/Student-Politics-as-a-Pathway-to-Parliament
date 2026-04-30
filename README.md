**Work in Progress**  
> This repository contains ongoing work for a master’s thesis.  
> The data, code, and documentation are still being refined and may change.

# Student Politics as a Pathway to Parliament: A Case Study from the University of Iceland, 1931–2024

Master’s thesis completed as part of the M.A. in Quantitative Methods for the Social Sciences at Columbia University.

## Abstract
Blablabla

## Data
An original dataset was compiled from two primary sources: archived student publications available via [timarit.is](https://timarit.is/), and parliamentary records from the [althingi.is](https://www.althingi.is/altext/cv/is/?cstafur=S) biographies pages.

Refer to _____ for an exhaustive list of sources.

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

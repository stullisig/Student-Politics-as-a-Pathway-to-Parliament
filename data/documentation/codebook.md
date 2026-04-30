# Codebook

## Data Description

| Variable              | Description                                                     | Type         |
|----------------------|-----------------------------------------------------------------|-------------|
| name                 | Full name of individual                                         | Identifier  |
| student_association  | Student political association affiliation                       | Categorical |
| year_student_pol     | Last year of participation in student politics                  | Numeric     |
| student_year_decade  | Decade of student political activity                            | Categorical |
| cohort               | Aggregated historical cohort (e.g., 1930s–1950s)                | Categorical |
| position             | Role in student association (e.g., Chairman, Board Member)      | Categorical |
| gender               | Gender of individual (m/f)                                      | Binary      |
| ran_for_council      | Ran for student or university council (1 = yes, 0 = no)         | Binary      |
| ticket_position      | Position on electoral list (1–5; 99 = missing/NA)               | Ordinal     |
| student_council      | Candidate for student council (1 = yes, 0 = no)                 | Binary      |
| university_council   | Candidate for university council (1 = yes, 0 = no)              | Binary      |
| parliamentarian      | Entered national parliament (1 = yes, 0 = no)                   | Binary      |
| minister             | Became minister (1 = yes, 0 = no)                               | Binary      |
| party                | Political party affiliation (if applicable)                     | Categorical |
| year_parliament      | Year of entry into parliament                                   | Numeric     |

## Notes

- Value `99` indicates missing or not applicable.
- The analytical sample includes only individuals who ran for student or university council.
- Final sample size: N = 856; parliamentary entries: 67.

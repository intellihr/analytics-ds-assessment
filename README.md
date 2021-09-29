# Analytics Data Science Assessment


## Background

Company **XYZ** maintains their employee data in an Excel spreadsheet, and one day, **Tony**, the boss of Company XYZ, was told by his friend **Ady** that how data is like the new Gold in the recent era and there are many cool things he can potentially do with any data that he owns.

Tony has got excited by this idea and decided to hire you as the data scientist to help him dig out important insights from the employee data of his company.


## Data Specification

The employee data of Company XYZ can be found in `dataset.xlsx` file.

The file contains 7 sheets, and each sheet contains a different part of the employee data. The definition of each of the sheet are listed below.


### people

This sheet contains basic personal information of the employees.

| Column Name | Description |
| ----------- | ----------- |
| person_id   | person / employee identifier |
| first_name  | employee first name |
| last_name   | employee last name |
| dob | date of birth |
| gender | employee gender |


### jobs

This sheet contains basic job related information of the employees. This sheet can be linked to the `people` sheet using the `person_id` column.

| Column Name | Description |
| ----------- | ----------- |
| job_id   | employee job identifier |
| person_id | person / employee identifier |
| job_start | the date the employee started the job |
| job_end | the date the employee ended the job |


### pay_grade

This sheet contains the pay grade information associated with the jobs. This sheet can be linked to the `job` sheet using the `job_id` column.

| Column Name | Description |
| ----------- | ----------- |
| job_id   | employee job identifier |
| effective_dates | the start date (inclusive) and end date (exclusive) of the pay grade associated with the job |
| pay_grade_name | the pay grade type / name |


### work_types

This sheet contains the work type information associated with the jobs. This sheet can be linked to the `job` sheet using the `job_id` column.

| Column Name | Description |
| ----------- | ----------- |
| job_id   | employee job identifier |
| effective_dates | the start date (inclusive) and end date (exclusive) of the work type associated with the job |
| work_type_name | the name of the work type |


### location

This sheet contains the location information associated with the jobs. This sheet can be linked to the `job` sheet using the `job_id` column.

| Column Name | Description |
| ----------- | ----------- |
| job_id   | employee job identifier |
| effective_dates | the start date (inclusive) and end date (exclusive) of the location information associated with the job |
| location_name | the name of the location |
| location_id | the location identifier |
| parent_location_id | the identifier of the parent location |


### salary

This sheet contains the salary information associated with the jobs. This sheet can be linked to the `job` sheet using the `job_id` column.

| Column Name | Description |
| ----------- | ----------- |
| job_id   | employee job identifier |
| effective_dates | the start date (inclusive) and end date (exclusive) of the salary amount associated with the job |
| salary | the salary amount (in AUD) |


### happiness rating

This sheet contains the employee happiness rating response data that are obtained by recurrent surveys sent to the employees at a regular base. This sheet can be linked to the `job` sheet using the `job_id` column.

| Column Name | Description |
| ----------- | ----------- |
| job_id   | employee job identifier |
| rated_at | the time when the employee submitted the rating |
| happiness_rating | employee's happiness rating response, the rating scale is set to be 1 to 10 (where 1 is very unhappy and 10 is super happy) |


## Tasks

**Tony**, the business owner is **NOT** very techy and data savvy, however, he is really keen to know more about the potential key insights that can be drawn from the employee data of his business. The following are some of the areas in the business that he is interested in, and really hope you can help him learn more about the business:

1. What's the gender pay gap looks like in Company XYZ?

2. What are the key factors that could effect employee's happiness in Company XYZ?

3. What's the likelihood of the employees staying more than 2 years in Company XYZ?

4. Is there any other cool insights that you can show or share with Tony about Company XYZ?


> It is acceptable to make your own assumptions about the data and business context when required during the analysis. However, please clear document and communicate the assumptions in the assessment submission.


### Evaluation Criteria

Please note, there are **NO** predefined answers for the above questions. It is also **NOT** necessary to complete all of the questions listed above, the submission of the assessment will be evaluated based on:

1. Demonstration of the level of data science related experiences, knowledge and skills.

2. Ensure the findings or results in the submission can be effectively communicated and comprehended by the target audiences.

3. (Optional) Python and Jupyter notebook are the main tools used in the team currently. Submission with similar tooling would potential make the evaluation process more smooth. However, the key focus is still on providing meaningful analysis and insights to the provided dataset. Therefore, submission with any other tooling such as R, scalar, power BI, tableau are also acceptable as long as sufficient and clear instructions and documentation are provide in the submission.

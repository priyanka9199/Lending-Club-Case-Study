# Lending-Club-Case-Study
**Table of Contents**

***Introduction***

EDA Observations & recommendations

Technologies Used

Acknowledgements

Contact

**Introduction**

**Background:**

For a consumer finance company, two types of risks are associated with their decision to approve or reject any loan application. 

Those are Customer defaults: If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company .
Opportunity loss: If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company

**Business Problem:**

To reduce the risks associated with the approval process, we are to identify patterns to indicate if a person is likely to default, which may then be used for taking actions such as denying the loan, reducing the amount of loan, lending (to risky applicants) at a higher interest rate, etc.

**Dataset:**

We have about 40k loan records which contain loan attributes(rate, installment, interest rates etc) and customer financial information for all those loans. All loan applications also have loan status (target variable) which can be

Fully paid: Applicant has fully paid the loan (the principal and the interest rate)

Current: Applicant is in the process of paying the installments, i.e. the tenure of the loan is not yet completed. These candidates are not labeled as 'defaulted'.

Charged-off: Applicant has not paid the installments in due time for a long time, i.e. he/she has defaulted on the loan PS: The data related to rejected loan applications is not provided. Hence, the opportunity losses will be out of scope for this case study. Also, Current loan records will be ignored as we don't know if they will default or not. Hence can't be studied to find required trends.

****EDA Data observations & recommendations****

**Loan attributes:**

About 14.2 loans have defaulted over last 4 years
The total number of loans suggest that the business is consistently over the years
Most of the loans issued are in 5k to 10K range
More than 50% of loans are in grade A, B which have charge off rates of below 14.2
About 70% of loans are short duration (3 years).
The interest rates increase with duration of loans.Similarly,the interest rate increase as the loan grade lowers.This is to factor in riskiness of longer duration and low graded loans.

**Customer attributes**

Most of the customers have salary in 40 K to 80 K range.
More than 75% of customers have either rented homes or have mortgages
About 40% of customers come from California, New York and Florida.

**Recommendations:**

The loan applicants whose income has been verified are doing poorly than unverified loans. This is rather odd. There is a need to investigate further to see if it is a data issue or evaluation issue.
The grade C&D loans for customers having mortgaged or rented houses have relatively higher default rate. More investigation is needed.
I couldn’t see any direct relation to loan amount issued to customer income or DTI. Further investigation is needed to establish how customer’s ability to pay is factored in the loan approval process.

**Technologies Used**

seaborn 0.11.1

jupyter 1.0.0

numpy 1.20.1

anaconda 2021.05

python 3.8.8

matplotlib 3.3.4

Microsoft excel

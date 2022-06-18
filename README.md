# Prosper Loan Data Exploration
## by Arthur Ezenwanne


## Dataset
This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others taken from the [ProsperLoanData](https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv). A subset of features were selected and the data was also wrangled before being used for analysis and visualizations. Using the `Define - Code - Test` approach I cleaned and tidied the dataset by performing the following:
* Renaming feature names that are not uniformly named.
* Removing observations that contains null values.
* Merged the credit range lower and upper features into a single categorical feature.
* Updated the datatypes of some features as required.

## Summary of Findings
From the dataset we clearly observed that the data for `BorrowerRate` and `EstimatedReturn` is fairly uniformly distributed and correlated while economic indicators such as `EmploymentStatus`, `EmploymentStatusDuration`, `IsBorrowerHomeowner`, `IncomeRange`, etc shows that most loans were given to individuals that are on the high end of the economic indicators range with such applicants enjoying lower interest rates. Approved loan disbursements also showed that a larger percentage of the loans were given to applicants that are home owners with an `IncomeRange` above __*25,000 USD*__.

From the features, I observed that most loans was for debt consolidation, while all bad loans accounted for less than __*10%*__ of the total loans. It was also intriguing to see that in each financial year, more loans were disbursed in the __*4th*__ quarters than in preceeding quarters except for the Year __*2012*__. A large proportion of the loans have a duration of __*36*__ months and above while __*67%*__ of the loans are currently running. It is worthwhile to also note that loans with a shorter term of __*12*__ months have on average a lower loan interest rate than loans with a longer term.

From the multivariate plots of economic status, risk and rate we observed that borrower rates is inversely proportional to economic status and also inversely proportional to risk levels. Loan amounts above __*$15,000*__ were mostly approved for applicants that are homeowners, while most of the `Defaulted` and `Past Due` loans are loans where the applicants have lower `IncomeRange` values. We also observed a direct relationship between between the `EstimatedReturn` and `BorrowerRate`, irrespective of the `LoanOriginalAmount`.


## Key Insights for Presentation

# Udacity_Communicat-Data-Findings_Project-5_DAND

# Prosper - Loan Data

## Dataset

> [Data set](https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv&sa=D&source=editors&ust=1622283415087000&usg=AOvVaw0vpDb-LcekmeJjNUwDsRyP) has information on peer-to-peer loans facilitated by, a credit company, [Prosper](https://www.prosper.com/). The data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others. But some of the features I selected for alanysis are listed below with their descriptions taken from [here](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0).

- **Term**: The length of the loan expressed in months.
- **LoanStatus**: The current status of the loan: Cancelled,  Chargedoff, Completed, Current, Defaulted, FinalPaymentInProgress, PastDue. The PastDue status will be accompanied by a delinquency bucket.
- **BorrowerRate**: The Borrower's interest rate for this loan.
- **ProsperRatingAlpha**: The Prosper Rating assigned at the time the listing was created between AA - HR.  Applicable for loans originated after July 2009.
- **ListingCategoryNumeric**: The category of the listing that the borrower selected when posting their listing: 
    -  *0* - Not Available
    -  *1* - Debt Consolidation
    -  *2* - Home Improvement
    -  *3* - Business
    -  *4* - Personal Loan
    -  *5* - Student Use
    -  *6* - Auto
    -  *7* - Other
    -  *8* - Baby&Adoption
    -  *9* - Boat
    - *10* - Cosmetic Procedure
    - *11* - Engagement Ring
    - *12* - Green Loans
    - *13* - Household Expenses
    - *14* - Large Purchases
    - *15* - Medical/Dental
    - *16* - Motorcycle
    - *17* - RV
    - *18* - Taxes
    - *19* - Vacation
    - *20* - Wedding Loans
- **EmploymentStatus**: The employment status of the borrower at the time they posted the listing.
- **DelinquenciesLast7Years**: Number of delinquencies in the past 7 years at the time the credit profile was pulled.
- **StatedMonthlyIncome**: The monthly income the borrower stated at the time the listing was created.
- **TotalProsperLoans**: Number of Prosper loans the borrower at the time they created this listing. This value will be null if the borrower had no prior loans.
- **LoanOriginalAmount**: The origination amount of the loan.
- **LoanOriginationDate**: The date the loan was originated.
- **Recommendations**: Number of recommendations the borrower had at the time the listing was created.
- **Investors**: The number of investors that funded the loan.



## Summary of Findings

- The highest number of loan borrowers are **employed** with *600K+* in count.
- The people who belongs to **Full-time or Self-employed or Other** category are *few thousands* in count.
- The least number of people who borrow loans are **Not employed or Retired or Part-time** and they are just *few hundreds* in count. 
- With a boundary of mean and 2 times standard deviation, distribution of stated monthly income still has high right skewness.
- Any how, now one can infer that the mode of data is nearly to 5000.
- Second highest majority in Loan Status is of Completed ones in the data set.
- In the data set, Loan Status with Current are the highest ones. 
- Chargedoff loan also have substantial amount.
- Past due loans are categorized in several groups on the basis of length of payment delay.
- Rating 'D' is the most frequent one in both 'Completed' and 'Defaulted' statuses.
- Rating 'AA' is the least frequent one in both 'Completed' and 'Defaulted' statuses.
- Lower Ratings seem to have greater proportions of individuals with employment statuses 'Self-employed', 'Not employed', 'Retired' and 'Part-time'.
- Completed credits tend to be smaller incomparison to Defaulted credits ones.
- Loans of amount more than USD25000/- ones belong to Completed credits mostly. On the other hand, very few Defaulted credits are of amount more than USD25000/-.
- 'Debt Consolidation' is the most frequent category of all the time in Completed credits as well as Defaulted credits.
- Most of the defaulted credits comes from individuals with low Prosper rating.
- Defaulted credits tend to be larger than completed ones, except the lowest ratings.
- Debt Consolidation and Other category tend to have larger amount.



## Key Insights for Presentation

> I've chosen key plots with high data-to-ink ratio for the presentation. The plots I've chosen shows distribution of main variables, Loan status, monthly income, Prosper rating and I've tried to tell a story what are major predictors for loan status and Prosper rating variables.

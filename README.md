# (ProsperLoan Dataset)
## by (Abbey Christian Banafo)

## Preliminary Wrangling
> *We gather our dataset using data provided on the Udacity platform*.
> *We Assess for Quality and Tidyness Issues the data for any possible Issues but try to channel our focus more towards what we intend to achieve for our analysis.*
> *We clean the data using the Define, Code and Testing strategy*

The project is divided into two Phases;
> * *.***Phase 1***: *This Phase of the project mainly focuses on Exploring our dataset using Python datascience and analytics visualization tools. This includes pythons Pandas and Numpy Libraries, Seaborn and Matlplotlib. This phase further involved 3 main steps which was plotting univariate variables, bivarate and finally Multivariate variables. This, we refer to as the exploration phase of the project.*
> * *.***Phase 2***: *The second phase is the explanatory phase where we communicate our findings to the audience with the help specific grahs from the exploration phase. To this end, We will create a slide deck that leverages polished, explanatory visualizations to communicate your results.*


## Dataset

> * *This data is from [Prosper.com](https://www.prosper.com/), a money lendeng platform where people make money from those who borrow based on the interest rates.This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others. The null values of the Borrowers APR(Annual Percentage Rates) values were filled with the mean of the difference in availabe APR and interest rates.*
> * *The **ListingCategory (numeric)** column seemed to give a false impression of being an **ordinal** Categorical Variable but was not hence, assigned the actual names associated with the numeric variables and also renamed it as **ListingCategory** as well. The column as well appears to be of type **int** hence would need to be coverted in a categorical data type.*
> * *The listing categories, Occupations, prosperscore and prosperscore (alpha) were all converted to a categorical type data as well with the orders paramers of some set to true to represent an  ordinal type data.*
> * *More attention was not given to most columns that we thought may not have been relevant in our analysis*
> * *A large number of columns were also dropped to decrease code runtime.*

## Summary of Findings

> * *The aim for this exploration was to determine posible factors that could be responsible for lending out loan to members on the prosper platform as well as the APR(Anual Percentage Rate) that may be involved. Variables such as the loanAmounts, the StatedMontly Income, the Borrower APR and Interest Rates, Occupation, ListingCategories and many others including the ProsperScore which is a custom risk score built using historical Prosper data was explored for the analysis. The score ranges from **1-10, with 10 being the best**, or lowest risk score.*

> * *In finding out the factors that could affect the amount to be lent out to debtors, we looked at the distribution of members on how the loans were given out. We also looked at the distribution of the monthly income of these persons. A comparison between the distribution of the loan amount and the monthly income was generated. It was foundout borrowers with monthly incomes less than a region around **\$8k** were not given loans more than **\$25k**. Members with higher monthly income generally received higher loans. The occupations of these persons were hence compared to the monthly incomes to compare the distribution. The difference in monthly income did not vary that much with respect to the occupations of the borrowers. The borrowers generally received monthly income between a region slightly lower than **\$1k** to **\$10k** range. Since Occupation salaries did not vary that much it could only mean the amount loaned out to individuals were not so dependant on their occupations. Those who were doctors however seemed to have a wider range in terms of their salaries. The loan amounts was thus compared to the ListingCategories as well which in short terms was the reason for coming for the loan. It was found out borrowers usually came for loans as a result of dept, but the distribution of the loan amount was not so different for the dept categories as compared to the others. Hence could be concluded that one was more likely to receive a loan for reasons associated to dept in prosper. APR values also decreased with increase in prosperscores which was directly proportional to higher loan amounts as well*
> * ***In a nutshell***, *we can say having a higher monthly income as well as using it for reasons related to dept in addition to having a high properscore is more likely to earn one a loan on the prosper platform. One is also more likely to have a lower interest rate with these factors as well.*


## Key Insights for Presentation

> * *Most borrowers seem to have monthly incomes within the **\$10k** range*
> * *The amount of loan lent out to borrowers was highly dependant on the monthly income of a borrower.*
> * *Monthly Incomes less than a region around **\$8k** were not given loans more than **\$25k**.*
> * *BorrowerAPR values was dependant on borrowers monthly income and as well the amount of money lent out to these borrowers.*
> * *ProsperScore values of borrowers seemed to be lower for borrowers with higher APR values.* 
> * *Most borrowers had prosperscore between **4.0** and **8.0**.*

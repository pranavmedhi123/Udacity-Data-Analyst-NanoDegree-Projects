# Dataset Exploration of Prosper Loan Data
## by Pranav Medhi


## Prosper Loan Dataset

> Prosper Loan Data is a dataset that contains information about 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and various other variables, this is one of the most varied dataset I found which contains information on topics that are closely related as well as not so much, it can be used for studying tons of trends in the loan business, which is one of the reasons why I picked this dataset.


## Summary of Findings

1. We can see that Type C of the ProsperRating is the most common among the Applicants for loans while the AA Type having the least of the counts.
2.A huge majority of the Borrowers are in the Current Bracket for Loanstatus. Looks like Completed and Chargedoff are the next in line , while Nearly no borrowers in the Past Due(>120 days) bracket.
3.The Top 5 popular states we have borrowers from are CA, NY, TX, FL, IL. With CA being the at the top with almost double the counts of the borrowers in any of the follower states.
4.Most common occupations among the borrowers were Other, Professional, Executive, Computer Programmer, Teacher.
5.Overall majority of the population of the dataset are employed, and the retired , not employed, self employed, part-time type of employments section were negligible compared to it.
6.Most common income range was 50k-75k closely followed by 25k-50k range. It was rather amusing to look at the highest amount range which was 100k+ not adding to the lowest percentage of the borrowers, I think an income range of even higher paid individual would have made it such that it be the lowest percent of the population.
7.We can observe that the most popular listing category for which loan borrowers were present were categories 1, 7 and 2 which signify Debt Consolidation, Other and Home Improvement categories. 
8.Most of the borrowers have No Deinquencies in the past 7 years.
9.BorrowRate is pretty mixed, with maximum number of borrowers having the borrowerRate of 0.15 or 15 percent. Interesting , very low count of people have the maximum of 35% or minimum of 5% borrowerRate.  
10.We can observe that most of the employees have been in their status for a range of 0-100 months.
11.We can observe from the visuals that majority of the population has been the StatedMonthlyIncome in the range 2.5k-10k $. with the maximum being at 5k$.
12.We can observe that the visualisation is right skewed with multiple local maximas at 4000 USD, 10000 USD and 15000 USD.
13.We can observe that the PercentFunded variable is dominated by nearly all the population at 100% funded and a very tiny amount 70-73% funded loans. This was kind of a deadend variable as it didnt give much of the information that is required for my interest goal.
14.For Investors majority of the population lies withing the 0-100 mark, very low count of people get the mark above 100 Investors.
15.The Credit Score upper Range was a variable I expected to have some kind of impact on the loan approval chance, it looks like a lot of people have average upper range for their credit score, maybe most of the loan borrowers dont have much of a credit history.

16.We can observe that the LoanOriginalAmount and Monthly LoanPayment are highly correlated,borrowerrate and prosper score are highly correlated(negative correlation), borrowerrate and LoanOriginalAmount are (negative correlation).
17.Borrowers with low Prosper rating generally receive lower loan amount and higher Borrowrate(Interest on the loan). LoanAmounts borrowed for 'other' and 'auto' categories are generally lower than rest of the categories, the rate is somewhat similar for all the categories.
18.There is a gradual and steady increase in the Loan Amount allotted as the income range increases.From the violinplots we can observe that the for the lowest income range which 1-25k we have huge density of count of Borrowers for the same median Loan Amount while as we go further increasing the income range our data becomes more and more spread out and sparse around the median.
19.I have used the original dataset for this relation check , because originally we had Not Employed as a parameter in the Employment status , which I had to remove for getting a better and more sensible monthly income visualisation. So using the original dataset, keeps the contrast of the relation between having the Borrower as a home owner and LoanStatus (Major difference observed in the Defaulted section for both true and false of Homeowner status). We can observe that the majority of the population lies in the loan status of Current and Completed. 
20.Delinquencies in past 7 years have a direct relation with the clear visual that AA type Prosper Rating candidate having huge density around the median, where median is 0, as we go further with the types of Prosper Ratings we have minor spreading around the median signifying the increase in the Delinquency number. 
21.First Visualisation: Most of the population comes under the Employed and Fulltime sections with majority having the income between the ranges 25-50k or 50k to 75k with maximum being in the later.
Second Visualisation: The distribution was pretty evenly spread out , only for the Type C prosperRating being the maximum by some margin, with a most common incomerange of 50k-75k.
Third Visualisation: Majority of the population is employed and with the ProsperRating of Type C closely followed by Type B and Type A. The most common Type for Fulltime employee was Type A. 

22.We can take a lot of insights from this FacetGrid Scatter plots, such as: huge majority of the population falls under the Employed and FullTime Employed status, in that part majority have a loan amount between 1-20k, some even go as high as 25k. 
23.It can be observed that the AA Type ProperRating has the least BorrowerRate to pay for their loans, and the BorrowRate keep increasing as we go down the other types, we can also observe that generally the Homeowners have to lesser BorrowerRate as compared to the NonHomeowners
24.The Highest observed AverageMonthlyIncome was for EmployementStatus Employed, Type AA ProsperRating, while the lowest average income being for Self-Employeed EmployementStatus, Type AA ProsperRating which is 1500. 
25.It can be clearly observed that as the incomerange increases the Original Loan Amount Increases as well, with the least being for 1-25k income range and maximum at 100k+ incomerange, on an average its A, B, C type having the maximum for most of the IncomeRange. The most varying loanamount was for Type AA ProsperRating 1-25k Income range.
26.It can be observed that the Employed and FullTime employed members of the population has the highest and the most stable StatedMonthly Income Values, with AA Type ProsperRating having the highest and rest all going down as we move in order of types. The most volatile sector for StatedMonthlyIncome was SelfEmployed, they have the lowest StatedIncome of all the AA Type borrowers, where the values for the other types are varying a lot as well.





## Key Insights for Presentation


- Prosper Rating from AA to D have the higher loan amount allotted to them also that have more StatedMonthlyIncome as compared to the rest.
- Majority of the Borrowers are from the ProsperRating type B. Making it a point that there could be more chance of a loan being approved for type B ProsperRating Borrowers.
- NonHomeowner have to pay more Interest (BorrowerRate) as compared to the homeowners. We can conclude that Homeowners have a higher chance of loan approval. One other observation is that ProsperRating Type HR have to pay the highest interest rates irrespective of their Homeowning status.
- EmploymentStatus also plays a huge role in the decision of the Loan Amount, As it was observed that the maximum loan amount allotted was to the type B ProsperRating individuals that were Employed, and had StatedMonthlyIncome between 8000-10000.
- Delinquencies in past 7 years have a direct relation with the clear visual that AA type Prosper Rating candidate having huge density around the median, where median is 0, as we go further with the types of Prosper Ratings we have minor spreading around the median signifying the increase in the Delinquency number.
# RetirementSavingsSimulation

## Basic idea and assumptions

* A fixed percentage ($\alpha$) of net-of-tax income is saved each year for 30 years
* After year 30 the savings are spent at a rate of $(1-\alpha)$ times last income every year for 20 years
* There is some rate payed every year on savings (initially fixed afterwards random with uniform distribution)
* There is some rate of increase of income every year (initially fixed afterwards random with uniform distribution)

## Net-of-tax income every year

This is the income recieved before substracting the savings for retirement. Starts at a normalized $1$.

![income per year 30%, for rates between 1% and 6% of income growth](images/income_per_year_30%25.png)

As can be seen from the graph, income increments exponentially, and after retirement, maintains a constant rate. The step is because 
the graph is income *before savings*. As can be seen after retirement, no more income is saved, and the payouts are constant.

For this analysis the returns rate is used to represent a "return from general economic growth", and assumes that the efficiency of production
(of the salaried individual) increases inline with the general economy.

For other saving rates, the graph is similar. but larger and larger amounts are saved up:

![income per year 40%, for rates between 1% and 6% of income growth](images/income_per_year_40%25.png)
![income per year 50%, for rates between 1% and 6% of income growth](images/income_per_year_50%25.png)

## Savings for constant returns

![savings per year 30%, for rates between 1% and 6% of income growth and same rate of return on savings](images/savings_per_year_30%25.png)

We can see how for all rates of return, savings at 30 % decreases rapidly and only 5% and 6% make it over the 20 year line.

![savings per year 40%, for rates between 1% and 6% of income growth and same rate of return on savings](images/savings_per_year_40%25.png)

At 40% savings rate, all make it over the 20 year line, and at a rate of return of 6% there is the oportunity of an increase in retirement salary
without ever reducing the saved capital. All rates of return at or over 3% have substantial saved up income after 20 years of retirement.

![savings per year 50%, for rates between 1% and 6% of income growth and same rate of return on savings](images/savings_per_year_50%25.png)

When saving half of net-of-tax income, they all have substantial savings after 20 years.

## Savings for random returns

Now we asume that every year a 4 sided die is tossed, and economic growth for that year are determined by the result (-1% to 2% means that each year returns can be -1%, 0%, 1% or 2%).
This distribution is meant to assume that the return rates given before were "good" years. 

![savings per year 30%, for rates between -1% to 2% and 5% to %7 of income growth and same rate of return on savings](images/savings_per_year_30%25_random_returns.png)

Now returns are much worse. 

![savings per year 40%, for rates between -1% to 2% and 5% to %7 of income growth and same rate of return on savings](images/savings_per_year_40%25_random_returns.png)

5% to 7% barely keeps the savings constant up, and -1% to 2% barely reaches the 20th year of retirement at 40% savings. 

![savings per year 50%, for rates between -1% to 2% and 5% to %7 of income growth and same rate of return on savings](images/savings_per_year_50%25_random_returns.png)

For 50% savings all returns reach the 20 year retirement with spare.

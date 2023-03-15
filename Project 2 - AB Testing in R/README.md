## AB Testing in R 

## Behind - 
**We want to analyze a fictional dataset spanning seven months from July to January, where we conducted an A/B test in October.**

**The dataset is a fictional dataset which has been created in data_creation.ipynb**

### Task -1 
**Load the experiment_data.csv via read_csv and look at some random rows.**

`Month` shows the time dimension ranging from July 2022 to January 2023.

`Group` indicates whether a customer is in the treatment group or not

`Treated` is always 0 for the control (Existing) group as well as for the A group before October (prior to implementing the experiment).

`Dollars` are the $ spent by our customers

`id` is a personal identifier of the customers


### Task - 2
**Look at the customer_data to see the number of customers we observe per month in each group. How many individual customers are there? Look at the `Treated` column by `Month`**

### Task - 3

**Aggregate the whole dataset by `Month` and `Group` and look at the `Dollars` spent with a line plot.**

### Task 4

**Plot the `Dollars` spent by `Group` in the actual A/B time period.**


### Task - 5 
**Plot again the `Dollars` spent by `Group` in the actual A/B time period. This time, however, on a new dataset where we averaged the individual Dollars spent (by period) to avoid having multiple observations by the same customer during the same period.**

### Task - 6
**Now let's compare the `Dollars` spent between `New` vs. `Existing` `Group` in the actual A/B testing period.**

### Task - 7
**But we could also compare only `New` before and after implementing the A/B test. Let's do that!!**

### Task - 8
**Calculate the standard deviation of the `Dollars` spent in A/B period of the `New` group and use `power.t.test()` to calculate the necessary sample size to get statistical significant results on the `p = 0.05` signficiance level assuming `power = 0.8` (and equal variances).**

### Task - 9 
**Finally, let's run a linear regression approach where we regress `Treated`, `Group`, `as.factor(Month)` on `Dollars`.
Let's correct the standard error for the fact that we observe some clients multiple times.** 


About Dataset
This dataset is the most up-to-date kaggle dataset about daily sunspot counts with no missing values.

The source data originate from the World Data Center SILSO, Royal Observatory of Belgium, Brussels.

The Daily total sunspot number is derived by the formula: R = Ns + 10 * Ng, with Ns the number of spots and Ng the number of groups counted over the entire solar disk.
The original data contained some values between 1818 and 1850 but I removed those years because there was too much missing values.

Error values
Those values correspond to the standard deviation of raw numbers provided by all stations.

Before 1981, the errors are estimated with the help of an auto-regressive model based on the Poissonian distribution of actual Sunspot Numbers.
From 1981 onwards, the error value is the actual standard deviation of the sample of raw observations used to compute the daily value.
The standard error of the daily Sunspot Number can be computed by:
sigma/sqrt(N) where sigma is the listed standard deviation and N the number of observations for the day.
Before 1981, the number of observations is set to 1, as the Sunspot Number was then essentially the raw Wolf number from the Zürich Observatory.
Columns Description
Column 1-3: Gregorian calendar date
Year
Month
Day
Column 4: Date in fraction of year
Column 5: Daily total sunspot number. A value of -1 indicates that no number is available for that day (missing value): there should not be any missing values as I removed all years before 1850 where there was missing values.
Column 6: Daily standard deviation of the input sunspot numbers from individual stations.
Column 7: Number of observations used to compute the daily value.
Column 8: Definitive/provisional indicator. A blank (NaN) indicates that the value is definitive. A '*' symbol indicates that the value is still provisional and is subject to a possible revision (Usually the last 3 to 6 months)


source: https://www.kaggle.com/datasets/patrickfleith/daily-sunspots-dataset

# Diamonds Data Exploration

## Dataset

The data consists of information regarding 113,937 loans. The dataset has 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others. The dataset can be found for download in the kaggle website  [here](https://www.kaggle.com/datasets/yousuf28/prosper-loan) and,  [data dictionary](https://www.google.com/urlq=https://docs.google.com/spreadsheet/ccckey%3D0AllIqIyvWZdadDd5NTlqZ1pBMHlsUjdrOTZHaVBuSlE%26usp%3Dsharing&sa=D&source=editors&ust=1620931527882000&usg=AOvVaw3vbnU-g9ISX-OFBKzCIkqf) explains the variables in the data set.


## Summary of Findings

In the exploration, I found that there was a strong relationship between the
Borrower APR and Borrower rate. The strong relationship is illustrated by positive correlation coefficient very close to 1. This implied that an increase in one variable led to the increase of another variable and vice versa. The other variable of interest to our research questions, loan original amount showed a slightly moderate negative correlation with borrower APR and borrower rate. Out of all employment status categories, 'other' is the only one with minimum count of APR and rate greater than 0.2. Rest of the employment status categories have a 'cloud' of points below 0.2 for both APR and Rate. If borrower APR and rate are less than loan than 0.2, employment status is more likely to be anything except 'other'. I observed that 'employed' employment status received higher loan original amount compared to other employment status categories for the majority listing conditions except of the following 'student use', 'personal loans', 'taxes' and 'not available'. This also means that borrowers with a 'employed' employment status are likely to list any of the listing conditions except for the ones previously noted.

Outside of the main variables of interest, after taking the cubic root of DTI(debt to income ratio), we observe that 'defaulted' and 'cancelled' loan status have higher median scores of DTI than other loan status. This is likely because banks are reluctant to issues loan to borrowers with high DTI.


## Key Insights for Presentation

For the presentation, I focused on the features that were related to the research questions, features that showed unexpected association and leaving out other variable that seemed less likely to contributed to the questions. I started by introducing the distribution of borrower APR and rate using the histogram, followed by checking the strength of the numeric variables using the correlation heatmap. 

Afterwards, I introduced categorical variables like employment status and loan status. To start with,
I used the box plot to investigate the impact of employment status on borrower APR and rate. I further compared the impact of loan status on DTI and loan original amount after applying some transformation on these features.

Finally, the presentation was concluded by using a 2d histogram to facilitate multivariate analysis of borrower APR vs rate faceted by employment status, and employment status vs loan original amount faceted by listing conditions.
# KNN-Classification

## Classification - Personal Loan Dataset

This case is about a bank which has a growing customer base. Majority of these customers are liability customers (depositors) with varying size of deposits. The number of customers who are also borrowers (asset customers) is quite small, and the bank is interested in expanding this base rapidly to bring in more loan business and in the process, earn more through the interest on loans. 

In particular, the management wants to explore ways of converting its liability customers to personal loan customers (while retaining them as depositors). A campaign that the bank ran last year for liability customers showed a healthy conversion rate of over 9% success. This has encouraged the retail marketing department to devise campaigns to better target marketing to increase the success ratio with a minimal budget.

The department wants to build a model that will help them identify the potential customers who have a higher probability of purchasing the loan. This will increase the success ratio while at the same time reduce the cost of the campaign.

**Dataset Description**:

| Feature | Description |
| --- | --- |
| ID | Customer ID |
| Age | Customer's age in completed years |
| Experience | # years of professional experience |
| Income | Annual income of the customer (In 1,000 dollars) |
| ZIPcode | Home address ZIP code |
| Family | Family size of the customer |
| CCAvg | Average monthly spending on credit cards (In 1,000 dollars) |
| Education | Education level: 1: undergrad; 2: Graduate; 3: Advance/Professional |
| Mortgage | Mortgage Value of house mortgage if any. (In 1,000 dollars) |
| Securities Acct | Does the customer have a securities account with the bank? |
| CD Account | Does the customer have a certifcate of deposit (CD) account with the bank? |
| Online | Does the customer use internet bank facilities? |
| CreditCard | Does the customer use a credit card issued by the UniversalBank? |
| **Personal loan** | **Did this customer accept the personal loan offered in he last campaign? 1: yes; 0: no (target variable)** | 

**The classification goal is to predict if the client will subscribe (yes/no) a term loan (variable y).**
___

The dataset is available at the path `datasets` from the current directory.

## K nearest neighbors
		
K nearest neighbors is a simple algorithm that stores all available cases and classifies new cases based on a similarity measure (e.g., distance functions).

Algorithm: 
A case is classified by a majority vote of its neighbors, with the case being assigned to the class most common amongst its K nearest neighbors measured by a distance function.

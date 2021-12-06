# Bank-Marketing-Dataset
### Bank Customer Acquisition Analysis


## Introduction :
A Portuguese bank had conducted a telemarketing campaign for a term deposit product somewhere around late 2010. A term deposit is very similar to a fixed deposit, where we deposit money for a fixed period of time.

Through the campaign, the bank had collected data about the prospects' demographics, other financial products they have purchased in the past (loans, deposits, etc.), the number of times they were called, etc. They also recorded the response data, i.e., whether the person had subscribed to the term deposit product, which is the target variable.

The bank's marketing team wants to launch yet another telemarketing campaign for the same product. As an analyst at the bank, we want to answer the following questions using the past data:

   1. Which prospects are more likely to buy the product (i.e., to respond )?
   2. Which attributes determine the propensity to buy a term deposit?
   3. Once we predict the likelihood of response, how many prospects should we target for telemarketing?
   4. By how much can we reduce the marketing cost using the model, and how many prospects will we acquire?

## Term deposit :
## What is Term Deposit?
Term deposit is deposit account where money is locked up for some period of time, which ranges from few months to years. However, as a tradeoff to money being locked up, term deposit offers higher interest rate than traditional, liquid savings accounts. Early termination (withdrawl of money) is often associated with penalties.

It is also known as certificate of deposit in the United States.

You can read more about term deposit if you are interested:

  * Investopedia article: https://www.investopedia.com/terms/t/termdeposit.asp
  * Wikipedia article: https://en.wikipedia.org/wiki/Time_deposit#:~:text=A%20time%20deposit%20or%20term,to%20as%20its%20%E2%80%9Cterm%E2%80%9D.


## Assessing marketing campaigns :
### Conversion and Retention
Most widely used metrics to measure the success of a marketing campaigns are conversion rate and retention rate.

Conversion rate answers the question, "Are we good at making new customers (or subscribers in this case)?" by calculating the propportion of prospects (of a marketing campaign) that became a customer. Retention rate answers the question, "Are we good at keeping our current customers?", by calculating the proportion of existing customers (of a marketing campaign) that has stayed as customers after a given time.

For the context of analyzing this dataset, we will be observing the conversion rate across clients with differnt attributes, and retention rate is not relevant to the analysis. However, it is a good concept to be aware of.

### Segmentation
Segementation is a process of separating your audience into groups based on shared attribute(s), and marketing campaigns utilize them to make their messages resonate more with their target audience. Let's say you are running a marketing agency and that sent an email campaign for advertising life insurance policies. Would you expect the same or different levels of response from people in their 20s and 60s? Answer is most likely the latter.

Attributes used to segment audience or customers vary widely. They may include demographic information like age and gender and/or lifestyle traits and even past behaviors. For companies, segmentation also help companies to have deeper understanding of their audience or determine the most effective channel of communication.

This also means that effectiveness of any marketing campaigns should be evaluated separately on segment of audience/customer rather than calcaulting a single conversion rate or retention rate for the campaign.

I have listed additional articles below if you are interested this topic.

  * HubSpot Article: https://blog.hubspot.com/marketing/segmentation-targeting-positioning
  * Wikipedia: https://en.wikipedia.org/wiki/Market_segmentation

## Problem and Business Objective :
  * To reduce customer acquisition cost by targeting the ones who are likely to buy
  * To improve the response rate, i.e., the fraction of prospects who respond to the campaign

## Bank Marketing :
The data is related with direct marketing campaigns of a Portuguese banking institution. The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be (or not) subscribed.

The classification goal is to predict if the client will subscribe a term deposit (variable y).

## Description of Dataset :

  **Customer data:** Demographic data, data about other financial products like home loans, personal loans, etc.

  **Campaign data:** Data about previous campaigns (number of previous calls, number of days since the last call was made, etc.) Macroeconomic data

  **Target variable:** Response (Yes/No)

  **Input variables :**

  **Bank client data:**

   1. Age : (numeric)

   2. Job : type of job (categorical: “admin.”, “unknown”, “unemployed”, “management”, “housemaid”, “entrepreneur”, “student”, “blue-collar”, “self-employed”, “retired”, “technician”, “services”)

   3. Marital : marital status (categorical: “married”,“divorced”,“single”; note: “divorced” means divorced or widowed)

   4. Education : (categorical: “unknown”,“secondary”,“primary”,“tertiary”)

   5. Default : has credit in default? (binary: “yes”,“no”)

   6. Balance : average yearly balance, in euros (numeric)

   7. Housing : has housing loan? (binary: “yes”,“no”)

   8. Loan : has personal loan? (binary: “yes”,“no”)


**related with the last contact of the current campaign :**

   9. Contact : contact communication type (categorical: “unknown”,“telephone”,“cellular”)

   10. Day : last contact day of the month (numeric)

   11. Month : last contact month of year (categorical: “jan”, “feb”, “mar”, …, “nov”, “dec”)

   12. Duration : last contact duration, in seconds (numeric)

**other attributes :**

   13. Campaign : number of contacts performed during this campaign and for this client (numeric, includes last contact)

   14. Pdays : number of days that passed by after the client was last contacted from a previous campaign (numeric, -1 means client was not previously contacted)

   15. Previous : number of contacts performed before this campaign and for this client (numeric)

   16. Poutcome : outcome of the previous marketing campaign (categorical: “unknown”,“other”,“failure”,“success”)

**output variable (desired target) :**

   17. y : has the client subscribed a term deposit? (binary: “yes”,“no”)

## Dataset Source :
     https://www.kaggle.com/janiobachmann/bank-marketing-dataset

      https://archive.ics.uci.edu/ml/datasets/bank+marketing

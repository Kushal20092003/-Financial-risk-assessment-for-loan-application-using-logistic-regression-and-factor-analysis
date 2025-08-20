# -Financial-risk-assessment-for-loan-application-using-logistic-regression-and-factor-analysis

[Abstract](#abstract)

[Introduction](#introduction)

[Literature Review](#literature-review)

[Methodology](#methodology)

[Result](#result)

[Conclusion](#conclusion)

[Recommendation for future research](#recommendation-for-future-research)

## Abstract

Loan officer at any bank would be interested in detecting the factors which can identify people who are likely to default on loans, consequently good and bad credit risks. Moreover, he will also be interested in designing model which can predict chances of default with reasonable accuracy. A crucial step in the loan application process is financial risk assessment, which helps financial institutions minimize credit risk and allocate resources as efficiently as possible. This paper creates a predictive framework for estimating the probability of loan defaults by combining factor analysis and logistic regression. While Factor Analysis lowers dimensionality and finds latent characteristics influencing financial risk, like credit history and debt-to-income ratio. Logistic Regression is a strong classification technique is used to estimate default probabilities by balancing sensitivity and specificity, the suggested model showed excellent predictive accuracy. It offers a data-driven and interpretable way to expedite loan approval decisions, guaranteeing a more fair and effective procedure.

## Introduction

The overall purpose of this project is to analyse and build a model on loan application data that can be useful for decision-making purposes. Traditional methods rely on credit scoring models that consider a range of financial and demographic variables. However, these models often face challenges due to multicollinearity, high dimensionality, and the lack of interpretability of complex relationships among variables. To address these limitations, advanced techniques of multivariate analysis are applied here: Factor Analysis & Logistic regression. These will help identify patterns, relationships, and predict from the dataset, thus supporting managerial decision making in risk assessment and loan approval processes. This term paper simulates the real-world scenario wherein a financial institution aims to optimize its loan approval system. The analysis would identify the key factors that influence loan decisions, segment customers into meaningful groups, and build predictive models for loan approval within the restrictions of risk management standards.

### objective 

a) To identify the key underlying factors that influence loan approval decisions
based on borrowers' financial profiles, credit history, and demographic characteristics.

b) To predict loan approval likelihood based on financial and demographic
factors, identifying significant predictors such as credit score, debt-to-income ratio,
homeownership, and loan term to inform loan decision-making.

## Literature Review

Statistical and machine learning techniques for evaluating loans have been thoroughly examined in previous studies. Because of its ease of use and interpretability, logistic regression has been a mainstay. Conversely, factor analysis has been used in many fields to extract latent variables from correlated data. In order to improve performance, recent research emphasize the advantages of combining dimensionality reduction approaches with predictive models. By preprocessing loan data using factor analysis before utilizing logistic regression for prediction, this study expands on previous discoveries.

### Credit Assessment

The process of assessing a person's or an organization's creditworthiness in order to ascertain their capacity to repay debt is known as credit evaluation. To ascertain the degree of risk involved in making a loan to a borrower, it entails examining their income, assets, liabilities, and financial history because it enables them to reduce risk and make well-informed lending decisions, credit evaluation is essential for financial institutions. (Nsengiyera 2020) Financial firm risk losing money if they lend money to people or organizations that might not be able to repay the loan if their credit is not properly evaluated.

Credit Assessment Types —
There are several methods for evaluating credit, and each has pros and cons of its own. These are a few of the most prevalent kinds:

- Traditional Credit Assessment: This kind of evaluation is predicated on a borrower's financial records, payment history, and credit history. The evaluation entails examining the borrower's credit utilization ratio, existing debts, payment history, and credit score. Banks and other financial organizations frequently conduct traditional credit evaluations.

- Behavioural Credit Assessment: This method determines a borrower's creditworthiness by analysing information about their habits and behaviour. In order to learn more about the borrower's reliability and character, this method looks at non-financial data including social media activity and internet purchases.

- Alternative Credit Assessment: This method of determining a borrower's creditworthiness uses non-traditional data sources, like utility bills, rent payment history, and other information. This strategy is especially helpful for borrowers who do not have a lot of credit history or who have little access to conventional credit information.

### Logistic Regression

Credit risk Analysis can be carried out through numerous methods. The logistic regression and neural network models both are alike & worthy. Though the prior one is marginally better. Moreover, the genetic algorithm model is somewhat inferior but efficient. (Gouvea 2007). Logistic regression and multicriteria decision making have been combined to create a proficient strategy to achieve high performance. Logistics regression is used to find probability of default whereas multicriteria decision is used to classify firms for credit scoring based on predefined criteria. (Jerić 2009). Credit Risk Analysis is modelled using an artificial neural network. In commercial banks, logistic regression modelling is more effective than logistic regression modelling at identifying problematic clients. Higher credit risk results from higher interest rates and longer repayment terms. Customers in the industry sector are more affected. With a longer customer relationship history with the bank and a longer loan repayment period, it decreases. (Karimi 2014).

### Factor Analysis 

Factor analysis, which includes methods like principal component analysis and common factor analysis, is a statistical technique for identifying interrelations among a large number of variables. It explains these variables in terms of underlying dimensions or factors. The primary goal is to reduce a large dataset into fewer variables (factors) while retaining most of the original information. By providing a quantitative estimation of the variables' structure, factor analysis offers an objective method to create summarized scales. For instance, in a study of customer ratings for a fast-food restaurant, six variables—food taste, food temperature, freshness, waiting time, cleanliness, and employee friendliness—could be analysed.  (Joseph F. Hair 2019) The analysis might reveal that food taste, temperature, and freshness cluster into a single factor, termed "food quality." Similarly, waiting time, cleanliness, and employee friendliness might form another factor, referred to as "service quality." This approach helps researchers better understand the underlying relationships among variables.

## Methodology

- Dataset Definition and Source:

The dataset used for this analysis includes detailed information on loan applications from borrowers and various types of variables- financial and credit profile, demographic characteristics, and loan-specific details.

- Source: 

The dataset has been curated and shared for academic purposes to simulate loan approval data in a financial institution.

- Dataset Objective:

This dataset will be analysed to identify key factors influencing loan approval decisions,
predict loan outcomes, and segment borrowers into actionable groups based on financial and credit profiles.

- Dataset Description:

The dataset consists of 1,099 records, with the following key variables

<img width="451" height="481" alt="image" src="https://github.com/user-attachments/assets/2ae402d8-3a4f-4617-b7a4-8489a860d02e" />

### Factor Analysis :
Objective: To identify the key underlying factors that influence loan approval            decisions based on borrowers' financial profiles, credit history, and demographic characteristics.


- SPSS Output:
  
a)	KaiserMeyerOlkin (KMO) : Measures the sampling adequacy to ensure that the data is suitable for factor analysis. A value close to 1 indicates that factor analysis is appropriate.

• KMO Value: 0.553

• The KMO value above 0.5, indicates that the dataset is adequate for factor analysis.

b) Bartlett's Test of Sphericity :

  Tests the null hypothesis that the correlation matrix is an identity matrix (no correlation between variables). A significant result (p-value < 0.05) suggests that the data is suitable for factor analysis.

• Chi-square (Approx.): 4964.935

• Degrees of Freedom (df): 136

• Significance (Sig.): 0.000

The test is highly significant (p < 0.05), indicating that the correlation matrix is not an identity matrix. This means there are significant relationships among the variables, justifying the use of factor analysis.

<img width="342" height="136" alt="image" src="https://github.com/user-attachments/assets/4afc3f21-6a8c-4934-8bee-cf43b4884ae5" />

c) Principle Component Analysis:

• Eigenvalues and Factor Retention:

• Components with eigenvalues above 1 are typically considered significant and considered for further analysis in Factor Analysis. In this case, seven components have an eigenvalue above 1, so they were taken as the significant factors.

• This states, complexity in your dataset can be reduced to about seven core factors without information loss being too consequential

Scree Test: A visual inspection of the eigenvalues in a scree plot. The point where the curve flattens helps to determine the number of factors to retain.

Variance Explained by Each Factor:

• The initial eigenvalues column shows that the first component explains 16.507% of the
variance, while the cumulative variance explained by the seven factors is 64.764%. This
means that these seven components capture around 65% of the total variance in the dataset.


<img width="468" height="304" alt="image" src="https://github.com/user-attachments/assets/07936c46-f4cd-491b-866d-92e8e089b3ac" />

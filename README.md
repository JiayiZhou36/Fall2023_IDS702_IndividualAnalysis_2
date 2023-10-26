# Fall2023_IDS702_IndividualAnalysis_2
This is for statistics class individual analysis 2.

#### Research Question
How do race and gender influence job application callback rates?

#### Overview
[Resume dataset](https://www.openintro.org/data/index.php?data=resume) contains experimental data from a study aimed at understanding the factors that influence resume selection for a callback. The experimental data is derived from a study that sought to investigate the impact of race and gender on job application callback rates. The study monitored job postings in Boston and Chicago for several months during 2001 and 2002 and used this data to construct a set of test cases. The research question is: How do race and gender influence job application callback rates? This is an inference problem. The dataset comprises 4,870 observations and 30 variables, including gender, race, callback receipt, job type, and job industry.

#### Modeling Logistic Regression
Based on the question, the outcome variable is whether applicants receive a callback. Logistic regression is used because the outcome variable has two categories: receiving a callback (coded as 1) or not receiving a callback (coded as 0).

#### Result
In relation to the research question, our aim is to determine the influence of race and gender on job application callback rates. Based on the summary table presented earlier, with respect to gender, while controlling for all other variables, we have found that the odds of male candidates receiving callbacks are 0.97 times higher than those of female candidates. However, based on the p-value and the significance level (𝛼 = 0.05), we do not reach a conclusive relationship between gender and applicants’ callback reception. The confidence interval ranges from 0.71 to 1.32, indicating that we can be 95% confident that the odds of male candidates receiving callbacks are between 0.71 and 1.32 times higher than those of female candidates.
Regarding race, while controlling for other variables, we observed that the odds of white candidates receiving callbacks are 1.557 times higher than those of black candidates. This leads us to conclude that there is a significant linear relationship between race and callback reception in the population at the 𝛼 = 0.05 level. The confidence interval for this comparison falls within the range of 1.26 to 1.94, implying that we can be 95% confident that the odds of white candidates receiving callbacks are between 1.26 and 1.94 times higher than those of black candidates. Based on figure 2, we can also see that white candidates receive more callback compare to black candidates.
Additionally, other variables such as job location in Chicago, job type (e.g., manager or sales representative), the employer being an Equal Opportunity Employer, job-required education, computer skills, and organizational skills, applicants with a college degree, honors degree, computer skills, special skills, employment gaps, and years of experience also have an effect on job application callback rates based on p-values.

#### Future Work
The validity of this analysis depends on the accuracy of the assumptions made and the representativeness of the dataset. One of the strengths of this analysis is its inclusion of numerous confounding variables related to both race, gender, and whether applicants receive a callback. However, it also has several limitations.
Firstly, we are dealing with a highly imbalanced dataset where the number of observations not receiving callbacks significantly outweighs the number of observations receiving callbacks. In the future, it would be beneficial to use a more balanced dataset for analysis.
Secondly, race and gender are inferred based on first names, but the accuracy of this inference is uncertain as we lack verified data. This introduces potential biases into the analysis. Additionally, there are two variables with missing values: the indicator for whether the employer is a federal contractor and the type of company. If we can provide more detailed values for these variables and include them in the model, it might lead to improvements in the model’s performance.

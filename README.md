
---

# Talent Forecast & Retention Analysis Project

## Project Objective

The HR department at Salifort Motors wants to take some initiatives to improve employee satisfaction levels at the company. They collected data from employees, but now they don’t know what to do with it. They refer to you as a data analytics professional and ask you to provide data-driven suggestions based on your understanding of the data. They have the following question: what’s likely to make the employee leave the company?

The goals in this project are to analyze the data collected by the HR department and to build a model that predicts whether or not an employee will leave the company. 

If you can predict employees likely to quit, it might be possible to identify factors that contribute to their leaving. Because it is time-consuming and expensive to find, interview, and hire new employees, increasing employee retention will be beneficial to the company.
This project aims to deploy advanced data analytics and predictive modeling techniques to furnish the Human Resources (HR) department of a prominent consulting firm with actionable insights for workforce optimization.


## Methodology

The project will involve an in-depth analysis of the firm's HR data to construct a predictive model capable of identifying the likelihood of employee attrition. This model will serve as a decision-support tool for Salifort Motors, enabling proactive retention strategies and talent management.

## Installation Instructions

The project is executed using Python and requires the installation of the following packages :

- pandas
- numpy
- matplotlib
- seaborn
- sklearn
- xgboost

These packages can be installed using pip :

```
pip install pandas numpy matplotlib seaborn sklearn xgboost
```

## How to Use the Dataset

The dataset is a CSV file named 'HR_capstone_dataset.csv'. It can be loaded in Python using the pandas library :

```python
import pandas as pd

data = pd.read_csv('chemin_vers_le_fichier/HR_capstone_dataset.csv')
```

## Results and Conclusions

   - **Key Findings :**

- **What key insights emerged from your model(s)?**
  The key insights from the models include the identification of critical factors influencing employee turnover. The models have highlighted variables like `satisfaction_level`, `average_monthly_hours`, and a newly engineered feature `overworked` as significant predictors. There's also an awareness of potential data leakage, especially concerning the `satisfaction_level` and `average_monthly_hours` variables, which might not be reliable in real-world scenarios.

- **What business recommendations do you propose based on the models built?**
  The models suggest focusing on proactive retention strategies and talent management. They can be used as decision-support tools to predict employee attrition likelihood, enabling HR to intervene timely. Additionally, optimizing workforce management by addressing the identified key factors could lead to enhanced employee satisfaction and reduced turnover rates.

- **What potential recommendations would you make to your manager/company?**
  It's recommended to use the model outcomes to improve employee satisfaction levels and reduce turnover by addressing the identified factors. Moreover, ensuring transparent and non-discriminatory communication of these outcomes to employees is vital. This approach will foster a more engaged and stable workforce.

- **Do you think your model could be improved? Why or why not? How?**
  Yes, the model can be improved. The concern about high evaluation scores indicates possible data leakage, which can be mitigated by refining the feature selection and data used for training. Dropping `satisfaction_level` and re-evaluating `average_monthly_hours` as features, along with more robust feature engineering, could lead to a more accurate and realistic model.

- **Given what you know about the data and the models you were using, what other questions could you address for the team?**
  The analysis doesn't explicitly mention additional questions that could be addressed. However, given the nature of the data and models, questions related to workforce diversity, employee engagement levels, and the impact of specific HR policies on employee retention might be worth exploring.

- **Do you have any ethical considerations in this stage?**
  Ethical considerations include ensuring data privacy, avoiding model bias, and fairness in model application. It's crucial to handle employee data responsibly, ensuring that the predictive models do not lead to discriminatory practices. Additionally, being transparent about how the model influences HR decisions is important for maintaining trust and ethical standards.
   
   
   - **Recommandations** To retain employees, the following recommendations can be helpful :


* Cap the number of projects that employees can work on.
* Consider promoting employees who have been with the company for atleast four years, or conduct further investigation about why four-year tenured employees are so dissatisfied. 
* Either reward employees for working longer hours, or don't require them to do so. 
* If employees aren't familiar with the company's overtime pay policies, inform them about this. If the expectations around workload and time off aren't explicit, make them clear. 
* Hold company-wide and within-team discussions to understand and address the company work culture, across the board and in specific contexts. 
* High evaluation scores should not be reserved for employees who work 200+ hours per month. Consider a proportionate scale for rewarding employees who contribute more/put in more effort. 

**Conclusion**

It may be justified to still have some concern about data leakage. It could be prudent to consider how predictions change when `last_evaluation` is removed from the data. It's possible that evaluations aren't performed very frequently, in which case it would be useful to be able to predict employee retention without this feature. It's also possible that the evaluation score determines whether an employee leaves or stays, in which case it could be useful to pivot and try to predict performance score. The same could be said for satisfaction score. 

For another project, we could try building a K-means model on this data and analyzing the clusters. This may yield valuable insight.

## License and Citation

The HR Salifort Motors data was created for educational purposes.
The dataset is publicly available for use in research and education.
This dataset is freely accessible for non-commercial use on Kaggle.com.
The dataset can serve a myriad of purposes in the realms of social sciences, psychology, and machine learning. For instance, it can be employed to study factors influencing employees satisfaction and retention.

## Contributions

Contributions to this project are warmly welcomed. If you're keen on contributing, please initiate by opening an issue to discuss what you'd like to modify.

## Contact

Should you have any queries or feedback regarding this project, please reach out to me at :

*abajolah@gmail.com*

---

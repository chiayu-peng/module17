## Report Summary

### Business Objective

The business objective is to find a machine learning model which explains the factors contributing to a sucessful marketing campaign through calling potentional customers, so that business managers can allocate resources efficiently to target customrs who are most likely to subscribe to the bank product. 

### Findings

The best model is found by comparing different models with hyperparameter tuning, and the evaluation metrics is F1 score. F1 score is chosen as it represents a balance between accurancy score and recall score for as the evaluation metrics because the dataset is unbalanced with the subscription rate euqual to 11.3%, and the goal is not to miss any potential buyer, which is to minimuze the number of false negatives, while reducing marketing cost, which is to minimize false positives. 

The final selected SVM with tuned hyperparameters performs better than the default SVM (0.39 > 0.38) for the F1 score. 
The model shows that the top five most important features are:
- `emp.var.rate`	
- `cons.price.idx`	
- `cons.conf.idx`	
- `month`	
- `poutcome`

The best model is tuned SVM with F1 score of 0.39. The model shows that the most important factors attributing to a successful subscription are employment variation rate, consumer price index, consumer confidence index, month of contact, and outcome of previous campaign. This information shows that to improve the marketing campaign results, bank managers should pay close attention to the listsed economic markers, choose the months of highest subscription rate (March, September, October, and December) to launch the campaign, and focus on those who have been contacted before. 

### Next Steps and Recommendations

To improve the performance of the model, perhaps more features need to be included, for examples, duration of call and time of call.

Link to Jupyter Notebook: https://github.com/chiayu-peng/module17/blob/main/prompt_III.ipynb

# Decision Tree Pruning Analysis
This project implements a Decision Tree Classifier using scikit-learn with a focused analysis on model complexity control through pre-pruning and post-pruning techniques.The primary goal was to study how tree depth and pruning strategies impact overfitting and generalization performance.
 # Project Objectives
 
1.Implement a Decision Tree classifier using sklearn

2.Apply pre-pruning techniques to control early tree growth
3.Apply post-pruning (Cost Complexity Pruning) using ccp_alpha
4.Compare model performance before and after pruning
5.Analyze bias–variance tradeoff
 # Methodology
1️⃣ Baseline Model (No Pruning)
-Trained a fully grown Decision Tree
-Observed high training accuracy
-Detected overfitting via test performance gap
2️⃣ Pre-Pruning Techniques
Applied hyperparameter constraints to limit tree growth:
-max_depth
-min_samples_split
3️⃣ Post-Pruning (Cost Complexity Pruning)
-Used cost_complexity_pruning_path() to compute effective alphas
-Trained multiple trees with varying ccp_alpha values
-Evaluated training and validation accuracy across alphas
# Key Insights
-Deep trees tend to memorize training data.
-Pre-pruning prevents early over-complexity.
-Post-pruning systematically removes weak splits.
-Optimal alpha selection improves model robustness.
-Controlled complexity leads to better generalization.
# Tech Stack
-Python
-NumPy
-Pandas
-Matplotlib
-Scikit-learn
# Future Improvements
-Hyperparameter tuning with GridSearchCV
-K-Fold Cross Validation
-Feature importance visualization
-Comparison with Random Forest
-Performance benchmarking on larger datasets

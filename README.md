It's vital for credit card companies to detect fraudulent transactions to ensure customers are not billed for unauthorized purchases. This dataset, comprising transactions made by European cardholders in September 2013 over two days, includes 284,807 transactions, of which only 492 are fraudulent, representing a mere 0.172% of the total, indicating a significant class imbalance.

All input features are numerical and have been transformed using PCA, except for 'Time' and 'Amount'. The 'Time' feature records the seconds elapsed since the first transaction, and 'Amount' represents the transaction value, which can be useful for cost-sensitive learning. The target variable, 'Class,' indicates whether a transaction is fraudulent (1) or not (0).

Given the severe class imbalance, the Area Under the Precision-Recall Curve (AUPRC) is recommended as a more meaningful metric for model evaluation, as traditional accuracy metrics may not provide useful insights in this context.

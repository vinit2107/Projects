The dataset has been taken from Kaggle. The aim of the project is to correctly identify a fraud while a transaction is in place. The link to the dataset can be found [here](https://www.kaggle.com/c/ieee-fraud-detection/data).

There were two datasets, one for the transaction information and the other for identity, transaction details of the transaction like card details, card type, etc. 
The dimensions of the transaction dataset was 590540 x 394. Not all transactions had identity information.

The steps followed for completion of the project are as follows:

1. Loading the dataset.

2. Exploratory Analysis of the dataset. As the columns were not labeled to give off meaningful information, the analysis had to be thorough. Following were the findings of the exploratory analysis.
    1. TransactionDT columns showed that the transaction information in the training dataset was for over a year.
    2. Transactions had the least count on the fourth day of the week. 
    3. Fradulent transactions were not of a very big amount.
    4. Visa was the most common card network but discover had the most percentage of frauds.
    5. Debit card was the most common card type but credit card had more percentage of frauds.

3. Correaltion coefficient was calculated for a set of columns and the column with large coeffiencts were dropped from the dataset.

4. Aggressive filtering was applied to the devices to lower the number of categories in the categorical column.

5. Since the project was completed on the kernel, with limited amount of memory, memory reduction techniques were applied to degrade the datatypes of the columns.

6. RandomForestClassifier was fit to the training dataset to have the accuracy of 0.99 and evaluated against the test dataset to have a score of 0.904. 

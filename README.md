<img src="https://github.com/sinemypolat/hiring-ds/blob/master/Score%20UP.png">

**ScoreUp** is a simple scoring model where you may use to score customer 'health' based on their previous purchases. It takes a dataset file path as input and the dataset must include 3 arguments in order:

1. date_col: Name of the column for purchase dates in any format.
2. id_col: Name of the column for customer id.
3. price_col: Name of the column for the purchase amount.

ScoreUp prepare/preprocess dataset, splits it into training and test sets and then uses ordinary linear regression from scikit-learn library.

**Future Improvements:**

- More data can be provided in addition to purchase data and model can be improved in the light of the new data.

- Data processing functions are written based on 2 example input datasets. More general rules can be followed to provide the flexibility of working with any dataset.

- More independent modules can be added so that:
	- a model can be trained with a training set then downloaded to local disk
	- there would be ready-to-use models to make score predictions
	- a downloaded model can be read and used as a model to make score predictions

**How to Run:**

python get_scores.py -f <file_path> -d <date_col> -id <id_col> -p <price_col>



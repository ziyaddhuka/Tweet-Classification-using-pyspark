# Tweet-Classification-using-pyspark
Tweet Classification using pyspark pipelines


### Creating a pipeline with the following steps. 

Below are the steps of the project:
1. Loading: 
• First step is to load the text file from the path specified in argument 1
• After that, we need to remove rows where the text field is null.
2. Pre-Processing:
• Stop Word Remover: Remove stop-words from the text column
• Tokenizer: Transform the text column into words by breaking down the sentence into words.
• Term Hashing: Convert words to term-frequency vectors
• Label Conversion: The label is a string e.g. “Positive”, which we need to convert to numeric format
3. Model Creation - 
• Creating a logistic regression classification model using ParameterGridBuilder for parameter tuning and then use the CrossValidator object for finding the best model parameters.
4. Model Testing & Cross Validation: Next, you will need to train and test your model on
the given dataset and output classification evaluation metrics, such as accuracy, etc. You can see details of multi-class evaluation metrics at
5. Output: Writing the output the classification metrics to a file whose location is specified by the second argument.

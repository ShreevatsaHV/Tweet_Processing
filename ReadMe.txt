1. Loading: First step is to define an input argument that defines the path from which to load the dataset.
2. Pre-Processing: You will start by creating a pre-processing pipeline with the following stages:
 Tokenizer: Transform the text column by breaking down the sentence into words
 Stop Word Remover: Remove stop-words from the words column
 Term Hashing: Convert words to term-frequency vectors
 Label Conversion: The label is a string e.g. \Positive", which you need to convert to numeric format
3. Model Creation - You will need to create two classification models that you can select from the MLlib classification library. You will have to create a ParameterGridBuilder for parameter tuning and then use the CrossValidator object for finding the best model.
4. Model Testing & Evaluation: Next, you will create a random sample of the dataset and apply your model on it and output classification evaluation metrics, such as accuracy, etc.
5. Output: Finally, you have to write the output the classification metrics to a file whose location is specified by the second argument to the class.
# Neural_Network_Text_Filtering
The filter compares known text strings (keywords) with input text (e.g. ocr results) and only stores the input text in a database if the two strings are "similar enough" (how similar is determined by algorithm hyperparameters).

Five different datasets, defined below, were used to determine the input text to the filtering algorithm.
genAllMatch = Dataset1 => Exact matches (Strings are the same)
genSpellMatch = Dataset2 => Only one letter in the keyword string is changed
genNoMatch = Dataset => No matches (different strings)
noMatchShort = Dataset => No matches and short strings
realData = Dataset5 => Comparing actual screen capture ocr results with neural network keywords

The attached database contains the filtering results (execution time and accuracy-related results) of all 13 string comparison algorithms described in the paper entitled "Dropping irrelevant neural network classifier input: A fast method for comparing string lists". 
[LINK]

# Neural Network Text Filtering
This work represents a way to drastically accelerate neural network classifications by introducing a filter that receives input text (e.g. ocr) and compares it with up to 300 tokens (known text strings that the neural network is trained on). The filter will only let the input text pass if it successfully finds a keyword that is "similar enough" to it.

Five different datasets were generated as input text to the filter, and were tested in terms of accuracy and performance, as shown below:
1. genAllMatch = Dataset1 => The input text is the exact same as one of the neural network tokens. <br />
2. genSpellMatch = Dataset2 => Only one character in the neural network tokens were changed. <br />
3. genNoMatch = Dataset3 => The input text is completely different from the neural network tokens. <br />
4. noMatchShort = Dataset4 => The input text is both shorter and completely different from the neural network tokens. <br />
5. realData = Dataset5 => The input text represents actual screen capture ocr results extracted using tesseract-ocr. <br />

The attached database contains the filtering results (execution time and accuracy results) of 14 different string comparison algorithms described in the paper entitled "Filtering noisy text to accelerate classification". 
You can find this paper in this repository: Filtering_noisy_text_to_accelerate_classification.pdf

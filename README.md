# Neural_Network_Text_Filtering
The filter receives input text (e.g. ocr) and compares it with up to 300 keywords (known text strings). The filter will only let the input text pass if it successfully finds a keyword that is "similar enough" to it.

Five different datasets were used to determine the input text to the filter:
1. genAllMatch = Dataset1 => The input text is the exact same as one of the keywords. <br />
2. genSpellMatch = Dataset2 => Only one character in the keyword string is changed. <br />
3. genNoMatch = Dataset3 => The input text is completely different from the keywords. <br />
4. noMatchShort = Dataset4 => The input text is both shorter and completely different from the keywords. <br />
5. realData = Dataset5 => The input text represents actual screen capture ocr results. <br />

The attached database contains the filtering results (execution time and accuracy-related results) of 14 different string comparison algorithms described in the paper entitled "Filtering noisy text to accelerate classification". 
[LINK]

# Sarcasm-Detection

Data Used - https://github.com/rishabhmisra/News-Headlines-Dataset-For-Sarcasm-Detection

Label Distribution -- \
![alt text](https://github.com/tejulp/Sarcasm-Detection/blob/main/images/Label%20distribution.png) \
0: non-sarcastic headline \
1: sarcastic headline

Objective: Recognition of sarcasm in news headlines after training on labelled dataset using Supervised Learning Approach. BERT Algorithm fine-tuned for this purpose.

Approach:
1. Clean headlines by removing punctuation and numbers.
2. To understand data better, created a counter to count the occurence of each word.
3. Splitting the data into training, testing and validation sets.
4. Get length distribution of each headline in training set and cap at 95th percentile value (i.e maximum of 15 words from each headline will be considered).
5. Tokenize and encode sequences in train, test and validation set and create tensors for input and actual output (labels).
6. Defining BERT model architecture, optimization algorithm, and saving weights in a separate file that can be used as a checkpoint during testing phase.

Model Performance Evaluation on Test set -- \
![alt text](https://github.com/tejulp/Sarcasm-Detection/blob/main/images/accuracy%20table.png) \

Confusion Matrix -- \
![alt text](https://github.com/tejulp/Sarcasm-Detection/blob/main/images/confusion%20matrix.png) \

Tech-stack: NLTK, BERT-uncased base, PyTorch, Transformers

Code Reference - https://github.com/prateekjoshi565/Fine-Tuning-BERT

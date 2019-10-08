**About Problem Statement**:
 - Genre: NLP (Natural Language Processing)
 - Problem Type: Contextual Semantic Similarity, Auto generate Text-based answers

**Description**
 - Here, we are given a Train.csv file containing the correct answers and Distractors and a Test.csv file containing the test dataset which contains
   the test dataset.
 - The solution is to make the distractors for the given question, where we can make upto 3 distractors.
 - Have made use of Google Colab to speed up the process and avail the functioning of GPU.

**Idea**
 - I have made use of the concept of Recurrent Neural Netwroks and LSTM (Long Short Term Memory) Layers in Deep Learning Models. 
 - Here, I have first pre-processed the data given in Test and Train dataset alike.
 - The data pre-processing includes removal of lower frequency words which have not occured very frequently, removal of punctuations and words having sigle letters (I,a etc).
 - After the pre-processing part we have made the Vocabulary for our given model.
 - Have appended the terms 'StartSeq' and 'EndSeq' for recognizing the starting and ending of the sentences, since LSTM and RNN follows fixed length sentences.
 - After this step have appended, the 'zeros' into the sentence to make every sentence of same length.
 - Also, I have made use that combining of three LSTM Networks into one final networks, where one network has Question, one has correct answers and 
another has distractors, in which it will predict word by word until the word - 'EndSeq' is encountered.
 - After making the given architecture in Deep Neural Networks, we let the model to train for almost 3-4 hours.
 - Many instructions have been embedded in the code file itself.

**Results**
 - Distractors have been formed and upto 3 distractors have been formed.	

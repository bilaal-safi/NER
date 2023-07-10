
# NER Tagging using LSTM Model

This code implements a Named Entity Recognition (NER) system using an LSTM model. It reads a text file containing labeled sentences, preprocesses the data, and trains an LSTM model to predict the NER tags for new sentences.

# Pre-requisites
Make sure you have the following libraries installed:

- numpy
- pandas
- matplotlib
- tensorflow
- sklearn

# Usage
### 1. Prepare the Data:
- Modify the 'train_file' variable to specify the path to the training data file.
- Modify the 'val_file' variable to specify the path to the validation data file.
- Modify the 'test_file' variable to specify the path to the test data file.
- The data files should follow the CoNLL 2003 format
### 2. Run the Code:

- Run the code in a Python environment.
- The code will read and preprocess the data, train an LSTM model, and evaluate its performance on the test data.
- The results will be displayed, including accuracy, precision, and recall for each NER tag.
### 3. Test with Custom Sentences:

- After running the code, you can enter custom sentences to test the model's performance on new inputs.
- The model will predict the NER tags for the entered sentence.
# Additional Notes
- The code uses the TensorFlow library for building and training the LSTM model.
- The data is preprocessed and converted into numeric sequences using the TextVectorization layer from Keras.
- The LSTM model consists of an embedding layer, followed by a bidirectional LSTM layer and a dense output layer with softmax activation.
- The model is trained using the Adam optimizer and categorical cross-entropy loss.
- Training progress is plotted using matplotlib, showing accuracy and loss over epochs.

## References

 -  Daniel Jurafsky & James H. Martin. Speech and Language Processing. Chapter 8 and 9. Draft of January 7, 2023. https://web.stanford.edu/~jurafsky/slp3/8.pdf
 - Erik F. Tjong Kim Sang and Fien De Meulder. Introduction to the CoNLL-2003 Shared Task: Language-Independent Named Entity Recognition. https://aclanthology.org/W03-0419.pdf
 

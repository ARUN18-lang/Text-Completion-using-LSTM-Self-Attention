# Text Autocompletion with LSTM and Self-Attention

This project demonstrates a text autocompletion model using LSTM and self-attention mechanism. It's trained on the "Alice in Wonderland" text and can predict the next word given a sequence of previous words.

## How it Works

1. **Data Preparation:**
   - The "Alice in Wonderland" text is loaded and tokenized into individual words.
   - A vocabulary is created, mapping each unique word to an index.
   - The text is converted into input sequences of a fixed length (context length) and their corresponding target words.

2. **Model Architecture:**
   - An embedding layer converts words into vector representations.
   - An LSTM layer processes the input sequence, capturing sequential dependencies.
   - A self-attention mechanism allows the model to focus on important words within the sequence.
   - A fully connected layer maps the output to the vocabulary size, predicting the next word.

3. **Training:**
   - The model is trained using the Adam optimizer and cross-entropy loss.
   - It's trained for a specified number of epochs, minimizing the difference between predicted and actual words.

4. **Autocompletion:**
   - Given a starting text, the model predicts the next word based on the context.
   - The predicted word is added to the text, and the process is repeated to generate a sequence of words.

## Usage

1. **Install Dependencies:**
   bash pip install torch numpy sklearn

   2. **Run the Code:**
   - Load the code into Google Colab.
   - Execute the cells to train the model and test its autocompletion capabilities.

3. **Customize:**
   - You can modify the context length, embedding dimensions, hidden size, and training parameters for experimentation.
   - Try training on different datasets to personalize the autocompletion behavior.

## Note

- The model's performance depends on the dataset size and training parameters.
- You can further enhance the model by incorporating more advanced attention mechanisms or using pre-trained language models

  I have included sections on how the code works, usage instructions, an example, and a note. I hope this is helpful! Let me know if you have any other questions.

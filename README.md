# Character-Level Bigram Model

This project demonstrates building a simple character-level bigram model using PyTorch. The model learns the probability of the next character given the current character, based on a dataset of tags.

## Project Steps

1.  **Prepare Data Set**: Load the tags from a JSON file and create a list of all unique characters.
2.  **Prepare Vocab**: Create mappings from characters to indices (`stoi`) and indices to characters (`itos`).
3.  **Create Bigram Matrix**: Build a matrix where each entry `N[i, j]` represents the number of times character `j` follows character `i` in the dataset.
4.  **Plot Bigram Matrix**: Visualize the bigram matrix to understand the character transitions.
5.  **Normalize to Probability**: Convert the bigram counts into probabilities by normalizing the matrix.
6.  **Sample Probabilities**: Generate new sequences of characters based on the learned probabilities (using the traditional bigram model).
7.  **Neural Net Implementation**: Set up the data for a neural network approach to the bigram model.
8.  **Create Encoding for the Tensors**: Create one-hot encodings for the input characters.
9.  **Add Softmax**: Implement the softmax function to get probabilities from the neural network's output.
10. **Sample Probabilities (Neural Net)**: Generate new sequences of characters using the probabilities from the neural network.
11. **Loss Eval**: Evaluate the performance of the traditional bigram model using negative log-likelihood.
12. **Gradient Descent for Entire Data Set**: Train the neural network model using gradient descent to minimize the negative log-likelihood loss.

## Files

-   `tags.json`: The dataset containing the tags used to train the model.

## How to Run

1.  Upload the `tags.json` file to the Colab environment.
2.  Run the code cells sequentially in the notebook.

This project provides a basic introduction to building language models at the character level, comparing a traditional statistical approach with a simple neural network implementation.

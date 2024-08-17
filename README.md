# Machine-Translation-Using-Neural-Language-Model
Seq2Seq Translation Model: A bilingual English-French translation model using LSTM networks in TensorFlow/Keras. This project demonstrates data preprocessing, model training, and inference to translate English sentences into French.


## README

# Seq2Seq Translation Model

This project is a Seq2Seq (Sequence to Sequence) model designed to translate English sentences into French using LSTM (Long Short-Term Memory) networks. The model is trained on a subset of bilingual sentence pairs to understand and translate simple English sentences into French.

## Features

- **Data Preprocessing:** 
  - Text cleaning, tokenization, and vectorization.
  - Handling special tokens like `START_`, `_END`, and `PAD` for the model.

- **Model Architecture:**
  - A Seq2Seq model consisting of an encoder and a decoder built with LSTM layers.
  - Embedding layers to convert words into dense vectors.
  - The model is trained with teacher forcing to improve the translation quality.

- **Model Training:**
  - The model is trained on 10,000 sentence pairs.
  - It uses categorical cross-entropy loss and RMSprop optimizer.
  - Validation is performed using a validation split of 0.2.

- **Inference:**
  - The project includes an inference step to translate unseen English sentences into French using the trained model.

## Installation

1. Clone this repository.
    ```bash
    git clone https://github.com/yourusername/seq2seq-translation.git
    ```
2. Install the required dependencies.
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. **Prepare the Data:**
   - Place the bilingual text file (`fra.txt`) in the `./Data/` directory.


2. **Translate Sentences:**
   - Use the trained model to translate English sentences into French.
     ```bash
     python translate.py
     ```


## Results

After training, the model will be able to translate simple English sentences into French with a reasonable degree of accuracy. The results will be displayed in the console for a few example sentences.

## Future Work

- Improve the model by using more sophisticated architectures like Attention Mechanisms.
- Expand the dataset to include more complex sentences.
- Experiment with different hyperparameters and optimization techniques.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgements

- TensorFlow and Keras for providing easy-to-use machine learning libraries.
- The dataset used is a collection of bilingual sentence pairs from various sources.

---


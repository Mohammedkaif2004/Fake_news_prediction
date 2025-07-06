# Fake_news_prediction#
Thanks for clarifying! Here’s a **simpler README.md** more suited to a Kaggle-style project where you just share your `.ipynb` (Jupyter Notebook) and Keras model file—**no requirements.txt, just a notebook, and the model**. This version will match your style and workflow:

---

# Fake News Classification

This project is for classifying news articles as **Fake** or **Real** using deep learning techniques in Keras.

## Dataset

* The dataset used is from Kaggle:
  [Fake News Classification Dataset](https://www.kaggle.com/datasets/saurabhshahane/fake-news-classification)

## Approach

* **Text Preprocessing:**

  * Used NLTK stopwords to remove common words.
  * Removed irrelevant text.
  * Combined the `title` and `text` columns for each news article for better context.

* **Word Embedding:**

  * Used [GloVe 50d word embeddings](https://nlp.stanford.edu/data/glove.6B.zip) to convert words into vectors.

* **Model:**

  * Built an LSTM model using Keras.
  * Trained the model on the processed text data.

* **Result:**

  * Achieved **94% accuracy** on the test set.

## Files

* **`FakeNewsClassification.ipynb`** — Main Jupyter notebook containing all code for data loading, preprocessing, model training, and evaluation.
* **`model.h5`** — Trained Keras LSTM model saved in HDF5 format.

## How to Run

1. Download the [Kaggle dataset](https://www.kaggle.com/datasets/saurabhshahane/fake-news-classification).
2. Download the [GloVe 50d embeddings](https://nlp.stanford.edu/data/glove.6B.zip) and extract `glove.6B.50d.txt`.
3. Open `FakeNewsClassification.ipynb` in Jupyter Notebook.
4. Make sure the dataset and GloVe file are in your working directory.
5. Run the notebook to preprocess data, train the model, and evaluate accuracy.
6. You can also load the pre-trained model from `model.h5`.

## References

* [Kaggle: Fake News Classification Dataset](https://www.kaggle.com/datasets/saurabhshahane/fake-news-classification)
* [GloVe Embeddings](https://nlp.stanford.edu/projects/glove/)

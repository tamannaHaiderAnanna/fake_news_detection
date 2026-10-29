# Fake News Identification of Bangla Online News Portal Using Deep Learning Approaches

B.Sc. thesis, Department of Computer Science and Engineering, International Islamic University Chittagong (IIUC), June 2021.

**Authors:** Sadia Alam and Tamanna Haider · **Supervisor:** Dr. Engr. Abdul Kader Muhammad Masum

In 2020 very little fake-news research existed for Bangla. This thesis built its own Bangla news corpus by hand,
trained a Word2Vec model on it, and compared three deep learning classifiers for telling fake articles from real ones.

## Data

`Dataset/` holds 10,035 Bangla news articles. They were collected by hand from Bangla news portals and satire
sites, because many of those sites block scraping. Every file has the columns `domain`, `category`, `headline`,
`content` and `label` (0 = fake, 1 = real).

| File | Articles | Label |
|---|---|---|
| `Fake - Fake.csv` | 1,851 | 0 (fake) |
| `FirstFile.csv` | 6,511 | 1 (real) |
| `SecondFile.csv` | 1,673 | 1 (real) |

The articles belong to their publishers. They are shared here for research and teaching only.

## Method

1. **Pre-processing:** tokenization, then removal of punctuation, of 398 Bangla stop words (from stopwords-iso) and
   of web links, then stemming.
2. **Word embedding:** a Word2Vec model (gensim) trained on our own Bangla vocabulary of 134,113 words.
3. **Classifiers:** LSTM, CNN and a CNN-LSTM hybrid (Keras / TensorFlow), evaluated on an 80/20 split and with
   5-fold cross-validation.

## Results

From the thesis:

| Model | Accuracy, 80/20 split | Mean accuracy, 5-fold cross-validation |
|---|---|---|
| LSTM | 92% | 91.01% |
| CNN | 90% | 90.75% |
| CNN-LSTM | 92% | 90.22% |

82% of the articles are real, so accuracy alone says little about how many fake articles are caught. The thesis
names this imbalance as its main limitation; the notebook prints precision and recall for each class.

## Running the notebook

Open `Code/Fake_News_Detection_Using_Deep_Learning.ipynb` in Google Colab, put the three CSV files in Google Drive
under `MyDrive/Datasets/BanglaNews/MainData/`, and follow `README file for running the code.txt`, the cell-by-cell
steps written in 2021.

## History

The notebook, the dataset and the run instructions are the original June 2021 thesis files. This repository was
created in October 2026: the 2021 commits were rebuilt from the thesis archive and dated by the files' save times,
and this README was added then.

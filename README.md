# ML Practice Notebooks

Small, self-contained notebooks covering tabular classification, regression, and basic NLP preprocessing. Each notebook is independent and can be run on its own.

## Contents

1. **[`iris_flower_classification.ipynb`](./iris_flower_classification.ipynb)** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lance-bit/ml-practice-notebooks/blob/main/iris_flower_classification.ipynb) — Classifies the Iris dataset with SVM, AdaBoost, Random Forest, and a small Keras neural network, comparing accuracy and classification reports across all four.

2. **[`gold_price_prediction.ipynb`](./gold_price_prediction.ipynb)** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lance-bit/ml-practice-notebooks/blob/main/gold_price_prediction.ipynb) — Predicts gold prices with an SVR regression model, engineering lagged price features and using correlated commodities (oil, silver, platinum, the dollar index) as inputs. Reaches an R² of ~0.995 on the held-out test set.

3. **[`ad_click_prediction.ipynb`](./ad_click_prediction.ipynb)** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lance-bit/ml-practice-notebooks/blob/main/ad_click_prediction.ipynb) — Predicts whether a user clicks an ad: automated EDA with `ydata-profiling`, IQR-based outlier removal, cardinality checks on categorical columns, and a logistic regression pipeline evaluated with 5-fold cross-validation.

4. **[`arabic_tokenizer_inference.ipynb`](./arabic_tokenizer_inference.ipynb)** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lance-bit/ml-practice-notebooks/blob/main/arabic_tokenizer_inference.ipynb) — Loads an Arabic LLaMA-3 tokenizer and walks through tokenizing, encoding, and decoding Arabic text, including a look at the individual subword tokens produced.

5. **[`text_cleaning_pipeline.ipynb`](./text_cleaning_pipeline.ipynb)** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lance-bit/ml-practice-notebooks/blob/main/text_cleaning_pipeline.ipynb) — A small, reusable text-cleaning pipeline: strips HTML tags, lowercases text, removes emojis, strips URLs, and removes punctuation/symbols.

## Setup

```bash
git clone https://github.com/lance-bit/ml-practice-notebooks.git
cd ml-practice-notebooks
pip install -r requirements.txt
```

`gold_price_prediction.ipynb` pulls its dataset via `opendatasets` and will prompt for Kaggle credentials on first run — get yours from your Kaggle account settings.

## Status

These are practice and exploration notebooks, not production pipelines.

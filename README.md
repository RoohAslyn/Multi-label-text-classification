# Twitter Multi-Label Classification with Word2Vec, GloVe, and RandomForest

## Overview
This project demonstrates **multi-label text classification** on Twitter data using **Word2Vec** and **GloVe** embeddings. The embeddings are used to train a **RandomForest classifier** via `MultiOutputClassifier` to predict multiple labels per tweet.  

The workflow includes:  
- Data preprocessing & tokenization  
- Label binarization for multi-label classification  
- Generating Word2Vec and GloVe embeddings  
- Combining embeddings for better performance  
- Model training, evaluation, and visualization  

---

## Dataset
- The dataset used is a **Twitter Multi-Label Classification Dataset** (CSV format).  
- Columns:
  - `tweets` – The text of the tweet  
  - `labels` – Multi-label tags for the tweet (comma-separated, e.g., `hate,sarcasm`)  

**Example:**

| tweets                    | labels           |
|----------------------------|----------------|
| "I hate this product"      | hate           |
| "This is so funny lol"     | humor, sarcasm |

---

## Requirements
- Python 3.8+  
- Libraries:
```bash
pip install numpy pandas matplotlib scikit-learn gensim scikit-multilearn

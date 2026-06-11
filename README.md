# DataScience_MachineLearning----TextMining----NLP-Reviews_CaseStudy_Project
# Consumer Reviews Text Mining & Topic Modeling Pipeline (NLP)

This repository contains an end-to-end **Natural Language Processing (NLP)** and text mining case study conducted on unstructured consumer review data. By leveraging core computational linguistics frameworks, the pipeline processes raw customer feedback text to perform **Exploratory Text Mining**, **Feature Vectorization**, and unsupervised **Topic Modeling via Latent Dirichlet Allocation (LDA)** to extract distinct thematic feedback categories and underlying service insights.

---

## 📂 Dataset Repository & Architecture

The analytical pipeline processes an active marketplace review matrix composed of unstructured text strings linked to dimensional performance markers:

* **File Source:** `data.csv`
* **Key Attributes:**
  - `review_id`: Unique token identifier for each consumer text session.
  - `text`: Unstructured text paragraphs written by customers detailing their service/product experience.
  - `stars`: Ordinal rating score assigned by the reviewer (Scale: 1 to 5 stars).
  - `useful` / `funny` / `cool`: Engagement and community validation counters tracking review impact.

---

## 🛠️ Computational NLP Preprocessing Pipeline

Raw textual data requires deep mathematical normalization before it can be parsed by machine learning algorithms. The workspace inside `python.ipynb` executes a rigid preprocessing pipeline:

1. **Text Sanitization:** Standardizing all paragraphs to lowercase and applying Regular Expressions (`re`) to strip out punctuation arrays (`string.punctuation`), digits, and erratic line formatting.
2. **Tokenization & Stopword Elimination:** Segmenting blocks of strings into separate word tokens via `word_tokenize`. It then drops standard English stopwords (e.g., "the", "is", "at") using customized NLTK lists to retain pure, context-dense keywords.
3. **Morphological Standardization (Lemmatization):** Implementing `WordNetLemmatizer` paired with **POS (Part-of-Speech) Tagging** (`pos_tag`). This reduces inflected words down to their root dictionary form (e.g., "ordered", "ordering", and "orders" all successfully map back to the base lemma "order").

---

## 🔬 Advanced Feature Extraction & Modeling

Once the text matrix is normalized, it transitions from character strings into numerical space to fuel statistical classifiers:

### 1. Vectorization Layer
The pipeline evaluates and builds sparse mathematical representations using scikit-learn's extraction blocks:
* **`CountVectorizer`:** Builds a Term-Frequency matrix capturing exact raw token repetitions.
* **`TfidfVectorizer` / `TfidfTransformer`:** Evaluates Term Frequency-Inverse Document Frequency, scaling down common corpus-wide words while giving higher weight to distinct, contextually significant terms.

### 2. Latent Dirichlet Allocation (LDA) Topic Modeling
* Uses an unsupervised **LDA Model** to uncover latent structures within the text data, grouping reviews into **10 distinct semantic themes (Topics)**.
* Evaluates and lists the top 20 structural keywords per topic group to help analysts map clear operational domains (e.g., isolating specific clusters focusing on restaurant food/bars, booking locations, dental/fitness studios, or customer service wait times).

---

## 🚀 Local Deployment & Execution Guide

Follow these steps to deploy and run this text mining framework locally:

### 1. Clone the Repository Workspace
```bash
git clone [https://github.com/YOUR_USERNAME/CONSUMER_REVIEWS_NLP](https://github.com/YOUR_USERNAME/CONSUMER_REVIEWS_NLP).

# Topic Modeling and Clustering

This repository contains a Jupyter Notebook that demonstrates how to perform topic modeling on text data using BERTopic and cluster the resulting data using K-Means clustering. This approach is valuable for uncovering hidden topics within large corpora of text and organizing them into meaningful clusters.

## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Results](#results)

## Introduction

This notebook is designed to help you extract meaningful topics from a large set of textual data using BERTopic and then cluster the text data into groups based on these topics. The clustering step uses K-Means clustering to determine the optimal number of clusters, providing a clear structure to the text data.

## Features

- **Text Preprocessing:** Tokenization, lemmatization, and other text cleaning processes.
- **Topic Modeling:** Extraction of topics using the BERTopic library.
- **Clustering:** Grouping the text data into clusters using K-Means.
- **Visualization:** Elbow method plot for determining the optimal number of clusters.

## Installation

### Requirements

- Python 3.8 or higher
- Jupyter Notebook
- The following Python libraries:

```bash
pip install bertopic scikit-learn matplotlib pandas nltk
```

### Additional Dependencies

Ensure that the necessary NLTK data files are downloaded:

```python
import nltk
nltk.download('punkt')
nltk.download('wordnet')
```

## Usage

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/topic-modeling.git
   cd topic-modeling
   ```

2. **Run the Notebook:**

   Open the `Topic_Modeling_v1.ipynb` file in Jupyter Notebook or JupyterLab and run the cells to perform topic modeling and clustering on your dataset.

3. **Load Your Data:**

   Replace the placeholder data loading section with your text data in `df['processed_text']`.

4. **Adjust Parameters:**

   Adjust the parameters for BERTopic or K-Means if needed, such as the number of clusters or the preprocessing steps.

## Results

- **Optimal Number of Clusters:** The notebook determines the optimal number of clusters using the Elbow method and silhouette scores.
- **Cluster Labels:** Each piece of text is assigned a cluster label, which can be used for further analysis.

# Named Entity Recognition (NER) CRF Model

## Model Description

The NER CRF model in this directory is designed to recognize and classify named entities in text data. It utilizes the power of Conditional Random Fields, a sequence modeling technique, to consider the contextual dependencies between neighboring words when making predictions about entity labels. The model classifies 
words into the following tags:
- geo = Geographical Entity
- org = Organization
- per = Person
- gpe = Geopolitical Entity
- tim = Time indicator
- art = Artifact
- eve = Event
- nat = Natural Phenomenon
-o = other


## Usage

To use the NER CRF model, follow these steps:

1. Open the `ner_crf.ipynb` Jupyter Notebook using Jupyter Notebook or JupyterLab.
2. The notebook will guide you through the process of loading the necessary data, preparing it for training and testing, and training the CRF model.
3. You will learn how to use the trained model for predicting named entities in new text data.

## Dataset

The necessary dataset for this model is `ner_dataset.csv` found in this directory. This dataset includes labeled examples of text data where named entities are annotated with their corresponding labels.

## Requirements

To run the NER CRF model notebook, you'll need the following:

- Python
- Jupyter Notebook or JupyterLab (install using `pip install jupyter`)
- Required libraries:
    - `nltk`
    - `pandas`
    - `sklearn_crfsuite`
    - `sklearn`

## About Conditional Random Fields (CRF)

Conditional Random Fields are a type of probabilistic graphical model used for sequence labeling tasks like NER. They allow us to consider contextual information in sequences, making them particularly effective for tasks where neighboring elements heavily influence each other.
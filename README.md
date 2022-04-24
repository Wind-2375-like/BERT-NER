# Named Entity Recognition with BERT

A simple re-implementation of NER with BERT from [this video](https://www.youtube.com/watch?v=MqQ7rqRllIc&t=184s).

## Requirements

- torch
- transformers
- tqdm
- numpy
- sklearn

Run `pip install -r requirements.txt` to install the dependencies.

## Dataset

The training dataset is from the Kaggle competition [Annotated Corpus for Named Entity Recognition](https://www.kaggle.com/abhinavwalia95/entity-annotated-corpus?select=ner_dataset.csv), click on **Download(28MB)** and unzip the dataset to get two files `ner_dataset.csv` and `ner.csv`.

Then switch on the project root directory and `mkdir input`, and `mv *.csv input`.

## Base model

I choose to automatically download `bert-base-uncased` from the [Hugging Face](https://huggingface.co/bert-base-uncased) website.

## Run the model

To train and validate the model, just:

```shell
python src/train.py
```

To get predictions from the model, just:

```shell
python src/predict.py
```

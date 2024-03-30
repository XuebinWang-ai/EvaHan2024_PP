# EvaHan2024_PP
EvaHan2024 shared task: https://circse.github.io/LT4HALA/2024/EvaHan

Report title: A Simple Sequence Labeling Approach to Sentence Segmentation and Punctuation Prediction for Classic Chinese Texts

### Preparation
The json file `dataset/train.json` and `dataset/dev.json` is the data generated by the [**Xunzi-Qianwen-7B-CHAT**](https://github.com/Xunzi-LLM-of-Chinese-classics/XunziALLM).

Download the [**SikuRoBERTa**](https://github.com/hsc748NLP/SikuBERT-for-digital-humanities-and-classical-Chinese-information-processing) and place it in the `SIKU-BERT/`.

### Install dependencies
```shell
pip install -r requirements.txt
```

### Train

#### Train the Two-CRF sequence labeling model
```shell
sh train.sh
```

#### Train the single CRF sequence labeling model
```shell
sh train_single.sh
```

### Predict

#### Predict using the Two-CRF sequence labeling model
```shell
sh predict.sh
```

#### Predict using the single CRF sequence labeling model
```shell
sh predict_single.sh
```

# IMPZH-BERT
The project for GJS's NLP Coursework

This repository contains code, model, dataset for [IMPZH-BERT]
*Optimization based on ChineseBert code*(https://github.com/ShannonAI/ChineseBert)

**[ChineseBERT: Chinese Pretraining Enhanced by Glyph and Pinyin Information](https://arxiv.org/pdf/2106.16038.pdf)**  
*Zijun Sun, Xiaoya Li, Xiaofei Sun, Yuxian Meng, Xiang Ao, Qing He, Fei Wu and Jiwei Li*

## Introduction

The following image shows an overview architecture of IMPZH-BERT model.
 
![MODEL](https://github.com/K0kkk1E/IMPZH-BERT/tree/main/images/IMPZH-BERT.png)


## Download 
We use pre-trained ChineseBERT models in Pytorch version and followed huggingFace model format. (Provided by ChineseBert team)

* **`ChineseBERT-base`**：12-layer, 768-hidden, 12-heads, 147M parameters 
* **`ChineseBERT-large`**: 24-layer, 1024-hidden, 16-heads, 374M parameters   
  
Pre-trained ChineseBERT model can be downloaded here:

| Model | Model Hub | Google Drive |
| --- | --- | --- |
| **`ChineseBERT-base`**  | [564M](https://huggingface.co/ShannonAI/ChineseBERT-base) | [560M](https://drive.google.com/file/d/1CseJzc58W4s8U_eIuAnshHQmnmi7Sr5-/view?usp=sharing) |
| **`ChineseBERT-large`**   | [1.4G](https://huggingface.co/ShannonAI/ChineseBERT-large) | [1.4G](https://drive.google.com/file/d/1-glLDbmCrPgs_odjPvacaBniY0KnC8Z5/view?usp=sharing) |


*Note: The model hub contains model, fonts and pinyin config files.*

## Experiments

## ChnSetiCorp
ChnSetiCorp is a dataset for sentiment analysis.  
Evaluation Metrics: Accuracy


Training details and code can be find [HERE](tasks/ChnSetiCorp/README.md)


### THUCNews
THUCNews contains news in 10 categories.  
Evaluation Metrics: Accuracy

Training details and code can be find [HERE](tasks/THUCNew/README.md)

### TNEWS

TNEWS is a 15-class short news text classification dataset. <br>
Evaluation Metrics: Accuracy


Training details and code can be find [HERE](tasks/TNews/README.md)

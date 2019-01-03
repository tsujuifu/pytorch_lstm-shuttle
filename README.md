# [EMNLP'18 (long)] Speed Reading: Learning to Read ForBackward via Shuttle
A PyTorch implementation of LSTM-Shuttle

[Project](https://tsujuifu.github.io/projs/emnlp18_lstm-shuttle.html) | [Paper](https://tsujuifu.github.io/pubs/emnlp18_lstm-shuttle.pdf) | [Poster](https://raw.githubusercontent.com/tsujuifu/pytorch_lstm-shuttle/master/imgs/poster.jpg)

<img src='imgs/case.png' width='55%' />

## Overview
LSTM-Shuttle is an implementation of 
"Speed Reading: Learning to Read ForBackward via Shuttle" 
Tsu-Jui Fu and Wei-Yun Ma
in Conference on Empirical Methods in Natural Language Processing (EMNLP) 2018

<img src='imgs/overview.png' width='75%' />

LSTM-Shuttle not only reads shuttling forward but also goes back. Shuttling **forward enables high efficiency**, and going **backward gives the model a chance to recover lost information**, ensuring better prediction. It first reads a fixed number of words sequentially and outputs the hidden state. Then, based on the hidden state, LSTM-Shuttle **computes the shuttle softmax distribution over the forward or backward steps**.

## Requirements
This code is implemented under **Python3** and [PyTorch](https://pytorch.org).
Following libraries are also required:
+ [PyTorch](https://pytorch.org) >= 0.4

## Usage

## Resources
+ [IMDB Dataset](http://ai.stanford.edu/~amaas/data/sentiment/)
+ [AG Dataset](http://www.di.unipi.it/~gulli/AG_corpus_of_news_articles.html)
+ [FB-CBT Dataset](https://research.fb.com/downloads/babi/)

## Citation
```
@inproceedings{fu2018lstm-shuttle, 
  author = {Tsu-Jui Fu and Wei-Yun Ma}, 
  title = {Speed Reading: Learning to Read ForBackward via Shuttle}, 
  booktitle = {Conference on Empirical Methods in Natural Language Processing (EMNLP)}, 
  year = {2018} 
}
```

## Acknowledgement
+ [Learning to Skim Text](https://arxiv.org/pdf/1704.06877.pdf)

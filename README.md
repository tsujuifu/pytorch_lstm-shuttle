# [EMNLP'18 (long)] Speed Reading: Learning to Read ForBackward via Shuttle
A PyTorch implementation of LSTM-Shuttle

[Project](https://tsujuifu.github.io/projs/emnlp18_lstm-shuttle.html) | [Paper](https://tsujuifu.github.io/pubs/emnlp18_lstm-shuttle.pdf) | [Poster](https://raw.githubusercontent.com/tsujuifu/pytorch_lstm-shuttle/master/imgs/poster.jpg)

<img src='imgs/case.png' width='55%' />

## Overview
<img src='imgs/overview.png' width='75%' />

LSTM-Shuttle not only reads shuttling forward but also goes back. Shuttling **forward enables high efficiency**, and going **backward gives the model a chance to recover lost information**, ensuring better prediction. It first reads a fixed number of words sequentially and outputs the hidden state. Then, based on the hidden state, LSTM-Shuttle **computes the shuttle softmax distribution over the forward or backward steps**.

## This will be updated soon

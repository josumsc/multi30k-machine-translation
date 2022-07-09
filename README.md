# Machine Translation: From "Hello World" to "Hallo Welt" 🇬🇧🇩🇪

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/josumsc/multi30k-machine-translation/blob/master/src/multi30k-machine-translation.ipynb)

For this project we will be using PyTorch to train a machine translation model from English to German.
We will be using the [Multi30k dataset](https://github.com/multi30k/dataset/tree/master/data/task1/raw) to train our 
model and evaluate it later.

During this notebook we will show how to:
- Train a Seq2Seq model from scratch
- Apply attention to our model
- Load pretrained embedding weights
- Design a transformer model to better parallelize computations

## Installation of the environment

You can follow up this notebook in your machine by downloading Anaconda and then running the following command in the terminal:
```python
conda env create --file multi30k-machine-translation.yml
```
This should have you prepared to run jupyter notebook in the terminal and then running the mentioned code using that familiar interface.

Please note that I've used a M1 Mac, so the installation might suffer from some problems if you are using a different CPU architecture. In those cases do not hesitate to look up information on the official sources such as PyPi to solve your occasional errors during the installation.

## References
- [DeepLearning.ai Sequence Models](https://www.coursera.org/learn/nlp-sequence-models)
- [Deep Learning with PyTorch](https://learning.oreilly.com/library/view/deep-learning-with/9781617295263/)
- [Language Translation with TorchText](https://pytorch.org/tutorials/beginner/torchtext_translation_tutorial.html)
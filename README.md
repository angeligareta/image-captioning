<h1 align="center">Image Captioning</h1>
<h4 align="center">Second lab of the Scalable Machine Learning course of the EIT Digital data science master at <a href="https://www.kth.se/en">KTH</a></h4>

<p align="center">
  <img alt="KTH" src="https://img.shields.io/badge/EIT%20Digital-KTH-%231954a6?style=flat-square" />  
  <img alt="License" src="https://img.shields.io/github/license/angeligareta/image-captioning?style=flat-square" />
  <img alt="GitHub contributors" src="https://img.shields.io/github/contributors/angeligareta/image-captioning?style=flat-square" />
</p>

## Introduction
This assignment aims to describe the content of an image by using CNNs and RNNs to build an Image Caption Generator. The model would be based on the paper [[4]](https://arxiv.org/pdf/1411.4555.pdf) and it will be implemented using Tensorflow and Keras. The dataset used is [Flickr 8K](https://www.kaggle.com/adityajn105/flickr8k), consisting of 8,000 images each one paired with five different captions to provide clear descriptions. 
The implementation has been done using Python in a Jupyter notebook, where every step is carefully documented.

## Architecture
The model architecture consists of a CNN which extracts the features and encodes the input image and a Recurrent Neural Network (RNN) based on Long Short Term Memory (LSTM) layers. The most significant difference with other models is that the image embedding is provided as the first input to the RNN network and only once.
![Model architecture](docs/decoder.png)

## Results
The following picture presents an example of a generated caption by the implemented model:
![Results Image Captioning](docs/results-example.jpg)

## Further work
Despite the good results on the previous example, the Bilingual Evaluation Understudy (BLEU) Score for n-grams where n is greater than 2 is not very positive. As future work it would be interesting
to study changes in the architecture from where to input the picture.

## Authors
- Serghei Socolovschi [serghei@kth.se](mailto:serghei@kth.se)
- Angel Igareta [angel@igareta.com](mailto:angel@igareta.com)

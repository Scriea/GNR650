# GNR650

Welcome to the GitHub repository for the course GNR650 - Advanced Topics in Deep Learning for Image Analysis!. 
This is a collaborated repository between Ashutosh(200100037) and Utsav(200100054).
[**Link to Drive**](https://drive.google.com/drive/folders/1yl_HxtUj31QARmwFAvjTQfG-EfqfWZis?usp=sharing)


## [**Assignment 1**](./Task1/)

The primary objective of this task is to understand how a deep neural network behaves when trained with a limited amount of data, causing it to overfit the training set.
Subtasks involved:

  -  Train a ResNet18 on a small subset of the CIFAR-10 dataset (100 images per class) to intentionally induce overfitting
  -  Dive into the inner workings of the model by visualizing the learned convolutional kernels. By visualizing these kernels, you'll gain an understanding of the features the network learns to detect.
  -  Analyze the feature maps generated by intermediate layers of the network. This visualization will provide insights into the hierarchical representation of features throughout the network

### Misc.

  Tried to do the same for a bigger architecture - ResNet50.

### References
  - [**Keras**](https://keras.io/)
  - [**ResNet Paper**](https://arxiv.org/abs/1512.03385)

 ---

## [**Assignment 2**](./Task2/)

The task is to analyze the performance of Visual Transformer Models (ViT) like _B12_, on both fine-tuned, and base models. We use **EuroSAT dataset** for training.

Subtasks involved:

  - Fine-tune final layer; Fine-tune bottom layers; Full fine-tune; Inference from pre-trained model.
  - Visualize feature maps and compare
  
_Note: \
Due to lack of computation resources we weren't able to train for sufficient number of epochs. Its clearly visible from the train-validation loss curves that more iterations are needed for fine-tuning the model effectively._


### References
- [**Hugging Face**](https://huggingface.co/docs/transformers/main/model_doc/vit)
- [**Tensorflow Datasets - Eurosat**](https://www.tensorflow.org/datasets/catalog/eurosat)

---

## [**Paper Review - ViViT**](https://arxiv.org/abs/2103.1569))



The paper titled "ViViT: A Video Vision Transformer" by Anurag Arnab et al. from Google Research introduces a pure-transformer based model for video classification. Building on the success of transformer models in image classification, the paper proposes a model that extracts spatiotemporal tokens from input videos, which are then encoded using transformer layers. The paper addresses the challenges of handling long sequences of tokens in videos by proposing efficient model variants that factorize spatial and temporal dimensions. Despite the known limitations of transformer-based models requiring large datasets, the authors demonstrate how to effectively train on smaller datasets. They achieve state-of-the-art results on several video classification benchmarks, surpassing previous methods based on deep 3D convolutional networks.\
Please read the full review [here](./Paper_Review/ViViT_Review.pdf).

---

## [**Paper Review - Universal Domain Adaptation through Self-Supervision**](https://arxiv.org/abs/2002.07953)

The paper introduces a new general domain adaptation framework called Domain Adaptative Neighborhood Clustering via Entropy optimization (DANCE). DANCE addresses the challenges of universal domain adaptation by leveraging a novel neighborhood clustering technique. This self-supervised approach learns the structure of the target domain, while entropy-based feature alignment aligns or rejects target features based on their entropy. Experiments demonstrate DANCE's superiority over baselines in various domain adaptation settings. \
Please read the full review [here](./Paper_Review/Universal_Domain_Adaptation_through_Self_Supervision-Review.pdf).

---



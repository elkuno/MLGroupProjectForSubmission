# MLGroupProject
CS 4320 Machine Learning Group Project doing [Leaf Classification](#competition-link)

## Important Information

You need to start with [traditional_models.ipynb](traditional_models.ipynb) because it contains all of the preprocessing necessary for the [Deep Learning Models](#deep-learning-models---score) as well.

We have split the models up into two different sections. [Traditional Models](#traditional-models---score) are what you think of when you think of Machine Learning (Random Forests, Decision Trees, KNN, etc.). [Deep Learning Models](#deep-learning-models---score) are models that use the Neural Network framework with many layers (ConvNet, MultiLayer Perceptron, Multimodal NN, etc.). 

These are split into two different sets of files. [Traditional Models](#traditional-models---score) use [traditional_models.ipynb](traditional_models.ipynb), [requirements.txt](requirements.txt). [Deep Learning Models](#deep-learning-models---score) use other notebooks, and will be submitted alongside the Traditional Models files.

### Deep Learning Models
- ***ONLY*** runs/tested in Python **3.11.7**. We have not gotten it to work in ANY other version
- The process for running these is ***QUITE*** involved. Should you try, we cannot really offer too good a guide. Please reach out to us if you do not think this is satisfactory.

### Traditional Models
- Only tested in Python **3.11.1**

## Auxiliary Information
### Slides Link:
https://docs.google.com/presentation/d/1PyNAxJ4sV3KhFrbPslyIZK_7mOAGxj4W-yd-Du5H8bQ/edit?usp=sharing

### Competition Link:
https://www.kaggle.com/competitions/leaf-classification 

### Competition Description:
The objective of this playground competition is to use binary leaf images and extracted features, including shape, margin & texture, to accurately identify 99 species of plants. Leaves, due to their volume, prevalence, and unique characteristics, are an effective means of differentiating plant species. They also provide a fun introduction to applying techniques that involve image-based features.

### Traditional Models - Score:
##### Scored with Multi-class Log Loss
- DummyClassifier (sklearn) - 4.59511
- VotingClassifier (sklearn) - 1.01819
- RandomForest (sklearn) (Metadata Only) - 0.68058

### Deep Learning Models - Score:
- Multilayer Perceptron (pytorch) (Images Only) - 1.67975
- Convolutional Neural Network (pytorch) (Images Only) - 1.61097
- Multimodal Neural Network (pytorch) (Using Data Augmentation) - 0.23164
    - Uses a Convolutional Neural Network for the MetaData and ResNet 152 (transfer learning) for the images

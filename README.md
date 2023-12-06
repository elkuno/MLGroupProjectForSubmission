# MLGroupProject
CS 4320 Machine Learning Group Project doing [Leaf Classification](#competition-link)

## Quickstart

### 1. Set up a Virtual Environment
```sh
python -m venv mlenv2
```

### 2. Activate the Virtual Environment

- **Bash:**
```sh
. mlenv2/Scripts/activate
```

### 3. Install the Required Packages
```sh
pip install -r requirements.txt
```

## Deactivating the Virtual Environment
Once you're done, you can deactivate the virtual environment by simply running:
```sh
deactivate
```

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


# Learning Through Interaction: A Feedback-Driven Image Captioning System

## Overview

This project develops an advanced **image captioning system** that integrates **adaptive attention mechanisms** and a **user-feedback framework** to improve the accuracy and contextual relevance of image captions. 

Key features include:
- Adaptive Attention Mechanism: Combines **channel-wise**, **spatial-wise**, and **domain** attention units.
- User Feedback Integration: Enables iterative learning through reinforcement learning.
- Applications: Designed for content creation and improved accessibility and adaptability.



## Motivation

Traditional models often fail to address user-specific contexts or niche domains due to:
1. Lack of diverse annotated data.
2. Inability to refine predictions based on individual preferences.

### Why Adaptive Attention?
- Focuses dynamically on relevant features (global and local).
- Enhances contextual understanding of image scenes.

### Why User Feedback?
- Allows the system to iteratively improve through human interaction, aligning outputs with user expectations.



## Dataset

### Used COCO Dataset - https://www.kaggle.com/datasets/awsaf49/coco-2017-dataset

#### Preprocessing
1. Image resizing to 224x224 pixels.
2. Caption tokenization with special tokens (`<start>`, `<end>`, `<unk>`).
3. Vocabulary creation with a threshold to manage rare words.



## Model Architecture

### Encoder
- **CNN (ResNet-50)**: Extracts visual features.
- Outputs a tensor representing image content.

### Decoder
- **LSTM**: Generates captions word-by-word.
- Integrates adaptive attention mechanisms:
  - **Channel-wise Attention**: Emphasizes important feature channels.
  - **Spatial-wise Attention**: Focuses on specific image regions.
  - **Domain Attention**: Combines global and local features dynamically.



## User Feedback Framework

### Mechanism
1. Users provide feedback by correcting or rating captions.
2. Feedback is incorporated into the model through reinforcement learning, optimizing for metrics like BLEU and METEOR.



### Achievements
- Improved contextual understanding with adaptive attention.
- Demonstrated adaptability through user feedback.



## Challenges and Future Work

### Challenges
- Managing large datasets efficiently.
- Simulating real-world user feedback.

### Future Directions
- Extend to multilingual image captioning.
- Incorporate active learning to prioritize informative samples.



## Contributors
- **Rohitha Ravindra Myla**
- **Aishwarya**

# Disaster Tweet Classification Project 

---

## Project Overview

**Classifying Disaster-Related Tweets as Real or Fake**

This project demonstrates advanced deep learning and natural language processing (NLP) techniques to build a binary classification model that distinguishes between tweets about real disasters and false alarms. The model was developed for an analytical company interested in monitoring and analyzing emergency-related communications on social media platforms, specifically Twitter (X).

Social media has become a critical communication channel during emergencies and disasters. However, not all disaster-related tweets represent actual events—many are speculative, fictional, or misleading. This project addresses the challenge of automating the identification of genuine disaster tweets versus false positives, enabling organizations to:

- Quickly identify authentic emergency situations
- Reduce noise in real-time crisis monitoring systems
- Improve resource allocation during emergencies
- Enhance situational awareness for decision-makers

## Dataset and Exploration

The training dataset comprises **7,613 labeled tweets** with the following characteristics:

- **Features**: Tweet text, keywords, location, and user ID
- **Target Variable**: Binary classification (1 = Real disaster, 0 = Non-disaster)
- **Class Distribution**: Imbalanced dataset (57% non-disaster vs. 43% real disaster)
- **Data Quality**: Missing values in keyword (61) and location (2,533) columns; clean text feature

### Data Preprocessing Strategy

- **Feature Engineering**: Dropped ID, location, and keyword columns after determining their low predictive value
- **Text as Primary Signal**: Focused on tweet text as the primary feature, leveraging semantic and linguistic patterns
- **Class Imbalance**: Acknowledged and addressed through appropriate model selection and evaluation metrics

## Methodology

### Architecture & Technology Stack

**Deep Learning Framework**: TensorFlow/Keras

**Model Components**:
1. **Text Vectorization Layer**: Converts raw text into numerical sequences for neural network processing
2. **Embedding Layer**: Learns dense word representations capturing semantic relationships
3. **Bidirectional LSTM**: Captures context from both directions in text sequences, improving understanding of disaster-related language patterns
4. **Dropout Regularization**: Prevents overfitting on limited disaster-specific vocabulary
5. **Global Average Pooling**: Aggregates sequential information into fixed-size representations
6. **Dense Output Layer**: Binary classification with appropriate activation

### Advanced Techniques Employed

- **Regularization**: L1, L2, and L1L2 regularizers to prevent overfitting
- **Optimization**: Adam and RMSprop optimizers for adaptive learning rates
- **Sequential Architecture**: Built custom neural networks tailored for NLP tasks

## Key Skills Demonstrated

✓ **Data Analysis**: Pandas-based exploratory data analysis, missing value assessment, distribution analysis  
✓ **Deep Learning**: Custom neural network architecture design using TensorFlow/Keras  
✓ **NLP**: Text vectorization, embedding layers, sequence modeling with LSTMs  
✓ **Model Optimization**: Regularization techniques, optimizer selection, hyperparameter tuning  
✓ **Data Visualization**: matplotlib and seaborn for insights and pattern discovery  
✓ **Machine Learning Pipeline**: End-to-end workflow from raw data to production-ready model  
✓ **Problem Solving**: Addressed class imbalance and missing data strategically

## Expected Outcomes

This model enables:
- **Real-time classification** of incoming tweets during crises
- **Reduced false positives** in emergency alert systems
- **Scalable solution** for monitoring multiple disaster types
- **Foundation for deployment** in production crisis management systems

---


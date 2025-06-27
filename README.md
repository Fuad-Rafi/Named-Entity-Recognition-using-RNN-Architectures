# Named-Entity-Recognition-using-RNN-Architectures

This project focuses on implementing and comparing various Recurrent Neural Network (RNN) models for Named Entity Recognition (NER) using a custom annotated dataset.

## 📁 Dataset

The dataset used (`Dataset_A_Tag_test.csv`) contains 4796 labeled sentences with BIO-tagged named entities. Each sentence is associated with a list of tags representing entity types such as `B-per`, `B-geo`, `B-org`, etc.

### Columns:
- **Sentence #**: Numeric index of each sentence
- **Sentence**: Full sentence string
- **Tag**: List of BIO entity tags corresponding to each token in the sentence

## 🧠 Project Workflow

### 1. Data Preparation
- Tokenization of sentences
- Conversion of tags to numerical format
- Padding sequences to ensure uniform input size

### 2. Model Implementation
Implemented and compared the following deep learning models:
- Vanilla RNN
- LSTM
- GRU
- BiLSTM

### 3. Training & Evaluation
- Models trained for 10 epochs
- Tracked training/validation loss
- Evaluated using confusion matrices and accuracy plots

### 4. Hyperparameter Tuning
- Adjusted learning rate, batch size, and optimizer settings
- Visual comparison of model performance

## 📊 Evaluation Metrics

The following metrics were used to evaluate model performance:
- **Accuracy**
- **Precision, Recall, F1-score**
- **Confusion Matrix**
- **Loss Curves**

## 📦 Dependencies

Make sure to install the following Python libraries before running the notebook:

pip install numpy pandas matplotlib seaborn scikit-learn tensorflow keras

## 📝 Results
BiLSTM performed best overall in terms of F1-score and confusion matrix clarity.

GRU provided a good tradeoff between speed and performance.

Vanilla RNN struggled with longer dependencies.

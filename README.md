
# IMDb Sentiment Analysis with Hugging Face Transformers

This project demonstrates sentiment analysis on the IMDb dataset using Hugging Face's `transformers` library. The model is based on DistilBERT, a smaller, faster, and lighter version of BERT.

## Project Overview
The goal of this project is to classify IMDb movie reviews as either positive or negative using the DistilBERT model for binary classification.

### Key Features:
- **Data Loading:** IMDb dataset using Hugging Face Datasets library
- **Tokenization:** Using `AutoTokenizer` from Hugging Face
- **Model Training:** Fine-tuning DistilBERT for sequence classification
- **Evaluation:** Computing evaluation metrics after training

---

## Dataset
We used the IMDb movie reviews dataset from Hugging Face Datasets:
- **Training Data:** 1% of IMDb training data
- **Test Data:** 1% of IMDb test data

---

## Project Workflow

### 1. **Data Preparation**
- Load the IMDb dataset using Hugging Face's `load_dataset`.
- Tokenize the reviews using `AutoTokenizer` with padding and truncation enabled.

### 2. **Model Setup**
- Use `DistilBertForSequenceClassification` with two output labels (binary classification).

### 3. **Training Setup**
- Define training arguments using `TrainingArguments`.
- Train the model using Hugging Face's `Trainer` class.

### 4. **Model Evaluation**
- Evaluate the model's performance after training, reporting metrics such as loss, evaluation runtime, and samples processed per second.

---

## Results
After one training epoch, the model achieved:
- **Evaluation Loss:** 0.0031
- **Evaluation Runtime:** 216.81 seconds
- **Samples per Second:** 1.153
- **Steps per Second:** 0.148

---

## Prerequisites
- Python 3.8+
- Hugging Face Transformers
- Datasets library
- PyTorch or TensorFlow

### Installation
```
pip install transformers datasets torch
```

---

## How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/imdb-sentiment-analysis.git
   cd imdb-sentiment-analysis
   ```

2. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the training script:
   ```bash
   python train.py
   ```

4. View the evaluation results.

---

## Contributing
Contributions are welcome! Feel free to submit issues or pull requests.

---

## License
This project is licensed under the MIT License. See the LICENSE file for more information.

---

### Developed with ❤️ by Sinan Bandi



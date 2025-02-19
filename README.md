# 🛫 Airline Tweet Complaint Detector
**Identifying Non-Complaints in Airline Customer Feedback**

<div align="center">

![Python](https://img.shields.io/badge/Python-3.8%2B-3776AB?logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-FF6F00?logo=tensorflow&logoColor=white)
![NLP](https://img.shields.io/badge/BiLSTM-Deep_Learning-yellow)

</div>

Outcomes
<div align="center">

| 🎯 **Challenge** | 📊 **Approach** | 🚀 **Results** |
|------------------|-----------------|---------------|
| Distinguish complaint vs non-complaint tweets | BiLSTM with embedding layer | 84.1% test accuracy |
| Handle Twitter-specific text | Custom preprocessing pipeline | Improved model robustness |
| Rank non-complaints by confidence | Probability-based sorting | 99.7% confidence for top predictions |

</div>

## 📊 Methodology
<div align="center">
  
```mermaid
graph LR
A[Customer Tweets] --> B{Text Preprocessing}
B --> C[Tokenization & Embedding]
C --> D[Bidirectional LSTM]
D --> E[Model Training]
E --> F[Confidence Scoring]
F --> G[Ranked Predictions]
```
</div>

## 📈 Performance Metrics
<div align="center">

| Model Architecture | Accuracy | Epochs to Converge | GPU Training Time |
|--------|---------|---------|----------|
| Single LSTM | 79.3% | 8 | 5.4 min |
| BiLSTM (32 units) | 83.8% | 5 | 6.3 min |
| BiLSTM with Dropout | 84.1% | 5 | 6.8 min |
| Ensemble Model | 84.9% | 7 | 12.5 min |

</div>

## 💡 Key Features & Techniques

- **Advanced Text Preprocessing**:
  - Twitter handle (@mention) removal
  - URL and hashtag filtering
  - Whitespace normalization
  - Custom airline terminology handling

- **Deep Learning Architecture**:
  - 256-dimensional word embeddings
  - Bidirectional LSTM layers (32 + 16 units)
  - Dropout regularization (0.5)
  - Early stopping to prevent overfitting

- **Performance Optimization**:
  - GPU acceleration
  - TensorFlow data pipeline with prefetching
  - Batch processing for memory efficiency

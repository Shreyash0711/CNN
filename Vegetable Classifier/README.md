# 🥬 Vegetable Classification with Deep Learning

An AI model that identifies 15 different vegetables from photos with **92.7% accuracy** using deep learning.

## 🎯 What This Does

Upload a photo of a vegetable → Get instant classification with confidence score

**Supported Vegetables**: Bean, Bitter Gourd, Bottle Gourd, Brinjal, Broccoli, Cabbage, Capsicum, Carrot, Cauliflower, Cucumber, Papaya, Potato, Pumpkin, Radish, Tomato

## 🚀 Quick Start

```bash
# Install dependencies
pip install tensorflow numpy matplotlib

# Run the model
python classify_vegetable.py --image path/to/your/image.jpg
```

## 📊 Performance

| Metric | Score |
|--------|-------|
| **Overall Accuracy** | 92.7% |
| **Best Performers** | Carrot (99%), Potato (98%), Capsicum (97%) |
| **Dataset Size** | 3,000 images (200 per vegetable) |
| **Training Time** | ~20 epochs |

<details>
<summary>📈 Detailed Performance (Click to expand)</summary>

| Vegetable | Precision | Recall | F1-Score |
|-----------|-----------|--------|----------|
| Bean | 88.9% | 92.0% | 90.4% |
| Bitter_Gourd | 86.2% | 97.0% | 91.3% |
| Bottle_Gourd | 96.9% | 93.0% | 94.9% |
| Brinjal | 93.0% | 86.0% | 89.4% |
| Broccoli | 84.8% | 92.0% | 88.3% |
| Cabbage | 89.3% | 87.5% | 88.4% |
| Capsicum | 99.0% | 95.0% | 96.9% |
| Carrot | 98.0% | 100% | 99.0% |
| Cauliflower | 86.3% | 94.5% | 90.2% |
| Cucumber | 93.4% | 92.5% | 93.0% |
| Papaya | 95.8% | 91.5% | 93.6% |
| Potato | 97.5% | 98.5% | 98.0% |
| Pumpkin | 94.7% | 90.0% | 92.3% |
| Radish | 97.0% | 95.5% | 96.2% |
| Tomato | 92.4% | 85.5% | 88.8% |

</details>

## 🏗️ Technical Details

**Model Architecture**: Simple CNN optimized for vegetable classification
- Input: 128×128 RGB images
- Layers: 2 Conv2D + MaxPooling → Dense layers
- Parameters: 7.39M (28.21 MB)
- Framework: TensorFlow/Keras

**Dataset**: [Vegetable Image Dataset](https://www.kaggle.com/datasets/misrakahmed/vegetable-image-dataset) by misrakahmed


## 🎓 What I Learned

- CNNs excel at image classification with proper architecture
- Data quality matters more than model complexity
- Early stopping prevents overfitting (best performance at epoch 8)
- Balanced datasets lead to fair model performance

## 🚀 Future Improvements

- [ ] Add data augmentation for better generalization
- [ ] Implement transfer learning (ResNet, EfficientNet)
- [ ] Deploy as web app with Flask/FastAPI
- [ ] Add confidence scoring and uncertainty estimation

## 📝 License

MIT License - feel free to use and modify!

---

⭐ **Star this repo** if you found it helpful! Questions? Open an issue.

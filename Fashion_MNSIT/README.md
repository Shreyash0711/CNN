# 👕 Fashion MNIST CNN Classifier

This project demonstrates a simple yet effective Convolutional Neural Network (CNN) built using **TensorFlow/Keras** to classify images from the **Fashion MNIST** dataset — a collection of 70,000 grayscale images of 10 fashion categories.

---

## 📂 Dataset

- **Dataset**: [Fashion MNIST](https://github.com/zalandoresearch/fashion-mnist)
- **Classes**:
  1. T-shirt/top  
  2. Trouser  
  3. Pullover  
  4. Dress  
  5. Coat  
  6. Sandal  
  7. Shirt  
  8. Sneaker  
  9. Bag  
  10. Ankle boot

---

## 🧠 Model Architecture

```python
Input(shape=(28, 28, 1))
Conv2D(32, kernel_size=3, activation='relu')
MaxPooling2D(pool_size=2)
Conv2D(32, kernel_size=3, activation='relu')
MaxPooling2D(pool_size=2)
Flatten()
Dense(128, activation='relu')
Dense(64, activation='relu')
Dense(10, activation='softmax')
```

⚙️ Training Details
- Optimizer: Adam

- Loss: Categorical Crossentropy

- Batch Size: 64

- Epochs: 24

- Validation Split: 10% from test set

📈 Performance
- Test Accuracy: ~89.38%

- Macro F1-Score: ~0.89

🔍 Classification Report (Excerpt)
Class	Precision	Recall	F1-Score
Trouser	0.9928	0.9720	0.9823
Sandal	0.9848	0.9690	0.9768
Shirt	0.7441	0.6600	0.6995
Avg	0.8931	0.8938	0.8928

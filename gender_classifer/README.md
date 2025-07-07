# 👤 Gender Classification with UTKFace Dataset

This project builds a Convolutional Neural Network (CNN) model to classify the **gender** of a person based on facial images using the [UTKFace dataset](https://susanqq.github.io/UTKFace/).

---

## 📁 Dataset: UTKFace

- **Source:** [Official Site](https://susanqq.github.io/UTKFace/) or [Kaggle Mirror](https://www.kaggle.com/datasets/jangedoo/utkface-new)
- **Format:** JPEG images
- **Gender Label Encoding:**
- `0` = Male  
- `1` = Female

---

## 🧠 Model Architecture

A simple CNN model built using TensorFlow/Keras:

```python
model = tf.keras.Sequential([
  tf.keras.layers.Input(shape=(128, 128, 3)),
  tf.keras.layers.Conv2D(32, (3,3), activation='relu'),
  tf.keras.layers.MaxPooling2D(),
  tf.keras.layers.Conv2D(64, (3,3), activation='relu'),
  tf.keras.layers.MaxPooling2D(),
  tf.keras.layers.Conv2D(128, (3,3), activation='relu'),
  tf.keras.layers.MaxPooling2D(),
  tf.keras.layers.Flatten(),
  tf.keras.layers.Dense(128, activation='relu'),
  tf.keras.layers.Dropout(0.3),
  tf.keras.layers.Dense(1, activation='sigmoid')  # Gender output
])

model.compile(optimizer='adam', loss='binary_crossentropy', metrics=['accuracy'])
```

| Metric         | Value  |
| -------------- | ------ |
| Final Accuracy | 91.7%  |
| Final Loss     | 0.2227 |
| Model Format   | `.h5`  |

![download (2)](https://github.com/user-attachments/assets/566a09fd-7ead-451e-89ef-206e0b0600b2)


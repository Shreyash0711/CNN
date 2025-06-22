# Object Classifier 🧩

A simple CNN-based object classification project using TensorFlow and Keras.
* Class_names = ['Books', 'Bottle', 'Mug']
## Requirements
- Python 3.8+
- TensorFlow 2.x
- NumPy
- Matplotlib
- scikit-learn

```bash
pip install tensorflow numpy matplotlib scikit-learn
```
## Model Architecture
- Input: 224x224 RGB images

- Conv2D (32 filters) + MaxPooling2D

- Conv2D (64 filters) + MaxPooling2D

- Conv2D (128 filters) + MaxPooling2D

- Flatten

- Dense (128 neurons, ReLU)

- Output (Softmax, classes=3)

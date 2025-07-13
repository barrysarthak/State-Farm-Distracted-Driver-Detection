# 🚗 State Farm Distracted Driver Detection

A deep learning project to classify driver behaviors from dashboard images using CNNs, Data Augmentation, Transfer Learning, and Fine-Tuning. This solution is built on the **State Farm Distracted Driver Detection** dataset hosted on [Kaggle](https://www.kaggle.com/competitions/state-farm-distracted-driver-detection).

---

## 📂 Dataset

The dataset consists of labeled images of drivers exhibiting various behaviors such as:

- `c0`: Safe driving  
- `c1`: Texting - right  
- `c2`: Talking on the phone - right  
- `c3`: Texting - left  
- `c4`: Talking on the phone - left  
- `c5`: Operating the radio  
- `c6`: Drinking  
- `c7`: Reaching behind  
- `c8`: Hair and makeup  
- `c9`: Talking to passenger  

---

## 🧠 Models Implemented

| Model Type                   | Description                  | Augmentation | Fine-Tuned | Status     |
|------------------------------|------------------------------|--------------|------------|------------|
| Dense Neural Network         | Basic fully-connected model  | ❌           | ❌         | ✅         |
| CNN                          | Custom convolutional model   | ❌           | ❌         | ✅         |
| CNN + Data Augmentation      | CNN with augmentations       | ✅           | ❌         | ✅         |
| Transfer Learning - ConvNeXt | Pretrained ConvNeXtTiny      | ✅           | ❌         | ✅         |
| Transfer Learning - ResNet50 | Pretrained ResNet50          | ✅           | ❌         | ✅         |
| Fine-Tuned ConvNeXtTiny      | Fine-tuned for better results| ✅           | ✅         | ✅         |

---

## 📊 Evaluation Metrics

- Accuracy
- Loss
- Confusion Matrix
- Smoothed Training Curves

---

## 🧪 Testing

- Predictions on Kaggle's unlabeled test set
- Created formatted `sub256.csv` file for submission

---

## 🛠 Libraries Used

- `TensorFlow`, `Keras`
- `OpenCV`, `PIL`
- `Matplotlib`, `Seaborn`
- `NumPy`, `Pandas`, `scikit-learn`

---

## 🧰 How to Use

```bash
# Clone the repo
git clone https://github.com/barrysarthak/State-Farm-Distracted-Driver-Detection.git

# Install dependencies
pip install -r requirements.txt

# Run the Jupyter notebook or Python script
jupyter notebook driver_detection.ipynb

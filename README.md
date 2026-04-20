# ♻️ Recyclable or Not? - Waste Classification with Visual Explainability

Deep learning system that classifies waste as **Recyclable** or **Non-Recyclable** and shows **why** using Grad-CAM heatmaps.

## 🎯 What It Does

Takes an image of waste and tells you:
- ✅ **Recyclable** (plastic, glass, paper, metal)
- ❌ **Non-Recyclable** (organic, trash, contaminated waste)

Plus a heatmap showing exactly which part of the image the model focused on.

## 🔬 Key Feature - Explainability

Unlike standard classifiers that give a black-box prediction, this model uses **Grad-CAM** to generate a heatmap overlay. You can visually verify if the model is looking at the actual waste item or background noise.

## 🏗️ Tech Stack

- Python 3.8+
- PyTorch (ResNet-18 pretrained)
- Grad-CAM for visualization
- OpenCV, Matplotlib, Seaborn

## 📊 Dataset

- **Training:** Kaggle Waste Classification (~22,500 images)
- **Validation:** Real-world collected images (22 images)

## 🚀 How to Run

### 1. Clone the repository
```bash
git clone https://github.com/YOUR_USERNAME/waste-classification-resnet.git
cd waste-classification-resnet
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Run the notebook
```bash
jupyter notebook waste_classification.ipynb
```
*Or open in Google Colab and upload the notebook.*

### 4. Use your own image
Modify the last cell to test your own image:

```python
image_path = "your_image.jpg"
# Run prediction + Grad-CAM
```










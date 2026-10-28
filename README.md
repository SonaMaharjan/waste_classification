# Waste Classification with Deep Learning

A simple computer vision project to classify images of waste into 10 categories for recycling.

---

## About the Project

Sorting garbage by hand is slow and messy. In this project, a deep learning model is built to automatically recognize different types of waste from images.

The model classifies items into **10 categories**:

* **Battery**
* **Biological** (food scraps and organic waste)
* **Cardboard**
* **Clothes**
* **Glass**
* **Metal**
* **Paper**
* **Plastic**
* **Shoes**
* **Trash** (non-recyclable waste)

---

## How It Works

1. **Data Loading**: Images are loaded and resized to $224 \times 224$ pixels.
2. **Data Augmentation**: Small random flips and rotations are applied to help the model learn from different angles.
3. **Transfer Learning**: A popular pretrained model (**EfficientNetB0**) is used as the base feature extractor.
4. **Training**: A small classification layer is added on top to output predictions for the 10 categories.
5. **Evaluation**: The model is evaluated on images it has never seen before, and predictions are plotted visually.

---

## Dataset

* **Source**: [Garbage Classification v2](https://www.kaggle.com/datasets/sumn2u/garbage-classification-v2) on Kaggle
* **Images**: ~13,000 images
* **Classes**: 10
* **Split**: 80% for training, 20% for validation

---

## Built With

* **Python**
* **TensorFlow / Keras**
* **NumPy**
* **Matplotlib**

---

## How to Run

### 1. Clone this repository
```bash
git clone https://github.com/sonamaharjan/waste_classification.git
cd waste-classification
```

### 2. Install requirements
```bash
pip install -r requirements.txt
```

### 3. Open the notebook
Open and run `waste_segregation_deep_learning.ipynb` using Jupyter Notebook, Google Colab, or Kaggle.

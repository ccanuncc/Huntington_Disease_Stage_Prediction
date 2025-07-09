# Huntington Disease Stage Prediction

This project aims to predict the **stage of Huntington’s Disease** based on various clinical features using supervised machine learning techniques.

## 📂 Dataset

We used a publicly available dataset from Kaggle:
[Kaggle Dataset Link](https://www.kaggle.com/datasets/rajmohnani12/huntington-disease-dataset)

After initial preprocessing and feature selection, the dataset was standardized and class imbalance was addressed using SMOTE.

---

## 🧠 Model

We trained a **deep learning model** using Keras:

- 3 hidden layers: 128 → 64 → 32 (ReLU)
- Output layer: 4-class Softmax
- Loss function: Sparse Categorical Crossentropy
- Optimizer: Adam

The model achieved good performance on the test set and was saved as `.keras` along with the scaler.

---

## 🛠️ Features

- SMOTE for class balancing
- Scikit-learn + Keras + Tensorflow
- Independent scripts for preprocessing, training, and prediction
- Presentation-ready version included

---

## 🧪 Project Structure

```
huntington-disease-stage-prediction/
│
├── data/                # Raw and processed data
├── models/              # Saved model and scaler
├── presentation_ready/  # Folder used for final presentation
├── images/              # Visual results
├── notebooks/           # Optional Jupyter notebooks
├── scripts/             # Main scripts used in pipeline
├── docs/                # Presentation and additional documentation
└── README.md
```

---

## 🧑‍🤝‍🧑 Project Background

This was a **team-based university graduation project**. The group was split into two sub-teams:

- Our team focused on data-driven disease stage prediction using YOLO, SMOTE, and deep learning.
- The other team developed a **ROS + Gazebo simulation environment** to simulate a robot-assisted testing setup.

---

## 🔍 Sample Results

Sample classification results are included in the `images/` directory.

---

## 🔗 How to Run

```bash
python scripts/modelEgitimKayit.py
```

> Make sure to install dependencies listed in `requirements.txt` (not included here, feel free to add later).

---

## 📬 Contact

GitHub: [ccanuncc](https://github.com/ccanuncc)

---

**Note**: This version is a clean, modular version of our final project presentation. For academic publication, a refined version using a different dataset will be developed.
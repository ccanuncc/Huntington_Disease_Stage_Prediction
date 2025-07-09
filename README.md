
# 🧠 Huntington's Disease Stage Prediction

This project was developed as part of a university **Probability course assignment**, aiming to predict the stage of Huntington’s disease using real-world medical data and machine learning techniques.

The project demonstrates how to handle class imbalance, preprocess medical datasets, train classification models, and prepare predictions using neural networks.

---

## 📁 Project Structure

```
.
├── data/
│   ├── temizlenmis_veri_seti.csv              # Cleaned dataset
│   └── test_veri_seti2.csv                    # Final test data
│
├── models/
│   ├── hd_stage_model_smote.keras             # Trained neural network model
│   └── scaler_smote.save                      # Scaler used for normalization
│
├── scripts/
│   ├── verisetini_duzenleme.py                # Preprocessing steps
│   ├── smote.py                               # SMOTE oversampling
│   ├── modelEgitimKayit.py                    # Model training and saving
│   ├── categoricToFloat.py                    # Type conversion
│   └── inputTahmin.py                         # Input-based prediction
│
├── presentation_ready/
│   ├── sunum_kod1.py                          # Streamlined presentation code
│   └── sunum_kod2.py
│
└── README.md
```

---

## 📊 Dataset

We used the [Huntington Disease Dataset on Kaggle](https://www.kaggle.com/datasets/rajmohnani12/huntington-disease-dataset), which includes anonymized patient data and disease stage labels (0–3).

Due to severe class imbalance, **SMOTE (Synthetic Minority Over-sampling Technique)** was applied to the training data.

---

## 🧠 Model Details

- Neural Network (Keras - TensorFlow backend)
- 3 Hidden Layers: 128 → 64 → 32 units
- Activation Functions: ReLU + Softmax
- Loss Function: sparse_categorical_crossentropy
- Optimizer: Adam
- Trained for 30 epochs with batch size 32
- Final test accuracy: ~%75

---

## 🚀 Usage

1. Run `scripts/verisetini_duzenleme.py` to clean the dataset.
2. Apply oversampling via `scripts/smote.py`
3. Train and save model using `scripts/modelEgitimKayit.py`
4. Make predictions with `scripts/inputTahmin.py` using your own input.

---

## 👥 Team & Collaboration

This project was conducted by a **three-person team** as part of a course project. While this version is educational, a more advanced version is planned for academic publishing with a new dataset and enhanced methods.

---

## 📌 Notes

- This project is shared as **open source** for educational purposes.
- You are welcome to fork and build upon it for similar classification tasks.

---

## 📬 Contact

For questions or collaborations, feel free to reach out via GitHub or LinkedIn.

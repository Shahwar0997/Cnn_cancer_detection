# Histopathological Cancer Detection Using CNN
---

## Approach

- **Data Preprocessing**:
  - Balanced dataset through undersampling
  - Tissue area analysis using grayscale thresholding
  - RGB channel distribution comparison

- **Modeling**:
  - Basic CNN as baseline
  - VGG-style CNN for improved depth
  - Final model includes callbacks like EarlyStopping and ReduceLROnPlateau

- **Training**:
  - Used `ImageDataGenerator` for efficient loading and augmentation
  - Trained on Kaggle with small batch sizes due to memory constraints

---

## Results Summary

| Model                     | Val Accuracy | Val AUC  |
|--------------------------|--------------|----------|
| Baseline CNN             | ~75.1%       | 0.82     |
| VGG-style CNN            | ~80.5%       | 0.89     |
| VGG + Hyperparameter Tuning (Final)  | **84.35%**   | **0.91** |

---

## Dependencies

- Python 3.8+
- TensorFlow / Keras
- NumPy, Pandas, Matplotlib, Seaborn
- scikit-learn


---

## License

MIT License. See `LICENSE` for details.

---

## Acknowledgements

- [Kaggle: Histopathologic Cancer Detection](https://www.kaggle.com/c/histopathologic-cancer-detection)
- TensorFlow & Keras documentation

# Aegis Vision: Age Estimation with Deep Learning

**English** | [Versión en español](./README.md)
---

This project was developed as the final project for the **Samsung Innovation Campus**. It consists of an Artificial Intelligence model based on Convolutional Neural Networks (CNN) capable of predicting a person's age in years from a single photograph.

## 📌 Key Features

- **Age Prediction:** Estimates human age with a Mean Absolute Error (MAE) of ~6.65 years.
- **Robust Training:** Implementation of *Data Augmentation* and *DropOut* regularization.
- **Overfitting Prevention:** Integration of *Early Stopping* to automatically restore the best weights.
- **Analytical Visualization:** Learning curve graphs and real-time prediction visualization.

## 🛠️ Technologies and Applied Concepts

- **Deep Learning:** TensorFlow & Keras.
- **Data Science:** NumPy, Pandas, and Matplotlib.
- **Architecture:** Convolutional Neural Networks (CNN) for Regression.

## 📁 Repository Structure

```
├── Aegis_Vision.ipynb       # Main notebook with the code.
├── requirements.txt         # List of project dependencies.
├── models/
│   └── aegis_vision_final.h5 # Pre-trained model.
├── README.md                # Spanish documentation.
└── README.en.md             # English documentation (this file).
```

> Note: The [UTKFace](https://www.kaggle.com/datasets/roshan81/ageutk?resource=download) image dataset is not included due to file size restrictions, but it can be downloaded from Kaggle.

## ▶️ Usage Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/SARD82/Aegis_Vision
   cd Aegis_Vision
   ```

2. Install dependencies:

Use the requirements file to quickly set up your environment:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the project:

Open the Aegis_Vision.ipynb file in Google Colab or Jupyter Notebook to view the training process or make new predictions.

4. Use the pre-trained model:

You can load the AI's "brain" directly into your Python code without having to retrain it:
   ```Python
    from tensorflow.keras.models import load_model

    # Load the AI
    aegis_vision = load_model('models/aegis_vision_final.h5')

    # Ready to predict on new images!
    # prediction = aegis_vision.predict(new_image)
   ```

## 👥 Credits

Developed by **Santiago Durán Rendón**.

**Samsung Innovation Campus** – Artificial Intelligence Final Project.

## 📄 License

This project is distributed under the **MIT License**. You are free to use, modify, and distribute this software, even for commercial purposes, as long as the original copyright notice is included and credit is given to the developers.

For more details, please refer to the [LICENSE](./LICENSE) file attached to this repository.

---
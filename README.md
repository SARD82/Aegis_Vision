# Aegis Vision: Estimación de Edad con Deep Learning

[English version](./README.en.md) | **Español**
---

Este proyecto fue desarrollado como proyecto final para el **Samsung Innovation Campus**. Consiste en un modelo de Inteligencia Artificial basado en Redes Neuronales Convolucionales (CNN) capaz de predecir la edad de una persona en años a partir de una sola fotografía.

## 📌 Funcionalidades principales

- **Predicción de edad:** Estima la edad humana con un Error Absoluto Medio (MAE) de ~6.65 años.
- **Entrenamiento robusto:** Implementación de *Data Augmentation* y regularización por *DropOut*.
- **Prevención de Overfitting:** Integración de *Early Stopping* para restaurar los mejores pesos automáticos.
- **Visualización analítica:** Gráficas de curvas de aprendizaje y visualización de predicciones en tiempo real.

## 🛠️ Tecnologías y conceptos aplicados

- **Deep Learning:** TensorFlow & Keras.
- **Data Science:** NumPy, Pandas y Matplotlib.
- **Arquitectura:** Redes Neuronales Convolucionales (CNN) para Regresión.

## 📁 Estructura del repositorio

```
├── Aegis_Vision.ipynb       # Cuaderno principal con el código.
├── requirements.txt         # Lista de dependencias del proyecto.
├── models/
│   └── aegis_vision_final.h5 # Modelo pre-entrenado.
├── README.md                # Documentación en español (este archivo).
└── README.en.md             # Documentación en inglés.
```

> Nota El dataset de imágenes [UTKFace](https://www.kaggle.com/datasets/abhikjha/utk-face-cropped) no se incluye por restricciones de peso, pero se puede descargar desde Kaggle

## ▶️ Instrucciones de uso

1. Clonar el repositorio:
   ```bash
   git clone https://github.com/SARD82/Aegis_Vision
   cd Aegis_Vision
   ```

2. Instalar dependencias:

Utiliza el archivo de requerimientos para configurar tu entorno rápidamente:
   ```bash
   pip install -r requirements.txt
   ```

3. Ejecutar el proyecto:

Abre el archivo Aegis_Vision.ipynb en Google Colab o Jupyter Notebook para ver el entrenamiento o realizar nuevas predicciones.

4. Uso del modelo pre-entrenado:

Puedes cargar el cerebro de la IA directamente en tu código de Python sin tener que volver a entrenarlo:
   ```Python
   from tensorflow.keras.models import load_model

    # Cargar la IA
    aegis_vision = load_model('models/aegis_vision_final.h5')

    # ¡Lista para predecir sobre nuevas imágenes!
    # prediccion = aegis_vision.predict(nueva_imagen)
   ```

## 👥 Créditos

Desarrollado por **Santiago Durán Rendón**.

**Samsung Innovation Campus** – Proyecto Final de Inteligencia Artificial.

## 📄 Licencia

Este proyecto se distribuye bajo la **Licencia MIT**. Eres libre de utilizar, modificar y distribuir este software, incluso con fines comerciales, siempre y cuando se incluya la nota de copyright original y se dé crédito a los desarrolladores.

Para más detalles, consulta el archivo [LICENSE](./LICENSE) adjunto en este repositorio.

---
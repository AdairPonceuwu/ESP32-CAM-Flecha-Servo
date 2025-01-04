# ESP32-CAM-Flecha-Servo

Este proyecto utiliza una ESP32-CAM para capturar imágenes en tiempo real, detectar flechas con un modelo de detección de objetos preentrenado (SSD MobileNet v3), y controlar un servomotor basado en la dirección detectada.

## Características

- **Detección de objetos:** Implementación de detección de flechas usando OpenCV y un modelo preentrenado.
- **Control del servomotor:** Movimiento del servomotor según la flecha detectada (izquierda, derecha, arriba).
- **Integración con ESP32-CAM:** Captura de imágenes a través de una cámara IP.
- **Modelo preentrenado:** Uso de SSD MobileNet v3 con configuración optimizada para detección de flechas.

## Archivos Principales

- `IPaddressClassification.py`: Script principal que realiza la detección y controla el servomotor.
- `frozen_inference_graph.pb`: Modelo preentrenado en formato TensorFlow.
- `ssd_mobilenet_v3_large_coco_2020_01_14.pbtxt`: Configuración del modelo.
- `coco.names`: Lista de nombres de clases para el modelo.

## Requisitos

- **Hardware:**
  - ESP32-CAM configurada como cámara IP.
  - Servomotor conectado a un microcontrolador o directamente a la computadora.
  - Microcontrolador compatible con comunicación serial (como Arduino).

- **Software:**
  - Python 3.7+
  - Bibliotecas de Python:
    - OpenCV
    - NumPy
    - PySerial


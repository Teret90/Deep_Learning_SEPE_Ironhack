# Proyecto: Detección de Plagas Agrícolas en Cultivos de Hortalizas Usando Deep Learning

## 1. Descripción del Problema
La agricultura es un sector crucial para la economía mundial, y la detección temprana de plagas es esencial para preservar la salud de los cultivos y garantizar la rentabilidad de los agricultores. Las plagas pueden causar daños graves, reduciendo la calidad y cantidad de producción. Este proyecto tiene como objetivo desarrollar un sistema de detección de plagas basado en imágenes mediante Deep Learning, proporcionando una herramienta eficaz para monitorear cultivos y permitir decisiones informadas.

## 2. Objetivos del Proyecto
- **Identificación de Plagas:** Desarrollar un modelo de clasificación de imágenes que pueda identificar diferentes tipos de plagas en cultivos de hortalizas.
- **Mejora de Eficiencia:** Crear una solución que permita la detección de plagas de forma rápida y precisa, reduciendo la dependencia de inspecciones manuales.

## 3. Selección de la Herramienta de IA
- **Herramienta Elegida:** TensorFlow/Keras.
- **Justificación:** 
  - TensorFlow ofrece flexibilidad y potencia para construir modelos de Deep Learning complejos.
  - Amplio soporte de la comunidad y documentación que facilitan la resolución de problemas comunes y acceso a recursos de aprendizaje.

## 4. Dataset Necesario
- **Tipo de Dataset:** Imágenes etiquetadas de cultivos de hortalizas, con ejemplos de plagas y plantas sanas.
- **Descripción del Dataset:** 
  - Clasificación de insectos en 9 clases de plagas en cultivos hortícolas. Se utiliza el siguiente dataset de Kaggle: [Pest Dataset](https://www.kaggle.com/datasets/simranvolunesia/pest-dataset).
  - Debido a limitaciones de tiempo, no fue posible entrenar un modelo de alta precisión, ya que el dataset contiene muchas imágenes duplicadas y pocas muestras por clase. Se implementaron técnicas de data augmentation para aumentar la variedad de imágenes, pero los resultados iniciales aún pueden mejorarse.
- **Aumento de Datos:** Se utilizan técnicas como rotaciones, cambios de escala, y variaciones de iluminación para incrementar la variedad y robustez del modelo.

## 5. Modelos de Deep Learning Seleccionados
- **Modelo Elegido:** Convolutional Neural Network (CNN)-- MobileNetV2.
- **Justificación:**
  - Las CNN son efectivas para clasificación de imágenes, captando patrones y características espaciales.
  - Arquitecturas preentrenadas como `EfficientNet`, `MobileNetV2` o `ResNet` pueden utilizarse para mejorar la precisión a través de un ajuste fino (fine-tuning).
  

## 6. Proceso de Entrenamiento del Modelo
- **División del Dataset:** Conjuntos de entrenamiento, validación y prueba en una proporción de 70-20-10.
- **Configuración del Modelo:** 
  - **Función de Pérdida:** Categorical Crossentropy.
  - **Optimizador:** Adam.
  - **Hyperparámetros Iniciales:** 50 epochs y batch size de 32, ajustables según la convergencia del modelo.
- **Evaluación del Modelo:** Se medirán precisión, recall, F1-score y matriz de confusión para evaluar el rendimiento del modelo.

## 7. Enfoque de Implementación
- **Entorno Real:**
  - **Aplicación Móvil/Web:** Permitir a los agricultores subir imágenes y recibir retroalimentación en tiempo real sobre la presencia de plagas.
  - **Integración con IoT:** Evaluar la posibilidad de integrar sensores IoT para capturar imágenes automáticamente en los cultivos.
- **Capacitación:** 
  - **Talleres para Agricultores:** Organizar capacitaciones sobre el uso de la aplicación y la interpretación de resultados para asegurar que comprendan cómo aprovechar la herramienta.

## 8. Resultados Esperados
- **Detección Temprana de Plagas:** Permitir la detección oportuna de plagas, reduciendo el uso de pesticidas y mejorando la salud de los cultivos.
- **Aumento de la Productividad:** Mejora en la productividad agrícola al ofrecer detección precisa y rápida de plagas, beneficiando a agricultores y consumidores.

## 9. Conclusiones
Este proyecto explora una aplicación innovadora de Deep Learning en la agricultura, proporcionando una solución técnica que responde a una necesidad crítica del sector. Con un enfoque estructurado y el uso de herramientas avanzadas, buscamos no solo detectar plagas, sino también empoderar a los agricultores en la gestión sostenible de sus cultivos. La limitada disponibilidad de datos y el tiempo de desarrollo iniciales abren la puerta a futuras mejoras y a la aplicación de técnicas avanzadas de transferencia de aprendizaje para alcanzar una solución más robusta.

---

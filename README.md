# capstone-project
Este repositorio contiene un modelo de **identificación y separación de células positivas y negativas** en imágenes de microscopía, utilizando técnicas de Visión por Computador y Deep Learning.

El objetivo es ofrecer un pipeline reproducible que permita:

- Detectar y segmentar células en una imagen.
- Clasificar cada célula como **positiva** o **negativa**.
- Generar métricas cuantitativas (porcentaje de células positivas, conteo total, mapas visuales, etc.).

---

## 🧠 Descripción del proyecto

En muchas aplicaciones de patología digital y biología celular es crítico cuantificar cuántas células expresan un marcador (positivas) frente a las que no lo expresan (negativas).  
Este proyecto automatiza ese proceso a partir de imágenes de microscopía.

El pipeline típico incluye:

1. **Preprocesamiento de imagen**  
   - Normalización, redimensionamiento, filtrado de ruido.
2. **Segmentación de células**  
   - Separación de células individuales (por ejemplo, usando modelos tipo U-Net u otros segmentadores).
3. **Clasificación positiva/negativa**
   - Asignación de una etiqueta (0 = negativa, 1 = positiva) a cada célula detectada.
4. **Generación de resultados y métricas**  
   - Conteo de células.
   - Porcentaje de positivas.
   - Visualización de la imagen con overlay de colores por célula.

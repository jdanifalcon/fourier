---

# Intercambio de Magnitud y Fase con Transformada de Fourier

Este proyecto explora cómo la transformada de Fourier puede usarse para manipular imágenes intercambiando sus componentes de magnitud y fase. El experimento ilustra cómo se descompone una imagen en diferentes partes y qué sucede cuando esas partes se mezclan entre dos imágenes distintas.

## Objetivo

El objetivo de este ejercicio es demostrar el papel que juegan la **magnitud** y la **fase** en la composición de una imagen. Al intercambiar la magnitud de una imagen con la fase de otra, podemos observar cómo estos componentes afectan la percepción visual de la imagen resultante.

## Descripción Técnica

La transformada de Fourier permite descomponer una imagen en:
- **Magnitud**: Representa la amplitud de las frecuencias presentes en la imagen. Proporciona la estructura general y la energía.
- **Fase**: Define la posición espacial de las frecuencias. Contiene información crítica para la apariencia precisa de la imagen.

### Proceso del Experimento

1. **Selección de Imágenes**: Se utilizan dos imágenes: una foto en blanco y negro de la actriz Hedy Lamarr y una imagen de margaritas. 
2. **Transformada de Fourier**: Ambas imágenes se transforman a su representación en el dominio de la frecuencia usando la FFT (Fast Fourier Transform).
3. **Intercambio de Componentes**: Se intercambia la magnitud de la imagen de Hedy Lamarr con la fase de la imagen de las margaritas, y viceversa.
4. **Reconstrucción**: Se aplica la transformada inversa de Fourier para obtener las imágenes resultantes.

### Resultados

A continuación, se muestran las imágenes originales y las resultantes tras el intercambio:

- **Imagen Original 1**: Hedy Lamarr
- **Imagen Original 2**: Margaritas
- **Resultado 1**: Magnitud de Hedy Lamarr + Fase de Margaritas
- **Resultado 2**: Magnitud de Margaritas + Fase de Hedy Lamarr

## Visualización

Las imágenes finales muestran cómo la magnitud y la fase afectan la apariencia visual. Cuando se usa la magnitud de una imagen y la fase de otra, el resultado tiende a parecerse más a la imagen que aporta la fase. Esto destaca la importancia de la fase en la definición de la estructura detallada de la imagen.

![Imágenes Intercambiadas](ruta_a_las_imagenes)

## Uso

Para replicar este experimento, asegúrate de tener instaladas las siguientes bibliotecas en tu entorno de Python:

```bash
pip install numpy matplotlib
```

Puedes ejecutar el código proporcionado en `fft_image_swap.py` para ver los resultados por ti mismo.

## Código Ejemplo

Aquí un extracto de cómo se realiza el intercambio en Python:

```python
import numpy as np
import matplotlib.pyplot as plt

# Funciones para aplicar FFT y realizar el intercambio
# (Código de ejemplo para calcular FFT, intercambiar magnitudes y fases)

# Cargar imágenes en escala de grises
# Calcular la FFT
# Intercambiar componentes y reconstruir
```

## Conclusión

Este ejercicio ayuda a entender cómo la información de la fase y la magnitud afectan la composición visual de una imagen. Es una demostración sencilla pero poderosa de conceptos de procesamiento de señales aplicados a imágenes.

## Recursos Adicionales

- [Documentación sobre FFT en NumPy](https://numpy.org/doc/stable/reference/routines.fft.html)
- [Transformada de Fourier para imágenes](https://en.wikipedia.org/wiki/Fourier_transform)

---

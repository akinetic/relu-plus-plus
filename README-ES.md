# "ReLU Plus Plus"

ReLU++: Una función de activación ReLU modificada con rendimiento mejorado para modelos de aprendizaje profundo (*Deep Learning*).

Una implementación mejorada de la función de activación ReLU, con una pendiente ajustable para valores positivos y negativos.

### Descripción

La función de activación ReLU (Unidad Lineal Rectificada) es una de las más populares en las redes neuronales profundas. Sin embargo, presenta algunas limitaciones, como la pérdida de información en los valores negativos (el problema de "Dying ReLU").

"ReLU Plus Plus" es una variante de la función ReLU que busca mitigar estas limitaciones. Permite ajustar la pendiente tanto para valores positivos como negativos, lo que puede mejorar el rendimiento y la robustez de las redes neuronales en diversas tareas.

### Fórmula

La función "ReLU Plus Plus" se define como:

Si x < 0, entonces f(x) = ax

Si x ≥ 0, entonces f(x) = bx

Donde a y b son parámetros que controlan la pendiente para los valores negativos y positivos, respectivamente, y 1 ≥ b > a ≥ 0.

Es importante notar que ReLU (a=0, b=1), Leaky ReLU (a=0.01, b=1), y Parametric ReLU (a=0.05, b=1) son casos especiales de ReLU++, lo que convierte a ReLU++ en una generalización más flexible y eficiente de estas funciones de activación.

### Características

- Pendiente ajustable para valores positivos y negativos.
- Compatible con las principales librerías de aprendizaje automático (TensorFlow, PyTorch, etc.).
- Fácil de implementar y usar.

### Instalación

Para instalar "ReLU Plus Plus", puedes usar el siguiente comando:

```
git clone https://github.com/akinetic/relu-plus-plus.git
```

_Uso_

Para usar "ReLU Plus Plus" en tus modelos de aprendizaje automático, simplemente importa la función y úsala como cualquier otra función de activación:

```
from relu-plus-plus import relu-plus-plus

Create a machine learning model
model = tf.keras.models.Sequential([
    tf.keras.layers.Dense(64, activation=relu-plus-plus(a=0.1, b=0.5)),
    tf.keras.layers.Dense(10, activation='softmax')
])
```

_Contribución_

"ReLU Plus Plus" es un proyecto de código abierto (open-source), y cualquier contribución es bienvenida. Si deseas contribuir, por favor bifurca el repositorio (fork the repository) y envía una solicitud de extracción (pull request).

_Autores_
- Alex
- Lumin

_Licencia_

"ReLU Plus Plus" se distribuye bajo la licencia MIT.

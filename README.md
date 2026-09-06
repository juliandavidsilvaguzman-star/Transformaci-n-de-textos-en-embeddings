
# Transformación de textos en embeddings
# Procesamiento de Lenguaje Natural: Transformación de Textos en Embeddings

## Docente: Paul Alexander Diaz Montaña
## Alumno: Julián Davied Silva Guzman
## Fecha: 06/09/2026

### Descripción del Proyecto

Este repositorio contiene un ejemplo práctico para demostrar la **transformación de texto en embeddings** y su posterior aplicación en la **búsqueda de similitud semántica** utilizando la librería `sentence-transformers` en Python. El objetivo es convertir texto (palabras, frases o documentos) en vectores numéricos (embeddings) que una computadora puede procesar y comparar. Estos embeddings representan el significado semántico del texto, de modo que textos con significados similares quedan ubicados cerca unos de otros en un espacio matemático.

### Funcionalidades Clave

El cuaderno aborda las siguientes funcionalidades:

- **Instalación de Librerías:** Configuración del entorno con las herramientas necesarias (`sentence-transformers`, `pandas`, `scikit-learn`).
- **Selección de Dispositivo:** Detección automática y uso optimizado de GPU (CUDA) o CPU para el procesamiento.
- **Carga de Modelo Multilingüe:** Utilización del modelo `paraphrase-multilingual-MiniLM-L12-v2` para generar embeddings.
- **Generación de Embeddings:** Conversión de textos en vectores numéricos de 384 dimensiones que capturan su significado semántico.
- **Cálculo de Similitud Semántica:** Medición de la relación entre textos mediante la similitud del coseno.
- **Búsqueda por Consulta:** Identificación de los textos más relevantes a una pregunta dada basándose en su significado.
- **Persistencia de Datos:** Guardado de los embeddings generados en archivos CSV para su reutilización.
- **Procesamiento de CSV Externos:** Opción para cargar y procesar textos desde archivos CSV propios del usuario.

### Análisis General y Conclusiones

Este ejemplo práctico ha demostrado un flujo de trabajo completo para la **transformación de texto en embeddings y su posterior aplicación en la búsqueda de similitud semántica**, utilizando el poder de los modelos de `SentenceTransformer`.

**Análisis General:**

1.  **Preparación del Entorno:** El proceso comienza con la instalación de las librerías necesarias (`sentence-transformers`, `pandas`, `scikit-learn`) y la importación de los módulos clave. La detección automática del dispositivo (`cuda` o `cpu`) asegura la optimización del rendimiento, aprovechando la GPU cuando está disponible.
2.  **Carga y Uso del Modelo:** Se cargó un modelo multilingüe (`paraphrase-multilingual-MiniLM-L12-v2`), lo que permite el procesamiento de texto en varios idiomas. Esto es fundamental para la flexibilidad de la solución.
3.  **Generación de Embeddings:** El corazón del ejemplo práctico es la conversión de textos en vectores numéricos de 384 dimensiones. Estos embeddings son representaciones densas que capturan el significado semántico del texto, una pieza clave para que las máquinas puedan 'entender' el lenguaje humano.
4.  **Similitud Semántica:** La similitud del coseno fue utilizada para cuantificar la relación semántica entre los textos. Se observó claramente cómo frases con significados similares resultan en valores de similitud altos, mientras que frases dispares tienen valores bajos. Esto fue evidenciado tanto en la matriz de similitud como en la búsqueda por consulta.
5.  **Búsqueda y Relevancia:** La demostración de búsqueda por consulta mostró la capacidad del sistema para encontrar los textos más relevantes a una pregunta dada, ordenándolos por su similitud semántica. Esto es aplicable en motores de búsqueda, sistemas de recomendación, y análisis de documentos.
6.  **Persistencia y Escalabilidad:** El ejemplo práctico ofrece soluciones para guardar los embeddings generados en un archivo CSV, lo que permite su reutilización sin necesidad de recálculo. Además, la funcionalidad de cargar textos desde un CSV externo hace que el proceso sea escalable para trabajar con grandes volúmenes de datos propios del usuario.

**Conclusiones:**

*   **Potencial de los Embeddings:** Los embeddings de texto son una herramienta extremadamente poderosa en el Procesamiento del Lenguaje Natural (PLN), permitiendo a las máquinas trabajar con el significado contextual de las palabras y frases, no solo con su forma literal.
*   **Aplicaciones Versátiles:** Las técnicas demostradas son la base de muchas aplicaciones de IA, incluyendo:
    *   **Búsqueda Semántica:** Mejora la relevancia de los resultados de búsqueda.
    *   **Recomendación de Contenido:** Sugiere elementos basados en el significado, no solo en palabras clave.
    *   **Clasificación de Texto:** Agrupa documentos similares.
    *   **Detección de Plagio:** Identifica contenido con significado similar.
*   **Facilidad de Uso:** Librerías como `sentence-transformers` simplifican la implementación de estas técnicas avanzadas, democratizando el acceso a la IA del lenguaje.
*   **Impacto Práctico:** La capacidad de procesar y comparar textos a nivel semántico tiene un impacto significativo en la automatización y la mejora de la eficiencia en tareas relacionadas con la información y el conocimiento.

En resumen, este ejemplo práctico ha proporcionado una comprensión práctica y funcional de cómo transformar texto en representaciones numéricas significativas y utilizarlas para medir la similitud semántica, un concepto fundamental en el PLN moderno.

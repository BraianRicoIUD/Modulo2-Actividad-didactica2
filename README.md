# Actividad Didáctica 2 - Modelo Oculto de Markov (HMM)

Este repositorio contiene la implementación y simulación de un Modelo Oculto de Markov (HMM) desarrollado para modelar el clima real (estado oculto) a partir de mediciones de humedad ambiental (observación visible). 

El proyecto analiza la evolución estocástica a corto plazo (30 días) y evalúa la convergencia empírica frente a la distribución estacionaria teórica mediante simulaciones a gran escala (10,000 iteraciones).

---

## 🚀 Ejecutar en la Nube (Google Colab)

Puedes interactuar con la simulación completa y ejecutar el código con un solo clic directamente desde tu navegador:

👉 **[Abrir Simulación en Google Colab](https://colab.research.google.com/drive/1SRsu_uMXv-D0z6sikCXuZMA1m--8Kan-#scrollTo=NZ9qhK1uSSIv)**

---

## 🛠️ Tecnologías y Librerías Utilizadas

El entorno de Google Colab ya incluye estas librerías por defecto, pero si deseas replicarlo localmente, el script utiliza:
* **NumPy:** Para el manejo de matrices y la selección estocástica indexada (`np.random.choice`).
* **Pandas:** Para la estructuración de los datos simulados y la creación de la matriz de confusión.
* **Matplotlib y Seaborn:** Para la generación de los gráficos de barras apiladas, mapas de calor y curvas de convergencia.

## 📊 Componentes del Notebook
1. **Explicación Conceptual y Formulación:** Delimitación del problema del clima y pertinencia del modelo HMM.
2. **Validación Matemática:** Comprobación automatizada de que todas las distribuciones de probabilidad sumen exactamente 1.
3. **Simulación Base (30 días):** Generación de secuencias temporales correlacionadas y gráficos comparativos alineados.
4. **Análisis de Convergencia:** Simulación de 300,000 días acumulados para demostrar de forma empírica la Ley de los Grandes Números frente a la distribución estacionaria calculada analíticamente mediante vectores propios.

# Aplicando LSA en PAES de Competencia Lectora

**Zhongzhe Cheng - Benjamín Pardo Albornoz**  
Proyecto final — Álgebra Lineal

Este repositorio contiene el código y los archivos necesarios para reproducir el análisis semántico latente (LSA) aplicado a un corpus de textos extraídos de las pruebas PAES de Competencia Lectora (DEMRE, Chile).

---

## Contenido del repositorio

```
├── notebooks/
  ├── Exploracion_LSA_PAES.ipynb   # Notebook principal con todo el análisis
  ├── stopword.txt                 # Lista de stopwords en español
  ├── stopword_IA.txt              # Lista complementaria de stopwords
  ├── paths.txt                    # Rutas a los documentos del corpus
├── textos/                      # Carpeta con los 57 documentos .txt
  ├── 2023m-04
  ├── ...
└── README.md
```

---

## Datos

Los textos utilizados son fragmentos extraídos de las pruebas oficiales PAES y PDT, disponibles públicamente en:

> [https://demre.cl/publicaciones](https://demre.cl/publicaciones)

Para reproducir el análisis, descarga los documentos desde esa página y colócalos en una carpeta llamada `textos/`. Luego actualiza el archivo `paths.txt` con las rutas correspondientes a tu sistema.

El corpus final consta de **57 documentos** en español, con una extensión de entre 200 y 800 palabras cada uno.

---

## Requisitos

Se recomienda usar Python 3.9 o superior. Para instalar las dependencias necesarias, ejecuta:

```bash
pip install -r requirements.txt
```

Las librerías principales que se utilizan son:

- `scikit-learn` — vectorización TF-IDF y preprocesamiento
- `spacy` — lematización en español
- `numpy` — cálculo de SVD
- `matplotlib` — generación de figuras

Además, es necesario descargar el modelo de español de spaCy:

```bash
python -m spacy download es_core_news_sm
```

---

## Instrucciones de ejecución

1. Clona este repositorio:
```bash
git clone https://github.com/Cheng-0201/IMT2230-Proyecto-SVD.git
cd lsa-paes
```

2. Instala las dependencias:
```bash
pip install -r requirements.txt
python -m spacy download es_core_news_sm
```

3. Asegúrate de que los textos estén en la carpeta `textos/` y que `paths.txt` apunte a ellos correctamente.

4. Abre y ejecuta el notebook en orden:
```bash
jupyter notebook Exploracion_LSA_PAES.ipynb
```

Ejecutar todas las celdas en orden reproduce todas las figuras y resultados del informe.

---

## Figuras reproducibles

| Figura | Descripción | Celda del notebook |
|--------|-------------|-------------------|
| Fig. 1 | Términos más frecuentes sin preprocesamiento | Sección 1 |
| Fig. 2 | Decaimiento de valores singulares | Sección 3 |
| Fig. 3 | Plano LSA: componentes 1 vs 2 | Sección 4 |
| Fig. 4 | Plano LSA: componentes 2 vs 3 | Sección 4 |
| Fig. 5 | Plano LSA: componentes 3 vs 4 | Sección 4 |

---

## Notas

- Si se ejecuta localmente, verificar que las rutas en `paths.txt` sean correctas para el sistema operativo utilizado.
- Los archivos de stopwords (`stopword.txt` y `stopword_IA.txt`) son necesarios para reproducir exactamente los resultados. Están incluidos en el repositorio.


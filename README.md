# IMT2230-Proyecto-SVD

Exploracion semantica sobre los textos que usan la PAES (y PDT) de Competencia Lectora.

## Eleccion y descripcion del corpus

### Descripción del corpus

**Fuente: Publicaciones oficiales del DEMRE** (Departamento de Evaluación, Medición y Registro Educacional), disponibles en demre.cl/publicaciones. Los archivos son PDFs de acceso público que contienen las pruebas completas de la PAES (Prueba de Acceso a la Educación Superior) y sus versiones de ensayo (PDT), con sus respectivos textos de comprensión lectora.

### ¿Cuántos documentos?

El corpus está compuesto por **56 textos** extraídos de las pruebas de comprensión lectora de PAES y PDT oficiales. Cada texto corresponde a un fragmento discontinuo o continuo presentado en la prueba, **con un largo que oscila entre 200 y 800 palabras aproximadamente**, lo que garantiza una cantidad razonable de contenido por documento.

### ¿Por qué es interesante?

El corpus es atractivo por varias razones. Primero, los textos **son seleccionados por especialistas del DEMRE siguiendo criterios técnicos y curriculares precisos, lo que los convierte en una muestra curada de lectura "legítima" según el sistema educativo chileno.** Segundo, al abarcar múltiples años de aplicación, permite estudiar cómo evolucionan en el tiempo las características de los textos seleccionados: temáticas, géneros discursivos, extensión, nivel de complejidad léxica y estructura. Tercero, la fuente es completamente abierta y oficial, lo que hace el corpus replicable y verificable.

## Hipotesis inicial

"Hipotetizamos que el corpus de textos PAES presenta diversidad temática (entre 3 a 5 categorías) y tipológica (al menos 3 géneros discursivos), y que esta diversidad se mantiene relativamente estable a lo largo de las distintas versiones de la prueba o los diferentes periodos de evaluacion."

## Preprocesamiento

Usamos eliminacion de Stopwords, Lematizacion y TF-IDF para limpiar los textos.

## Notebook

Todos los pasos estan en el [notebook](./notebooks/Exploracion%20LSA%20PAES%20(y%20PDT).ipynb)

## Licencia

Este repositorio está licenciado bajo Creative Commons CC-BY 4.0.
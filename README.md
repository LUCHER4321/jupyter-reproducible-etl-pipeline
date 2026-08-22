# Laboratorio Práctico 2 · Pipeline ETL reproducible

## Curso

**Análisis de Datos**  
Magíster en Data Science  
Facultad de Ingeniería  
Universidad del Desarrollo

---

## Descripción

Este laboratorio tiene como objetivo desarrollar habilidades para construir procesos reproducibles de extracción, transformación y carga de datos (ETL).

En el Laboratorio Práctico 1 se realizó una exploración inicial del conjunto de datos y se identificaron distintos problemas de calidad. En esta actividad se dará el siguiente paso: transformar los datos originales mediante un proceso sistemático, documentado y reproducible.

El objetivo no es simplemente obtener un dataset "limpio", sino desarrollar un flujo de trabajo que permita:

* identificar los problemas relevantes;
* tomar decisiones de transformación;
* implementar dichas decisiones mediante código;
* validar los resultados;
* generar un dataset preparado para análisis posteriores.

---

## Contexto del dataset

Se continuará trabajando con el mismo conjunto de datos utilizado en el Laboratorio Práctico 1.

El dataset corresponde a información de clientes de una empresa de retail e incluye variables relacionadas con:

* características demográficas;
* características económicas;
* comportamiento de compra;
* interacción con la empresa;
* satisfacción del cliente.

El uso del mismo dataset permite dar continuidad al análisis desarrollado previamente y concentrar el trabajo en la construcción de un pipeline ETL reproducible.

---

## Archivos disponibles

Este directorio contiene los siguientes archivos:

### `clientes_retail.csv`

Dataset original utilizado como fuente de datos.

Este archivo debe considerarse como la fuente **raw** del proceso ETL.

**No debe ser modificado ni sobrescrito durante el desarrollo del laboratorio.**

El dataset contiene problemas de calidad que deberán ser identificados y tratados de acuerdo con su naturaleza y contexto.

---

### `diccionario_clientes_retail.xlsx`

Documento descriptivo de las variables disponibles.

Incluye:

* nombre de variable;
* tipo esperado;
* descripción;
* ejemplo;
* observaciones relevantes de calidad.

Debe utilizarse como referencia para comprender el significado de las variables y apoyar las decisiones de transformación.

---

### `Laboratorio_2_Notebook_Template.ipynb`

Notebook plantilla para desarrollar la actividad.

El estudiante debe completar las secciones propuestas incluyendo:

* código;
* resultados;
* visualizaciones cuando sean pertinentes;
* decisiones metodológicas;
* validaciones;
* interpretación de resultados.

---

## Objetivo del laboratorio

Construir un pipeline ETL reproducible que transforme el dataset original en una versión preparada para análisis posteriores.

El proceso debe contemplar, como mínimo:

1. **Extract:** carga reproducible de los datos originales.
2. **Diagnóstico:** identificación de problemas relevantes.
3. **Transform:** tratamiento justificado de los problemas identificados.
4. **Ingeniería de variables:** creación de nuevas variables con utilidad analítica o de negocio.
5. **Validación:** comprobación de que las transformaciones produjeron resultados coherentes.
6. **Load:** generación de un dataset procesado sin modificar los datos originales.

---

## Preguntas orientadoras

El pipeline desarrollado debería permitir responder preguntas como:

* ¿Qué problemas de calidad deben ser tratados antes de utilizar los datos?
* ¿Qué decisiones de limpieza y transformación son apropiadas para cada problema?
* ¿Cómo se pueden implementar estas decisiones mediante código?
* ¿Qué variables derivadas podrían aportar información adicional?
* ¿Cómo verificar que las transformaciones fueron realizadas correctamente?
* ¿Cómo garantizar que otra persona pueda ejecutar nuevamente el proceso y obtener los mismos resultados?
* ¿Qué información del dataset procesado queda disponible para análisis posteriores?

---

## Decisiones de transformación

Una parte central del laboratorio corresponde a la justificación de las decisiones tomadas.

No existe necesariamente una única estrategia correcta para todos los problemas encontrados.

Para cada transformación relevante se debe considerar:

* problema identificado;
* decisión adoptada;
* justificación;
* implementación;
* resultado obtenido;
* validación.

El estudiante debe evitar aplicar transformaciones de manera automática sin considerar el contexto de los datos.

---

## Reproducibilidad

El pipeline debe construirse utilizando código y debe poder ejecutarse nuevamente desde el inicio.

El notebook debería permitir realizar el proceso:

```text
Datos originales
      ↓
   Extract
      ↓
  Diagnóstico
      ↓
 Transformación
      ↓
 Ingeniería de variables
      ↓
   Validación
      ↓
     Load
      ↓
Datos procesados
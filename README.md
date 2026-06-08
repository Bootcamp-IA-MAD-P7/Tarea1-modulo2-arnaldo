# Tarea1-modulo2-arnaldo
Guía de Estudio: Análisis Exploratorio de Datos (EDA)

Este repositorio contiene una guía estructurada orientada al aprendizaje y repaso del **Exploratory Data Analysis (EDA)**. El contenido ha sido optimizado con una redacción fluida, dinámica y natural, ideal tanto para lectura visual rápida como para herramientas de síntesis de voz (Text-to-Speech).

---

## 🚀 Índice de Contenidos

1. [¿Qué es el EDA y cuál es su propósito?](#1-qué-es-el-eda-y-cuál-es-su-propósito)
2. [¿Qué tipos de datos existen en un EDA?](#2-qué-tipos-de-datos-existen-en-un-eda)
3. [Diferencias entre análisis univariado, bivariado y multivariado](#3-diferencias-entre-análisis-univariado-bivariado-y-multivariado)
4. [¿Qué es la estadística descriptiva?](#4-qué-es-la-estatística-descriptiva)
5. [¿Qué es la limpieza de datos y qué tareas incluye?](#5-qué-es-la-limpieza-de-datos-y-qué-tareas-incluye)
6. [El papel de Pandas, Matplotlib y Seaborn](#6-el-papel-de-pandas-matplotlib-y-seaborn)
7. [¿Qué es una matriz de correlación y para qué sirve?](#7-qué-es-una-matriz-de-correlación-y-para-qué-sirve)
8. [¿Qué son los outliers, cómo se detectan y cómo se tratan?](#8-qué-son-los-outliers-cómo-se-detectan-y-cómo-se-tratan)
9. [¿Qué es el Hypothesis Testing y para qué sirve en el EDA?](#9-qué-es-el-hypothesis-testing-y-para-qué-sirve-en-el-eda)

---

### 1. ¿Qué es el EDA y cuál es su propósito?
El EDA, o Análisis Exploratorio de Datos por sus siglas en inglés, es la primera etapa fundamental en cualquier proyecto de datos. Su propósito principal es permitirnos "entender" el conjunto de datos antes de sacar conclusiones o entrenar modelos de Inteligencia Artificial. Imagina que es como revisar el mapa y el estado de un coche antes de emprender un viaje largo: te ayuda a conocer la estructura de la información, detectar errores, descubrir patrones ocultos, identificar anomalías y validar si los datos realmente sirven para resolver el problema que tienes entre manos.

---

### 2. ¿Qué tipos de datos existen en un EDA?
En el análisis exploratorio dividimos los datos en dos grandes familias: los cualitativos o categóricos, y los cuantitativos o numéricos. 

Dentro de los categóricos, tenemos los nominales, que son etiquetas sin un orden específico, como el país de origen o el estado civil; y los ordinales, que sí siguen una jerarquía lógica, como el nivel de estudios o los rangos militares. 

Por otro lado, los datos numéricos se dividen en discretos, que son valores enteros y contables, como el número de hijos o de coches; y continuos, que pueden tomar cualquier valor con decimales dentro de un rango, como la altura, el peso o el salario.

---

### 3. Diferencias entre análisis univariado, bivariado y multivariado
La diferencia radica en cuántas variables estamos cruzando al mismo tiempo. El análisis univariado se centra en una sola variable a la vez para entender cómo se distribuye y cuáles son sus valores centrales. El análisis bivariado da un paso más y analiza la relación directa entre dos variables, por ejemplo, si el gasto de un cliente aumenta a medida que suben sus ingresos. Finalmente, el análisis multivariado examina tres o más variables en simultáneo para entender interacciones mucho más complejas y evitar conclusiones engañosas causadas por variables ocultas.

---

### 4. ¿Qué es la estadística descriptiva?
La estadística descriptiva es la herramienta que nos permite resumir y organizar grandes volúmenes de datos de manera sencilla e informativa. En lugar de mirar miles de filas sueltas, usamos métricas para describir el grupo. Esto incluye las medidas de tendencia central, que nos dicen dónde se sitúa el medio de los datos mediante la media, la mediana y la moda; y las medidas de dispersión, como la varianza o la desviación estándar, que nos indican qué tan agrupados o alejados están los datos respecto a ese centro.

---

### 5. ¿Qué es la limpieza de datos y qué tareas incluye?
La limpieza de datos es el proceso de corregir, transformar o eliminar registros que estén dañados, duplicados o incompletos dentro de nuestro dataset. Si el EDA es el diagnóstico que revela los problemas, la limpieza es la cura. 

Entre las tareas más comunes están el manejo de valores nulos, donde decidimos si borrar las filas vacías o rellenarlas con estimaciones; la eliminación de filas duplicadas que puedan sesgar el análisis; el tratamiento de valores atípicos; y la normalización o escalado, que consiste en ajustar los números para que todas las variables jueguen bajo una misma escala matemática.

---

### 6. El papel de Pandas, Matplotlib y Seaborn
Estas tres librerías forman el equipo ideal para hacer un EDA en Python. Pandas es el motor de todo: sirve para cargar los datos, manipularlos, agruparlos y hacer la limpieza pesada en las tablas. Matplotlib es la librería base de visualización; te da un control total y absoluto sobre cada detalle de un gráfico, como los títulos, los ejes y los colores. Por último, Seaborn está construida encima de Matplotlib y está optimizada para gráficos estadísticos; te permite crear visualizaciones complejas, modernas y muy atractivas con poquísimas líneas de código.

---

### 7. ¿Qué es una matriz de correlación y para qué sirve?
Una matriz de correlación es una tabla que te muestra, de forma numérica y visual, cómo se relacionan todas las variables numéricas entre sí. Utiliza un coeficiente que va desde el menos uno hasta el uno. Si el valor está cerca de uno, significa que cuando una variable sube, la otra también. Si está cerca de menos uno, cuando una sube, la otra baja. En el EDA sirve muchísimo para identificar qué variables tienen un impacto real sobre lo que queremos predecir, y también para detectar variables redundantes que nos conviene eliminar.

---

### 8. ¿Qué son los outliers, cómo se detectan y cómo se tratan?
Un outlier, o valor atípico, es un dato que se desvía drásticamente del comportamiento común de los demás registros. Puede deberse a un error humano al escribir los datos, un fallo en los sensores, o simplemente a un evento real pero extremadamente raro. 

Para detectarlos usamos herramientas visuales como los diagramas de caja, o métodos matemáticos como el Rango Intercuartílico y el Z-Score. Para tratarlos existen tres caminos: eliminarlos si confirmamos que son errores, transformarlos matemáticamente para reducir su impacto, o dejarlos intactos si representan un comportamiento real e importante que el modelo debe aprender.

---

### 9. ¿Qué es el Hypothesis Testing y para qué sirve en el EDA?
El testeo o prueba de hipótesis es un método estadístico formal que nos ayuda a comprobar si las conclusiones o patrones que estamos viendo en los gráficos son verdaderos y sólidos, o si son simple fruto de la casualidad y el azar. Aunque el EDA es una etapa muy visual, el testeo de hipótesis le añade rigor científico. Nos sirve, por ejemplo, para asegurar con total certeza matemática si un grupo de usuarios se comporta de forma diferente a otro, o para validar si nuestros datos siguen una distribución normal antes de aplicar ciertos algoritmos.

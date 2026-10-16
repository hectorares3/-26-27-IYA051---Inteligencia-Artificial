# Reto 08 - Actividad práctica: fundamentos de Visión Artificial Clásica

Objetivo: En esta actividad vais a trabajar de forma práctica con algunos de los principales conceptos y operaciones utilizados en Visión Artificial Clásica.

El objetivo no es memorizar funciones de OpenCV, sino comprender cómo se transforma progresivamente una imagen hasta obtener información útil sobre los objetos que contiene. En visión clásica somos nosotros quienes decidimos qué información utilizar, cómo separar los objetos y qué características medir para poder tomar posteriormente una decisión.

Antes de comenzar, descargad el guion de la práctica y las imágenes necesarias para realizar los experimentos desde el Campus Virtual:
Materiales > Ejercicios > Vision artificial clasica

Comenzaremos entendiendo una imagen como una matriz de números, estudiando sus dimensiones, canales y valores de píxel. 
Realizaréis también operaciones matemáticas sencillas sobre imágenes para comprobar directamente sus efectos.
Después trabajaréis con diferentes representaciones del color, especialmente BGR y HSV, y utilizaréis histogramas para analizar la distribución de intensidades y colores.
Una parte importante de la práctica estará dedicada a la segmentación. Crearéis máscaras para aislar determinados objetos utilizando color o intensidad y experimentaréis modificando rangos y umbrales. Esto permitirá comprobar cómo cambios de iluminación, ruido o una mala elección de parámetros pueden afectar a una detección.
También experimentaréis con filtros, detección de bordes y operaciones morfológicas, observando cómo permiten eliminar ruido, reforzar estructuras o mejorar una segmentación.  
Posteriormente pasaréis de trabajar con píxeles a trabajar con objetos. Obtendréis contornos y calcularéis características como área, perímetro, relación de aspecto, circularidad, número de vértices, posición o color.  
Finalmente combinaréis algunas de estas características para construir pequeños detectores basados en reglas.

El proceso general será:  
  IMAGEN → SEGMENTACIÓN → REGIONES → CONTORNOS → OBJETOS → CARACTERÍSTICAS → DECISIÓN    
  
¿Para qué sirve?  
Este procedimiento constituye la base de numerosos proyectos de Visión Artificial Clásica: inspección industrial, conteo de objetos, control de calidad, robótica, análisis de documentos, sistemas de medida o detección de piezas, entre otros.  

Ante un nuevo problema deberéis aprender a plantearos preguntas como: ¿Cómo separo el objeto del fondo? ¿Qué ocurre si cambia la iluminación? ¿Qué características permiten distinguir unos objetos de otros? ¿Qué parámetros son adecuados? ¿Qué ocurre cuando aparece ruido o los objetos se tocan?  

Durante la práctica no os limitéis a ejecutar el código. Antes de cambiar un parámetro, intentad predecir qué ocurrirá; después comprobad el resultado.  
El objetivo final es que seáis capaces de entender y comenzar a diseñar vuestro propio pipeline de Visión Artificial Clásica, identificando qué información necesitáis extraer de una imagen y cómo convertirla progresivamente en una decisión.  

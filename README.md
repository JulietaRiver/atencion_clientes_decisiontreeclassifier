# atencion_clientes_decisiontreeclassifier

🎯 Objetivo del Proyecto
El objetivo de este proyecto fue analizar y predecir la probabilidad de conciliación de quejas registradas ante tres compañías específicas (Walmart, Aeroméxico y Bradescard), con base en características como el tiempo de resolución, el monto recuperado, y aspectos del proceso de atención como el medio de ingreso, procedimiento y modalidad de compra.
Se buscó identificar los factores más influyentes en la resolución efectiva de quejas, con el fin de proponer estrategias orientadas a mejorar la atención al cliente, la satisfacción y la retención.

🧭 Metodología de trabajo
1. Filtrado del dataset
Se partió de un conjunto amplio de datos de quejas, del cual se seleccionaron únicamente los casos correspondientes a las compañías Walmart, Aeroméxico y Bradescard, permitiendo un enfoque específico y aplicable.

2. Limpieza y transformación de datos
Se normalizaron los nombres de columnas (minúsculas y sin espacios).

Se convirtieron las columnas de fechas al tipo datetime.

Se creó la variable dias_resolucion como la diferencia entre la fecha de ingreso y la fecha de fin de la queja.

Se eliminaron o imputaron valores nulos relevantes según su contexto.

Se codificaron variables categóricas usando One-Hot Encoding.

3. Definición de la variable objetivo
Se creó una columna binaria llamada es_conciliado para identificar si una queja fue conciliada exitosamente (1) o no conciliada / desistida (0), en función del estado procesal.

4. Modelado predictivo
Se entrenó un modelo de clasificación usando árbol de decisión, con una división 70/30 entre datos de entrenamiento y prueba.
El modelo alcanzó una exactitud del 94%, con un F1-score balanceado de 0.91 a 0.96 entre clases, demostrando capacidad para identificar correctamente casos con alta probabilidad de resolución.

5. Interpretación e insights
Se identificaron las variables más influyentes, como:

Días de resolución

Monto recuperado

Tipo de procedimiento

Medio de ingreso

Esto permitió derivar recomendaciones prácticas para optimizar la atención y reducir el tiempo de respuesta.

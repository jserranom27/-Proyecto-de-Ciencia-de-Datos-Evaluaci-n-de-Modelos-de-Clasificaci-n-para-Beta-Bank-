<div align="center"> <img src="URL_DE_TU_IMAGEN" alt="Banner del Proyecto" width="100%"> </div>
🏦 Proyecto de Ciencia de Datos: Evaluación de Modelos de Clasificación para Beta Bank 💳📊
📌 Problema
Beta Bank busca reducir su tasa de pérdida de clientes mediante un modelo de clasificación que prediga con precisión si un cliente cancelará su cuenta. Sin embargo, el conjunto de datos presenta un fuerte desbalance de clases, donde la mayoría de los clientes permanecen en el banco y solo una minoría cancela su cuenta. Esto genera modelos que pueden mostrar alta precisión simplemente prediciendo siempre la clase mayoritaria, sin realmente identificar a los clientes en riesgo.

Nuestro objetivo es desarrollar un modelo predictivo robusto que equilibre precisión y recall, utilizando la métrica F1-score, y aplicar técnicas de sobremuestreo y submuestreo para mejorar su desempeño en la predicción de cancelaciones.

🏗️ Solución
Entrenamiento de Modelos Iniciales:
Se probaron tres algoritmos de clasificación sin aplicar técnicas de balanceo:

Árboles de Decisión
Bosques Aleatorios
Regresión Logística
📊 Resultados de F1-score en validación:

Árbol de Decisión: 0.6966
Bosque Aleatorio: 0.7166
Regresión Logística: 0.0786
Manejo del Desbalance de Clases:

Sobremuestreo: Se generaron nuevas muestras de la clase minoritaria para equilibrar la distribución.
Submuestreo: Se redujo la cantidad de muestras de la clase mayoritaria para nivelar los datos.
Resultados y Evaluación en el Conjunto de Prueba:

Con sobremuestreo, el Bosque Aleatorio alcanzó un F1-score de 0.8075 en validación.
En el conjunto de prueba, el mejor modelo fue Bosque Aleatorio con sobremuestreo, obteniendo un F1-score de 0.6042.
🛠️ Tecnologías Utilizadas
Python
Pandas
NumPy
Scikit-learn
Matplotlib
Seaborn
📈 Conclusiones
El Bosque Aleatorio con sobremuestreo fue el modelo más efectivo, demostrando que balancear el dataset mejora significativamente la predicción de cancelaciones.
La métrica F1-score validó que el modelo no solo predice correctamente a los clientes que se quedan, sino también a los que cancelan.
La solución desarrollada permitirá a Beta Bank anticipar cancelaciones y diseñar estrategias proactivas para la retención de clientes.

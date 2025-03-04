<div align="center"> <img src="Flux_Dev_A_highquality_modern_digital_illustration_of_a_futuri_0.jpeg" alt="Banner del Proyecto" width="100%"> </div>
# 🏦 Proyecto de Ciencia de Datos: Modelos Predictivos para Beta Bank 💳📊

## 📌 Problema
Cada mes, Beta Bank pierde clientes, lo que impacta sus ingresos. La dirección ha identificado que retener clientes es más rentable que adquirir nuevos. Para ello, se necesita un modelo que prediga con precisión qué clientes cancelarán su cuenta, permitiendo tomar medidas preventivas.

El desafío clave es el **desequilibrio de clases**, ya que la mayoría de los clientes permanecen en el banco, mientras que solo una minoría se da de baja. Esto genera modelos con alta precisión que ignoran la clase minoritaria, fallando en detectar clientes en riesgo.

El objetivo es desarrollar un modelo predictivo que **maximice el F1-score**, asegurando un equilibrio entre precisión y recuperación.

---

## 🏗️ Enfoque y Solución
Se probaron **tres modelos de clasificación iniciales** sin aplicar técnicas de balanceo:

- **Árboles de Decisión** 🌳  
- **Bosques Aleatorios** 🌲🌲  
- **Regresión Logística** 📉  

### 📊 Resultados iniciales (F1-score en validación):
✔️ **Árbol de Decisión**: 0.6966  
✔️ **Bosque Aleatorio**: 0.7166  
❌ **Regresión Logística**: 0.0786 (ineficiente para datos desbalanceados)  

Para mejorar la detección de clientes en riesgo, se aplicaron técnicas de balanceo de clases:

- 🔹 **Sobremuestreo**: Aumento de datos de la clase minoritaria.  
- 🔹 **Submuestreo**: Reducción de datos de la clase mayoritaria.  

### 📈 Mejor resultado tras balanceo:
✅ **Bosque Aleatorio con sobremuestreo** → F1-score en validación: **0.8075**  
✅ En el conjunto de prueba, este modelo logró un **F1-score de 0.6042**, superando el umbral requerido de **0.59**.  

---

## ⚙️ Tecnologías Utilizadas  
- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Seaborn  

---

## 🔎 Conclusiones  
✔️ **El Bosque Aleatorio con sobremuestreo fue el modelo más efectivo**, logrando predecir con precisión los clientes en riesgo de churn.  
✔️ **El balanceo de datos mejoró significativamente el rendimiento**, evitando sesgos hacia la clase mayoritaria.  
✔️ **Este modelo permitirá a Beta Bank implementar estrategias de retención**, reduciendo pérdidas y mejorando la relación con sus clientes.  

---

📌 **Ver el notebook completo aquí** 📑

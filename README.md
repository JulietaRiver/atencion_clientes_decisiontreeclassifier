# atencion_clientes_decisiontreeclassifier

# 🧠 Proyecto: Análisis y Predicción de Conciliación de Quejas – Atención al Cliente

Este proyecto tiene como objetivo analizar y predecir la probabilidad de que una queja presentada por clientes ante compañías como **Walmart**, **Aeroméxico** y **Bradescard** sea conciliada exitosamente, utilizando técnicas de análisis de datos y machine learning.

---

## 🎯 Objetivo

Identificar los factores clave que influyen en la conciliación de quejas con el fin de:
- Mejorar la **atención al cliente**
- Reducir el **tiempo de resolución**
- Prevenir el **abandono o insatisfacción**

---

## 📁 Dataset

Se utilizó un dataset público de quejas y devoluciones, del cual se filtraron más de 4,000 casos correspondientes a las tres compañías mencionadas.  
Columnas relevantes:
- `fecha_ingreso`, `fecha_fin`, `monto_recuperado`, `modalidad_compra`, `procedimiento`, etc.

---

## 🔧 Proceso de trabajo

1. **Carga y limpieza de datos**
   - Normalización de nombres de columnas
   - Conversión de fechas a tipo datetime
   - Cálculo de días de resolución (`dias_resolucion`)
   - Eliminación de columnas vacías o irrelevantes

2. **Creación de variable objetivo**
   - `es_conciliado = 1` si el estado procesal fue "Conciliada", `0` en caso contrario

3. **Codificación de variables categóricas**
   - Uso de `One-Hot Encoding` para variables como `modalidad_compra` y `procedimiento`

4. **Entrenamiento de modelo**
   - Árbol de decisión (`DecisionTreeClassifier`)
   - División 70/30 entrenamiento/prueba

5. **Evaluación**
   - Accuracy del modelo: **94%**
   - F1-score: balanceado entre clases (0.91 – 0.96)

---

## 📊 Resultados

- **Factores más influyentes**:
  - Tiempo de resolución
  - Monto recuperado
  - Tipo de procedimiento
- Casos conciliados suelen resolverse en menos de 15 días y con atención personalizada

---

## 💡 Conclusiones

> Un análisis efectivo del tiempo de atención, junto con la personalización en los procedimientos y compensaciones, permite predecir con alta precisión la probabilidad de conciliación.  
> Estas herramientas permiten tomar decisiones anticipadas para **mejorar la experiencia del cliente** y reducir quejas sin resolver.

---

## 🛠️ Herramientas

- Python
- Pandas
- Scikit-learn
- Matplotlib / Seaborn
- Árboles de decisión

---

## 📎 Autor

**Julieta Rivera Zamora**  


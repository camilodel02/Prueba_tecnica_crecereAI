# Prueba_tecnica_crecereAI
## 🗂️ Estructura Repositorio

```text
Prueba_tecnica_crecereAI/
│
├── Notebook_main_CamiloDelgado_CreceréAI.ipynb       # Notebook con el desarrollo del análisis
│
├── data/
│   └── prueba_analist_de_datos_crecere.csv           # Dataset sintético 
│
└── README.md
```
---
## Notebook
📘 Descripción del Proyecto
Este notebook analiza el comportamiento de deudores con mora superior a 180 días, con el objetivo de entender qué factores están asociados a la aceptación de acuerdos de pago. El análisis combina exploración de datos, razonamiento basado en hipótesis y modelos interpretables para identificar los principales determinantes económicos, patrimoniales y de estrategia de cobranza.

🧠 Enfoque Analítico

El análisis se estructura en tres etapas principales:

Análisis Exploratorio de Datos (EDA)

Revisión de calidad de datos y estadística descriptiva

Análisis de distribuciones mediante gráficos tipo violin y boxplot

Análisis de correlaciones para identificar relaciones lineales y posibles colinealidades

Evaluación de Hipótesis mediante Exploración de Datos
Se analizan hipótesis relacionadas con:

Nivel de ingresos y capacidad de pago

Monto total de la deuda

Diseño de la propuesta de pago (número de cuotas)

Estrategia de comunicación (agresiva vs. no agresiva)

Tenencia de bienes (propiedades)

El énfasis se pone en diferencias de distribución, solapamientos y ruido, evitando conclusiones basadas únicamente en promedios.

Modelado y Explicabilidad

Regresión logística explicativa (statsmodels) para evaluar dirección y significancia

Regresión logística predictiva (scikit-learn) para evaluar desempeño (AUC)

Análisis de importancia de variables mediante Permutation Importance

Interpretabilidad global y local utilizando SHAP values

📊 Principales Hallazgos

El monto total de la deuda es el factor más relevante y con mayor impacto negativo sobre la aceptación de acuerdos.

Propuestas con mayor número de cuotas aumentan significativamente la probabilidad de aceptación.

Los ingresos están asociados positivamente con la aceptación, aunque con alto solapamiento entre grupos.

La estrategia de comunicación agresiva se asocia a mayores tasas de aceptación, especialmente en deudores con propiedades, lo que sugiere efectos condicionados.

La decisión de aceptar un acuerdo es multifactorial y no lineal, sin un único determinante dominante.

⚠️ Consideraciones Importantes

Las relaciones observadas son asociativas, no causales.

Existen efectos de interacción que no son capturados por análisis bivariados simples.

El desbalance de clases fue tenido en cuenta durante el modelado para asegurar resultados robustos.

🛠️ Herramientas y Librerías

Python (pandas, numpy)

Visualización: seaborn, matplotlib

Modelado: statsmodels, scikit-learn

Explicabilidad: permutation importance, SHAP

🎯 Resultado

El notebook ofrece tanto insights analíticos como orientaciones accionables, mostrando cómo la flexibilidad en las propuestas de pago y una estrategia de comunicación segmentada según el perfil del deudor pueden mejorar la tasa de acuerdos aceptados en contextos de mora prolongada.

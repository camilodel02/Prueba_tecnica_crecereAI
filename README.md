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

Este notebook analiza a deudores con mora superior a 180 días para identificar factores asociados a la aceptación de acuerdos de pago. El análisis combina exploración de datos, evaluación de hipótesis y modelos de regresión logística interpretables.

A través de EDA y visualizaciones de distribución, se evalúan variables económicas y de negociación como monto de la deuda, ingresos, número de cuotas, estrategia de comunicación y tenencia de propiedades. Los resultados muestran que deudas más bajas y propuestas con mayor número de cuotas son los principales factores asociados a una mayor probabilidad de aceptación, mientras que ingresos, comunicación agresiva y patrimonio presentan efectos relevantes pero condicionados.

El estudio incluye modelos logísticos explicativos y predictivos, complementados con Permutation Importance y SHAP, que confirman que la aceptación de acuerdos es un proceso multifactorial y no lineal, con relaciones asociativas y no causales.

# Predicción de Score de Crédito

## Descripción General

Este proyecto educativo de ciencia de datos presenta una clasificación de score de crédito en un escenario ficticio. El notebook original compara Random Forest y KNN, y después utiliza el modelo con mayor exactitud registrada para generar predicciones de ejemplo.

## Metodología

1. cargar e inspeccionar `clientes.csv`;
2. codificar campos categóricos;
3. separar atributos y variable objetivo;
4. crear particiones de entrenamiento y prueba;
5. entrenar Random Forest y KNN;
6. comparar la exactitud registrada;
7. predecir scores para `novos_clientes.csv`.

## Imágenes Existentes

Las figuras originales se conservan y se explican en el [informe final](../../reports/final_report.md). La captura de la hoja de cálculo ilustra entrenamiento, etiquetas de prueba y predicciones. La imagen de KNN ilustra la clasificación por proximidad. La imagen original asociada a árboles sigue disponible, pero su legibilidad visual es limitada.

## Resultados Registrados

| Modelo implementado | Exactitud guardada en el notebook |
| --- | ---: |
| Random Forest | 0.8265 |
| KNN | 0.7350666666666666 |

Los valores pueden variar al ejecutar nuevamente el notebook porque la separación de entrenamiento y prueba no define `random_state`.

## Instalación

```bash
python -m venv .venv
python -m pip install -r requirements.txt
```

Abra `main.ipynb` en Jupyter y ejecute las celdas en orden. Consulte la [guía de datos](../../data/README.md), las [notas de seguridad](../../SECURITY.md) y el [roadmap](../../ROADMAP.md).

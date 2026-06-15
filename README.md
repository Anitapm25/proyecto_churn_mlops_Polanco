# Proyecto Churn MLOps

Este proyecto corresponde a una práctica inicial del módulo de MLOps.

El objetivo es construir una estructura básica de trabajo para un proyecto de Machine Learning que permita:

- Preparar datos.
- Entrenar un modelo.
- Evaluar métricas.
- Guardar el modelo entrenado.
- Exponer el modelo mediante una API.
- Ejecutar pruebas básicas.

## Problema del proyecto

Se trabajará con un caso simplificado de predicción de abandono de clientes, conocido como churn.

El modelo intentará predecir si un cliente podría abandonar un servicio, utilizando variables como edad, antigüedad, saldo promedio, reclamos y uso de aplicación móvil.

## Estructura del proyecto

```text
proyecto_churn_mlops
├── data
├── notebooks
├── src
├── models
├── api
├── tests
├── docs
├── README.md
└── requirements.txt
```

## Carpetas principales

- `data`: contiene los datos del proyecto.
- `notebooks`: contiene análisis exploratorios.
- `src`: contiene los scripts principales del modelo.
- `models`: contiene el modelo entrenado.
- `api`: contiene la API del modelo.
- `tests`: contiene pruebas automáticas.
- `docs`: contiene documentación y métricas.

## Flujo inicial del proyecto

El flujo básico será:

1. Preparar los datos.
2. Entrenar el modelo.
3. Evaluar el modelo.
4. Guardar las métricas.
5. Crear una API básica.
6. Probar el funcionamiento inicial.

## Flujo del Pipeline ML-Ops

<p align="center">
  <img src="docs/imagenpipeline/pipeline_mlops.png" width="250">
</p>

## Descripción del Pipeline ML-Ops

Este pipeline implementa un ciclo completo y automatizado para la operación continua de modelos de machine learning en producción. Su objetivo es garantizar que los modelos no solo sean precisos durante el entrenamiento, sino que se mantengan robustos, monitoreados y actualizables frente a cambios en los datos o en el entorno.
                                          
## Control de versiones
Este proyecto utiliza Git para registrar cambios y GitHub para respaldar el repositorio en la nube.
El uso de commits permite mantener trazabilidad sobre los cambios realizados en el código, la documentación y la estructura del proyecto.

### Mejoras realizadas (Mayo 2026)
### Algoritmos
- Regresión Logística (base)
- Random Forest (nuevo)

### Hiperparámetros modificados
- Random Forest: n_estimators=200, max_depth=15 

### Métricas
- Accuracy, Precision, Recall, F1-score, **ROC-AUC (nueva)**

### Nueva prueba de API
- Archivo: `tests/test_api_nueva.py`
- Ejecutar con: `python tests/test_api_nueva.py`

## Mejora técnica implementada:

- Se agregó el endpoint informativo /info...
   
### Autor
Ana Luisa - Antipam25
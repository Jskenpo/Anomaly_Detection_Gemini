# Anomaly Detection Gemini

## 1. ¿Qué se debe considerar al momento de elegir entre sensibilidad y precisión del umbral?

Al elegir entre sensibilidad y precisión, se deben considerar los siguientes factores:

- **Objetivo del modelo**:  
  - Si el objetivo es minimizar los **falsos negativos**, se debe priorizar la **sensibilidad (recall)**.  
    - Ejemplo: Diagnóstico médico (detección de cáncer), donde es crítico identificar todos los casos positivos.  
  - Si el objetivo es minimizar los **falsos positivos**, se debe priorizar la **precisión (precision)**.  
    - Ejemplo: Filtrado de correos spam, donde es importante que los correos legítimos no sean marcados como spam.

- **Costo de los errores**:  
  - Un alto costo por no detectar un positivo requiere mayor sensibilidad.  
  - Un alto costo por clasificar erróneamente como positivo requiere mayor precisión.

- **Balance entre ambas métricas**:  
  - En muchos casos, se busca un equilibrio utilizando métricas como **F1-score** o ajustando el umbral de decisión para optimizar la métrica más relevante para el problema.

La elección depende del contexto y del impacto que tengan los errores en la aplicación del modelo.

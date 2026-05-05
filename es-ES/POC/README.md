# Prueba de Concepto (POC): El Puente de Contexto

## 1. Alcance de la POC
El objetivo de la POC es demostrar que una IA puede identificar cuando un código enviado mediante un Pull Request (PR) **no cumple** con los criterios de aceptación definidos en una tarea de Jira.

## 2. Escenario de prueba
- **Entrada A:** Un ticket de Jira (por ejemplo, "Crear endpoint de login con validación de 2FA").
- **Entrada B:** Un diff de código (por ejemplo, código que crea el login, pero omite 2FA).
- **Salida esperada:** Un informe de la IA que indique: "Riesgo de calidad: el código implementa el login, pero falta la lógica de 2FA mencionada en el criterio de aceptación 2."

## 3. Arquitectura simplificada
1. **Datos simulados:** JSONs que simulan las APIs de Jira y GitHub.
2. **LLM Prompting:** Uso de Few-Shot Prompting para enseñar a la IA a comparar requisitos con código.
3. **Interfaz:** Un panel simple (Streamlit o Markdown estático) que compara "Esperado" vs. "Entregado".

## 4. Métricas de éxito de la POC
- Precisión en identificar "Brechas de Requisito" por encima del 80%.
- Tiempo de análisis inferior a 30 segundos por ticket/PR.

## Próximos pasos

- [Roadmap: Construcción de la POC (Fase 1)](ROADMAP/README.md)
- [Roadmap: Escalado a Producción (Fase 2+)](ROADMAP/after-poc-roadmap.md)

## Idiomas

- [Português (pt-BR)](../../pt-BR/POC/README.md)
- [English (en-US)](../../en-US/POC/README.md)

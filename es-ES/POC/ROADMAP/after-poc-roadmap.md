# Roadmap: Escalado a Producción (Fase 2+)

## Integración en tiempo real
- [ ] **Servicio de webhooks:** Implementar escucha activa para disparar análisis tan pronto como se abra un PR.
- [ ] **Integración con Jira:** Crear un widget en Jira que otorgue una "Puntuación de Calidad" a la historia antes de que llegue al desarrollador.

## Inteligencia avanzada
- [ ] **Análisis de sentimiento/esfuerzo:** Identificar señales de bajo compromiso mediante la verbosidad y claridad en los mensajes de commit.
- [ ] **Generación automática de tickets:** Si la IA detecta un bug recurrente en el código, sugerir automáticamente crear un ticket de deuda técnica.
- [ ] **Guías de estilo personalizadas:** Permitir que cada proyecto cargue su propio archivo de reglas (por ejemplo, "Este proyecto usa Clean Architecture estricta").

## Gobernanza y dashboards
- [ ] **Vista para managers:** Dashboard para gestores con métricas de "Calidad Evolutiva" del proyecto.
- [ ] **Feedback loop:** Permitir que el humano indique "IA, esta alerta fue un falso positivo", entrenando el modelo localmente.

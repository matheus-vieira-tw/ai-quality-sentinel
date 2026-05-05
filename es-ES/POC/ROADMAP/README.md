# Roadmap: Construcción de la POC (Fase 1)

## Setup y Diseño (Día 1-2)
- [ ] **Definición de la persona:** Crear el perfil del "Revisor Detallista" (la voz de la IA).
- [ ] **Dataset de prueba:** Seleccionar 5 ejemplos reales anonimizados de tickets buenos/malos y código correspondiente.
- [ ] **Elección del modelo:** Configurar acceso al modelo vía AI/works™ (o GPT-4/Claude para pruebas iniciales).

## Desarrollo (Día 3-5)
- [ ] **Módulo de extracción:** Script para leer texto de tickets (Markdown/JSON).
- [ ] **Módulo de análisis de código:** Script para procesar archivos `.diff` o `.py/.js`.
- [ ] **Ingeniería de prompts:** Crear el "System Prompt" que instruye a la IA a ser un auditor de calidad riguroso.
- [ ] **Validación de salida:** Crear una plantilla de respuesta (por ejemplo, Semáforo de Calidad - Verde/Amarillo/Rojo).

## Demostración (Día 6-7)
- [ ] **Grabación de video:** Demo comparando una revisión humana rápida con el análisis más profundo de la IA.
- [ ] **Documentación de resultados:** Tabla de "Antes vs Después" del uso de la herramienta.

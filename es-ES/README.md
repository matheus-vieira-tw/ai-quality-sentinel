# Visión general del proyecto: AI/Quality Sentinel (AI/QS)

## 1. El problema
La falta de calidad en proyectos de software muchas veces no es una falla técnica, sino una falla de **contexto**.
- **Brechas de entendimiento:** Requisitos vagos en Jira generan código que no satisface el negocio.
- **Falta de consistencia:** Plazos ajustados llevan al descuido de buenas prácticas.
- **Sobrecarga de revisión:** Revisores humanos (Tech Leads/Seniors) pierden tiempo con sintaxis y olvidan validar si la regla de negocio del ticket se cumplió.

## 2. La solución
**AI/Quality Sentinel** es un agente de gobernanza inteligente que actúa como un puente entre la gestión (Jira) y la ejecución (GitHub/GitLab). Analiza el "triángulo de calidad":
1. **Intención:** Lo que dice el ticket.
2. **Ejecución:** Lo que hace el código.
3. **Patrón:** Lo que exigen las buenas prácticas de Thoughtworks.

## 3. Objetivos principales
- Reducir el retrabajo en un 30% identificando desalineaciones antes del merge.
- Mejorar la salud del backlog mediante el análisis de calidad de las historias de usuario.
- Transformar al desarrollador en un "Revisor Estratégico", delegando el análisis detallado de patrones a la IA.

## 4. Diferenciador AI/works™
La solución usa la infraestructura segura de TW para garantizar que datos sensibles de clientes y código propietario se procesen bajo rigurosos estándares de privacidad.

## 5. Modelo de Equipo para Hackathon (hasta 3 personas)
- **Persona 1:** Producto y priorización (PO + SM)
- **Persona 2:** Desarrollo generalista enfocado en implementación core e integraciones
- **Persona 3:** Desarrollo generalista enfocado en implementación core y QA práctico

Para ver el mapa completo de contribución por rol y responsabilidades detalladas:
- [Roles del Equipo (Versión Hackathon)](roles/README.md)

### Prioridad de Ejecución en Hackathon
- Priorizar reglas de negocio, integraciones y evidencia de valor de punta a punta.
- Mantener la interfaz mínima en la primera iteración (API/CLI es válido para validar la demo).
- Evolucionar la interfaz solo si queda tiempo.

## 👥 Roles del Equipo

Conoce la estructura del equipo y cómo diferentes profesionales pueden ayudar:

- [Descripción General de Roles](roles/)

## Documentación

- [Prueba de Concepto](POC/README.md)

## Idiomas

- [Português (pt-BR)](../pt-BR/README.md)
- [English (en-US)](../en-US/README.md)

# Roles del Equipo (Version Hackathon) - AI/Quality Sentinel

Esta guia simplifica la estructura del equipo para un hackathon con hasta 3 personas.
El objetivo es acelerar decisiones, reducir overhead y enfocarse en entregar valor.

## Pagina Principal del Proyecto

Para la vision general de AI/Quality Sentinel (problema, solucion y objetivos), usa:
- [README del proyecto (es-ES)](../README.md)

## Estructura Recomendada (hasta 3 personas)

En hackathon, una persona puede asumir mas de un rol. La distribucion siguiente funciona bien para avanzar el POC sin depender de una separacion estricta FE/BE:

| Persona | Enfoque principal | Roles combinados |
|---|---|---|
| Persona 1 | Producto y priorizacion | Product Owner + Scrum Master |
| Persona 2 | Desarrollo (generalista) | Implementacion del core + integraciones |
| Persona 3 | Desarrollo (generalista) | Implementacion del core + QA practico |

## Responsabilidades Minimas por Frente

### 1. Producto y Priorizacion
- Definir el alcance minimo del hackathon (MVP).
- Priorizar backlog por impacto en la demo.
- Mantener alineacion entre problema, solucion y demo final.

Referencias:
- [Product Owner](product-owner.md)
- [Scrum Master](scrum-master.md)

### 2. Desarrollo Core (Persona 2)
- Implementar servicios y reglas principales del POC.
- Integrar datos y flujos necesarios para la demo.
- Garantizar funcionamiento end-to-end de los casos criticos.

Referencia:
- [Backend (.NET)](backend-dotnet.md)

### 3. Desarrollo Core + Calidad (Persona 3)
- Compartir implementacion del core con la Persona 2 (sin frontera fija FE/BE).
- Definir y ejecutar checklist rapido de calidad para flujos criticos.
- Cubrir lo esencial con pruebas (o guion de pruebas) para reducir riesgo en la presentacion.

Referencias:
- [QA](qa.md)
- [Frontend (React/Angular)](frontend-react-angular.md)

## Mapa de Contribucion por Rol

Esta seccion detalla como cada rol puede acelerar AI/Quality Sentinel en contexto de hackathon.

### Product Owner (PO)
- Traduce el problema de calidad en objetivos claros para el MVP.
- Define criterios de exito de la demo (que debe funcionar para mostrar impacto).
- Mantiene el foco en valor de negocio y evita alcance que no sera demostrado.

Referencia:
- [Product Owner](product-owner.md)

### Scrum Master (SM)
- Elimina bloqueos rapidamente (dependencias, decisiones pendientes, alineaciones).
- Organiza el flujo de trabajo para mantener productividad con bajo overhead.
- Garantiza una cadencia corta de seguimiento y ajuste del plan.

Referencia:
- [Scrum Master](scrum-master.md)

### Quality Assurance (QA)
- Define checklist minimo de calidad para los flujos mas criticos.
- Valida si los criterios de aceptacion del MVP realmente se cumplen.
- Ayuda a reducir riesgo en la presentacion con validacion orientada a escenarios.

Referencia:
- [QA](qa.md)

### Desarrollador Backend (.NET)
- Implementa servicios y reglas de negocio centrales de la solucion.
- Conecta integraciones necesarias para demostrar el ciclo completo (intencion -> ejecucion -> estandar).
- Estructura base tecnica para escalar el POC despues del hackathon.

Referencia:
- [Backend (.NET)](backend-dotnet.md)

### Desarrollador Frontend (React/Angular)
- Crea una experiencia minima para demostrar valor con claridad.
- Traduce resultados tecnicos en visualizaciones comprensibles para jurados y stakeholders.
- Apoya la narrativa de la demo cuando haya tiempo para evolucion de interfaz.

Referencia:
- [Frontend (React/Angular)](frontend-react-angular.md)

### Especialistas Adicionales (cuando disponible)
- DevOps: acelera setup, automatizacion y estabilidad del entorno.
- Datos: mejora calidad de insumos e interpretacion de resultados.
- Seguridad: reduce riesgos de exposicion y apoya buenas practicas desde el POC.

Referencia:
- [Especialistas Adicionales](additional-specialists.md)

## Referencias Rapidas de Todos los Roles

- [Product Owner](product-owner.md)
- [Scrum Master](scrum-master.md)
- [QA](qa.md)
- [Backend (.NET)](backend-dotnet.md)
- [Frontend (React/Angular)](frontend-react-angular.md)
- [Especialistas Adicionales](additional-specialists.md)

## Ritmo de Trabajo Ligero (Sugerencia)

- Daily corta: 10 minutos para alinear bloqueos y siguientes tareas.
- Checkpoint tecnico: 1 o 2 veces al dia para integrar frontend + backend.
- Revision final: validar guion de demo y plan B para fallas.

## Que No Priorizar en el Hackathon

- Procesos pesados de ceremonia.
- Cobertura amplia de pruebas fuera de flujos criticos.
- Alcance grande sin validacion de valor en la demo.

## Interfaz en el Contexto del Hackathon

- La interfaz puede ser minima o incluso reemplazada por flujo API/CLI en la primera iteracion.
- Prioriza primero: reglas de negocio, integraciones y evidencia de valor funcionando.
- Si sobra tiempo, evoluciona la interfaz para mejorar la narrativa de la presentacion.

## Equipo Actual

- [Matheus Costa Vieira](mailto:matheus.vieira@thoughtworks.com) - Desarrollo Backend (.NET)

## Siguiente Paso

Despues de validar este formato en todas las carpetas de idioma, mantener actualizaciones futuras sincronizadas entre en-US, pt-BR y es-ES.

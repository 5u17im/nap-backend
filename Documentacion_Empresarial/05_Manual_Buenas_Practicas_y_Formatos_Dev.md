# Manual de Buenas Prácticas de Desarrollo y Formatos de Control Técnico

Este documento dicta los estándares y rutinas que todos los operadores técnicos de la Célula Backend y Frontend deben acatar religiosamente para asegurar una trazabilidad gerencial y evitar "código espagueti".

## 1. Estándares y Flujo de Trabajo (*Git Workflow*)
- **Prohibición de Commits a Main:** Está estrictamente prohibido realizar despliegues o subidas de código directo a la rama principal (`main` o `production`). 
- **Ramas por Funcionalidad:** Todo desarrollo debe originarse en una rama separada (*Feature Branch*), por ejemplo: `feature/login-auth` o `hotfix/bug-pagos`.
- **Revisión por Pares (Pull Requests):** Para unir una nueva funcionalidad, el código debe ser validado y aprobado por el *Tech Lead* correspondiente de la Célula.
- **Commits Semánticos:** Se exige estandarización (ej. `feat: integra servicio de SMS`, `fix: error de alineación en perfil`).

## 2. Reportes de Frecuencia y Control Operacional

### A. Reporte Diario (*Daily Standup Async*)
A ejecutarse cada mañana en el canal de comunicación técnico del equipo (ej. Slack/Discord).
**Formato Obligatorio:**
> **1. ¿Qué paquete o tarea completé ayer?** (Describir avance).
> **2. ¿Qué tarea ejecutaré el día de hoy?** (Indicar módulo).
> **3. ¿Existe algún bloqueo o impedimento?** (Roadblock).

### B. Formato de Cierre de Tarea (*Issue / Ticket Closure*)
Al finalizar una funcionalidad asignada, el desarrollador debe documentar en la plataforma de gestión de proyectos (Jira/Trello/GitHub Projects):
**Formato Obligatorio:**
> **ID Tarea:** [Ref - ej. NAP-15]
> **Descripción del Cambio:** [Qué se programó y por qué]
> **Criterios de Aceptación:** [Lista de chequeo confirmando si cumple los requisitos]
> **Pruebas de Validación:** [Lista de pruebas realizadas. Ej: "Se intentó enviar el formulario vacío y generó error 400 correcto"]

### C. Reporte y Retrospectiva Mensual
A final de cada mes, se agendará una revisión (*Sprint Retrospective*) entre el Tech Lead y sus desarrolladores para evaluar:
- Cumplimiento de entregables.
- Identificación de deudas técnicas (*Technical Debt*) generadas por velocidad vs. calidad.
- Oportunidades de mejora operativa en la célula.

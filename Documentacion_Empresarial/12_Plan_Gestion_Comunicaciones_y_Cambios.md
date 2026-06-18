# Plan Integral de Comunicaciones y Gestión del Cambio

Como CEO has identificado correctamente que existen "puntos ciegos" administrativos. Este documento resuelve los vacíos de control mediante tres pilares: Cómo nos comunicamos, cómo gestionamos cuando el cliente/inversor quiere cambiar las cosas, y cuándo consideramos que algo está "Terminado".

## 1. Matriz de Comunicaciones
Define el flujo formal de información para evitar "teléfono roto".

| Ritual / Reporte | Frecuencia | Emisor | Receptor | Formato / Medio |
| :--- | :--- | :--- | :--- | :--- |
| **Daily Standup** | Diario | Devs / Tech Leads | Célula Interna | Asíncrono (Slack / Discord) - *Obligatorio* |
| **Sync Directivo** | Semanal | Tech Leads | CEO | Videollamada (30 mins) - *Decisiones Tácticas* |
| **Sprint Demo** | Quincenal | Tech Leads | CEO | Videollamada + Pantalla compartida (Entorno Staging) |
| **Reporte Financiero** | Mensual | Consultor Contable| CEO | Documento PDF / Hoja de Cálculo |
| **Update a Stakeholders**| Mensual | CEO | Socios / Asesores| Correo Electrónico (Métricas de Crecimiento) |

---

## 2. Gestión del Control de Cambios (Change Management)
Cualquier solicitud para agregar una funcionalidad que **no** esté en el ERS actual se considera un *Change Request* (Solicitud de Cambio) e impacta la triple restricción (Tiempo, Costo, Alcance). 

**Flujo de Aprobación de Cambios:**
1. **Solicitud:** El Interesado (B2B, Usuario o CEO) propone el cambio.
2. **Evaluación de Valor:** El CEO determina si aporta *Business Value* real o si es un "Capricho" visual (*Scope Creep*).
3. **Evaluación de Esfuerzo:** Si el CEO lo avala, el Backend y Frontend Lead estiman el costo técnico (Horas hombre / Complejidad API).
4. **Veredicto:** El CEO, basándose en la estimación de esfuerzo, decide: Aprobar, Posponer a v2.0, o Rechazar categóricamente.

---

## 3. Definición de "Terminado" (Definition of Done - DoD)
Para que un Tech Lead o Desarrollador marque un Paquete de Trabajo (WP) o tarea como "Completada" y exija su aprobación/pago, debe cumplir 100% de esta lista:

- [ ] **Desarrollo:** El código funciona según los Criterios de Aceptación del ERS.
- [ ] **Diseño:** El Frontend es responsivo (móvil y escritorio) y cumple los lineamientos UI/UX.
- [ ] **Pruebas (Testing):** El código compila sin errores. Se probaron "Happy Paths" y "Error Paths" básicos (ej. Contraseña incorrecta).
- [ ] **Revisión (Code Review):** El *Pull Request* fue revisado y aprobado por otro desarrollador / Tech Lead.
- [ ] **Despliegue:** El código está fusionado (*Merged*) y disponible en el entorno de pruebas (*Staging*) para revisión del CEO.

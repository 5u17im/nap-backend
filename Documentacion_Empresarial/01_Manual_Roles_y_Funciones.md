# Manual Organizacional: Roles, Funciones y Responsabilidades

**Entidad:** Nothing Sense (S.A.S. en Formación)

Este manual detalla a nivel granular las funciones y límites de responsabilidad de los actores principales y auxiliares en la ejecución del proyecto NAP.

## 1. Cargos Principales (C-Level / Dirección Técnica)

### 1.1. Chief Executive Officer (CEO) - Fredinson Solano Rois
- **Propósito:** Liderar la estrategia general, rentabilidad, modelo de negocio y marco legal de la corporación.
- **Funciones Directivas y Operativas:** 
  - Gestión de *Stakeholders* (Inversores, Clientes B2B, Consultores).
  - Firma, negociación y estructuración de acuerdos corporativos B2B.
  - Administración presupuestaria, control de caja y ejecución estricta de la "Regla de Cascadas" (orden de pagos).
  - Control de alcance (*Scope Creep*), con autoridad absoluta para aprobar o rechazar nuevas funcionalidades.
  - Resolución final en la Matriz de Escalamiento corporativo.

### 1.2. Backend Tech Lead - Steven Ricardo Quiñones
- **Propósito:** Diseñar, implementar y garantizar la escalabilidad y seguridad de la arquitectura del servidor.
- **Funciones Operativas:**
  - Modelado de bases de datos relacionales y seguridad transaccional garantizando propiedades ACID.
  - Diseño y ejecución de integraciones críticas con pasarelas de pago, motores de firmas electrónicas y facturación.
  - Auditoría de código (*Code Review*) y aprobación de *Pull Requests* de la célula Backend.
  - Definición y mantenimiento de los *API Contracts* bajo los cuales debe regirse la célula Frontend.

### 1.3. Frontend Tech Lead - Eduardo Morales
- **Propósito:** Materializar la experiencia de usuario y arquitectura del lado del cliente, garantizando una interfaz altamente funcional.
- **Funciones Operativas:**
  - Estructuración de la arquitectura UI/UX y manejo del estado global de la aplicación web.
  - Consumo riguroso y seguro de los servicios expuestos por el Backend.
  - Coordinación de la célula Frontend, asignando tareas a desarrolladores operativos y validando el rendimiento (*Performance*) en el navegador.

---

## 2. Cargos Auxiliares y Operativos

### 2.1. Desarrolladores Operativos (Backend / Frontend)
- **Propósito:** Fuerza de ejecución técnica subordinada a las células operativas.
- **Funciones:**
  - Desarrollo de Paquetes de Trabajo (*Work Packages*) definidos en el cronograma.
  - Generación de pruebas unitarias y documentación interna de su código.
  - Reporte diario de estado y alertas tempranas sobre *Roadblocks*.

### 2.2. Equipo Consultor Externo (Legal, Contable, Marketing)
- **Propósito:** Cubrir funciones especializadas bajo la figura de *Outsourcing* para mitigar cargas prestacionales.
- **Funciones:** Proveer servicios predefinidos por hitos (ej. Acuerdos de términos de servicio, habilitación tributaria, campañas publicitarias focalizadas), cobrando por entregable cumplido.

# Manual de Operaciones: Frontend Tech Lead

Este documento centraliza las rutinas operativas, protocolos visuales y entregables que el Frontend Tech Lead (Eduardo Morales) debe custodiar y ejecutar.

## 1. Documentos y Artefactos de Control Exclusivo (Frontend)
- **Sistema de Diseño (Design System / UI Kit):** Repositorio en Figma (u otra herramienta) con componentes estandarizados (Botones, Formularios, Tipografías, Colores). Evita retrabajos y mantiene consistencia visual.
- **Arquitectura de Estado Global:** Documentación sobre cómo se maneja la sesión del usuario, caché y estado de la aplicación (ej. Redux, Zustand, Context API).
- **Métricas de Rendimiento (Web Vitals):** Monitoreo del tiempo de carga inicial y respuesta de las interacciones en cliente.

## 2. Responsabilidades Operativas de Ejecución
- **Integración de *API Contracts*:** Consumo estricto de los endpoints provistos por el Backend. En caso de ausencia de API real, generar "Mocks" para no detener el desarrollo visual.
- **Revisión de Código (Code Review / PRs):** El líder debe aprobar los *Pull Requests* de desarrolladores frontend subordinados, validando:
  - Diseño responsivo (Mobile-First adaptado a escritorio).
  - Manejo de estados de carga (Loaders) y manejo de errores visibles al usuario (Alertas de fallo).
- **Mitigación de *Scope Creep* Visual:** Rechazar el uso de animaciones innecesarias o librerías pesadas que no aporten al *Business Value* inicial del MVP.

## 3. Rutina Semanal Sugerida
- **Lunes (Sincronización Visual):** Revisión de *Wireframes* a programar. Asignación de componentes al equipo.
- **Miércoles (Sincronización Directiva):** Reunión de 30 mins con CEO y Backend Lead para reportar bloqueos (ej. "Falta un campo en la respuesta del endpoint").
- **Viernes (Cierre Visual):** Pase de código al entorno de *Staging*. Verificación multiplataforma (iOS/Android navegadores).

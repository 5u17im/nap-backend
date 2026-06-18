# Manual de Operaciones: Backend Tech Lead

Este documento centraliza las rutinas operativas, protocolos técnicos y artefactos que el Backend Tech Lead (Steven Ricardo Quiñones) debe custodiar y ejecutar.

## 1. Documentos y Artefactos de Control Exclusivo (Backend)
- **Documentación de API (Swagger/OpenAPI):** Contrato técnico que define cómo el Frontend se comunicará con el servidor. Debe actualizarse antes de escribir el código del endpoint.
- **Esquema de Base de Datos (Prisma Schema):** Único responsable de las migraciones de base de datos (`schema.prisma`). 
- **Gestión de Secretos (.env):** Custodia y rotación de llaves de API (Pasarelas de pago, AWS, JWT Secrets). Nunca se exponen en repositorios públicos.

## 2. Responsabilidades Operativas de Ejecución
- **Revisión de Código (Code Review / PRs):** El líder debe aprobar los *Pull Requests* de desarrolladores backend subordinados, validando:
  - Ausencia de bucles infinitos y queries N+1.
  - Cobertura de pruebas unitarias en funciones de cálculo financiero (Comisiones).
- **Gestión de Despliegue (DevOps / CI-CD):** Configurar y supervisar que las ramas pasen a entornos de *Staging* (Pruebas) y *Production* (Producción) sin romper el sistema.

## 3. Rutina Semanal Sugerida
- **Lunes (Planificación):** Asignación de *Work Packages* al equipo backend. Definición de contratos de datos para la semana.
- **Martes y Jueves (Supervisión):** Revisión de PRs, desbloqueo de *Roadblocks* y programación profunda (*Deep Work*).
- **Miércoles (Sincronización):** Reunión directiva de 30 mins con CEO y Frontend Lead para evaluar integraciones cruzadas.
- **Viernes (Cierre):** Pase de código aprobado al entorno de *Staging*. Pruebas de humo (*Smoke Testing*). No se hacen despliegues a producción los viernes por norma de seguridad.
